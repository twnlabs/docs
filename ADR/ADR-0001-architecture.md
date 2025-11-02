# ADR-0001: Architecture Overview and Principles

Status: Accepted
Date: 2025-10-01  # Aligned with Q4 2025 roadmap acceptance window
Owners: Architecture Council (Product, Engineering, Security)

Context
- Identity‑native AI twin platform anchored by iNFT ownership on Solana; public, verifiable transparency is a core requirement.
- Priorities: security, privacy, and stability; low‑latency UX; deterministic accounting and reporting.
- Governance: multisig (2‑of‑3) with a timelock applied only to non‑spending iNFT identity/transfer controls. No timelock for financial/market operations.

Decision
- Adopt a modular, security‑first architecture:
  - On‑chain programs (Anchor) for iNFT/identity/transfer policy.
  - Off‑chain services for AI orchestration, the airdrop engine, and the reporting pipeline.
  - Public read‑only API; private/authenticated endpoints are kept separate (a future private/partner spec).
  - Deterministic reporting (CSV/JSON + SHA‑256 checksums); wallet‑level distributions published.
  - Multi‑repository layout: `contracts`, `twn-ops`, `transparency`, `docs`, `sdk-*`, `web`, etc.
- Preserve immutable tier weights 10:5:1 (Gold/Silver/Bronze) and caps; other parameters via multisig.
 - Human‑in‑the‑loop approvals (execution guardrail): Any funds movement generated from allocation artifacts MUST pass dual human approvals (two distinct approvers, two distinct wallets) with an attestation bundle that includes triple‑source verification references prior to making Squads proposals executable.

Scope / Non‑Goals
- In scope: identity/iNFT, public read‑only API, airdrop/reporting pipeline, transparency artifacts, SDKs.
- Out of scope: dividends/rewards sharing; claim‑based airdrops; putting PII on‑chain; timelock for market operations.

Alternatives Considered
- Single monolithic service/repo: simpler CI but weaker separation of concerns and scalability.
- Pure on‑chain accounting: more complexity/fees and operational friction; chose off‑chain reporting with optional on‑chain pointers.
- Claim‑based user flow: UX and security costs (phishing/claims management); chose direct airdrops.

Consequences
- Pros: verifiability, modular evolution, transparent reporting, low barrier for integrations.
- Cons: stricter IDL/SDK versioning discipline, schema management, multi‑repo coordination overhead.

Notes
- Core iNFT tier distributions are designed as direct airdrops (no claim step) for simplicity and security.
- Social/community reward campaigns (e.g., Discord/Twitter/3rd‑party XP/level programs) MAY use either direct airdrops or claim‑based flows depending on campaign mechanics and risk controls.

Risks & Mitigations
- MEV/route risk: TWAP/DCA and (where possible) private routing; slippage limits and full route reporting.
- Snapshot consistency: finalized (executed) slot + UTC timestamp; tier‑local carryover rules.
- Data exposure/PII: no PII on‑chain; public API is read‑only; rate limiting and “no‑PII” response schemas.
- Operational risk: idempotent jobs, retries/backoff, monitoring/alerts, immutable logs.
 - Approval & provenance risk: Require a signed `propose-report.json` attestation bundle containing inputs digests and verification references; archive alongside monthly artifacts.

KPIs / SLOs
- Airdrop and monthly report targeted within 7 days after month‑end; <0.1% failed transfers after retries.
- Tx‑hash coverage and checksum verification rate; API p95/p99 latency targets.

References
- Whitepaper §§9–12, §21; Token Economy §§4–15.
- OpenAPI (public): `docs/API/openapi.yaml` (security: []).
- Transparency schemas: `https://schemas.twnlabs.com`.
