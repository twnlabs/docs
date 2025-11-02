# ADR-0002: Airdrop Engine and Reporting

Status: Accepted
Date: 2025-10-01  # Aligned with Q4 2025 roadmap acceptance window
Owners: Finance Engineering, Platform Engineering

Context
- Monthly snapshot → allocation → direct distribution; deterministic rounding at 1e‑6 precision, per‑tier carryover; no cross‑subsidy across tiers.
- First 6 months vesting: 50% Treasury / 35% Community / 15% Developer; Community ≈5.83M TWN/month distributed 10:5:1 across Gold/Silver/Bronze.
- Post‑vesting: distributions continue from Platform Revenues → TWN (same split), variable nominal amounts.
 - Community/social rewards: Select campaigns (e.g., Discord/Twitter and third‑party platforms with XP/level systems) may receive airdrops in addition to iNFT tier distributions.

Decision
- Implement a standalone airdrop engine (Node/TypeScript) with CLI:
  - snapshot:scan → inputs from private ops data (finalized slot + per‑tier wallet lists)
  - allocate → 10:5:1 weights; equal per‑wallet within tier; 1e‑6 flooring; tier‑local carryover
  - distribute → direct SPL transfers; optional ATA funding from Treasury; collect tx signatures
  - reconcile → retries for failed transfers; strict matching and reconciliation
  - report:generate → CSV/JSON artifacts + SHA‑256 checksums
- Publish artifacts to `transparency/monthly` and maintain quarterly summaries; validate with JSON Schemas and CI.
 - Social reward distributions:
   - Source of truth: campaign outputs from platform integrations (Discord/Twitter/3rd‑party) with snapshot references and integrity checks.
   - Payout method: either direct airdrop or a claim‑based flow depending on campaign mechanics and risk controls; the chosen method is documented per campaign.
   - Reporting: monthly artifacts include campaign summaries, allocation totals, and verification references.
 - Proposer integration (human‑in‑the‑loop):
   - Inputs: Use the Reporter’s finalized allocation artifacts and/or chain‑derived datasets (Ingest → R2 NDJSON/Parquet) to assemble a canonical recipient/amount list.
   - Produce `propose-report.json` (attestation bundle) including: inputs digests (hashes), allocation summary, per‑tier carryovers, and cross‑checks performed.
   - Triple‑source verification is REQUIRED prior to execution:
     1) Blockchain verification: tx/signature evidence and/or slot/snapshot proofs against chain data (Helius/DAS or RPC).
     2) Platform verification: TWN Labs internal ledger/index and monthly Reporter outputs alignment (schema‑validated).
     3) Third‑party verification: corroborating signals where applicable (e.g., Discord leaderboards/snapshots, public dashboards or external datasets referenced in the report).
   - Approvals: Two distinct human approvers using two distinct wallets must review the `propose-report.json` and sign off (2‑person, 2‑wallet policy) before any Squads proposal is marked ready for execution.

Scope / Non‑Goals
- In scope: deterministic allocation, tx signature reporting, carryover, swap route reporting.
- Out of scope: dividends/profit sharing; retroactive changes. Claim‑based flows are allowed only for social reward campaigns where mechanics require it (not for core iNFT tier distributions).

Alternatives Considered
- On‑chain distributor program: more complexity/fees; operational oversight overhead. Chose off‑chain engine + transparency.
- Pro‑rata usage weighting (Phase 2): begin with equal per‑wallet within tier, add usage signals later.

Consequences
- Pros: auditable, reproducible, cost‑efficient and fast; verifiable via CSV/JSON + checksums.
- Cons: relies on operational discipline and CI; correctness of input data (wallet lists) is critical.

Risks & Mitigations
- Input consistency: double‑check finalized slot and wallet lists; CLI guardrails and validations.
- Transfer failures: idempotent execution, batching and retries; complete tx signature coverage in reports.
- Fees/ATA creation: Treasury budgets and explicit monthly reporting; limits/slippage policy files.
 - Social/operational error: enforce human‑in‑the‑loop with dual approval and a signed attestation bundle (`propose-report.json`) archived with the monthly artifacts.

KPIs / SLOs
- <0.1% failed transfers after retries; monthly report targeted within 7 days; comprehensive tx signature coverage.
- Schema/validation CI pass rate; correct propagation of tier carryovers.
 - Verification quality: 100% proposals include triple‑source verification references; dual human approvals recorded per proposal.

References
- Token Economy §§3–8, §§10–15; Whitepaper §§10–12, §21.
- Transparency: Monthly artifacts (CSV/JSON + checksums) and schema endpoints at `https://schemas.twnlabs.com`.
- Engine CLI (planned): `twn-ops/apps`.
