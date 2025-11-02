
# TWN Token Economy 

**Identity-Native AI Twin Platform**  

**Date:** October 2025

> **TWN Labs leverages on‑chain identity to power creator‑owned AI twins and agents, with integrated governance and verifiable provenance.**

---

## Table of Contents

1. Supply & Parameters
2. Launch & T₀ Team Acquisition
3. Team Lockup & Vesting (6 months, linear)
4. Community Distribution — iNFT (Identity NFT) Tiers
5. Platform Revenues → TWN (monthly)
6. Wallet Purposes
7. Liquidity & Security
8. On‑chain Costs & Fee Handling (operational)
9. Post‑vesting (Phase 2)
10. Snapshot & SLA
11. Eligibility (per snapshot)
12. Governance & Parameter Changes
13. Transparency & Wallet‑Level Reporting
14. Anti‑Sybil & Community Conduct
15. Quarterly Reports — Publication
16. Operational Disclaimers
17. Legal Notice & Disclaimers (Summary)

---

## 1) Supply & Parameters

- Total supply (fixed): 1,000,000,000 TWN
- Decimals: 6
- Inflation / additional mint: None (fixed 1B)

## 2) Launch & T₀ Team Acquisition

- Launch model: Bonding-curve launch on Pump.fun. On graduation, the project intends—subject to platform mechanics and market conditions—to create a liquidity pool on PumpSwap (and/or Raydium) and target LP lock/burn per platform mechanics. Live parameters and on-chain tx references will be published at launch.
- T₀ acquisition: At TGE, the team purchases on the public bonding‑curve targeting **20% of total supply (200,000,000 TWN)**. Purchased tokens are immediately locked and vest linearly over six months; the vested portion is programmatically routed at the published split — 50% Treasury / 35% Community / 15% Developer. All addresses and tx‑hashes are published in monthly reports; additional policies and disclosures apply.

## 3) Team Lockup & Vesting (6 months, linear)

- The acquired 200,000,000 TWN is intended to be locked and released linearly over 6 months in equal monthly tranches.
- Indicative monthly unlock (gross): ≈33.33M TWN
- Split of each monthly unlock (at time of unlock):
  - 50% → Treasury
  - 35% → Community
  - 15% → Developer
- Program wallets are operated via multisig (2‑of‑3); timelock applies only to non‑spending iNFT identity/transfer controls (via Squads v4); addresses and txids are published in official channels.

## 4) Community Distribution — iNFT (Identity NFT) Tiers (simple & transparent, direct airdrop)

- Rule: 1 account = 1 iNFT (Identity NFT) total. A wallet may mint exactly one iNFT in one of the tiers (Gold or Silver or Bronze). Once minted, the same account cannot mint another tier.
- Enforcement: Designed to be enforced by smart contracts and platform policy.
- Tier configuration (immutable weights & caps; prices may change):
  - Gold: cap 100, mint price 5 SOL
  - Silver: cap 250, mint price 2.5 SOL
  - Bronze: cap 1000, mint price 0.5 SOL
 - Monthly iNFT distribution budget (vesting period, first 6 months): **≈5.83M TWN** (funded solely from §3 — 50% of the Community allocation; §5 platform revenues are not used during this period) allocated by price‑aligned weights Gold:Silver:Bronze = **10:5:1** (**weights are immutable**)
  - Gold: **≈3.65M TWN / month**
  - Silver: **≈1.82M TWN / month**
  - Bronze: **≈0.36M TWN / month**
 - Post‑vesting (Month 7+): Monthly distributions continue from **Platform Revenues → TWN** with a variable amount (no fixed nominal figure). Split and transparency rules remain unchanged.
 - Per‑twin shares (post‑vesting): Within each tier, distributions are performance‑weighted based on transparent usage and outcome metrics (e.g., active users, sessions/minutes, API requests, engagement and retention). Rewards for iNFT holders are proportional to their twin’s measured performance within the same tier, normalized to the monthly tier budget, and always respecting the immutable tier weight hierarchy.

- Transferability & Locks (iNFT): iNFTs are non‑transferable for the first 6 months (immutable program/policy lock). From month 6, an early‑unlock off‑chain vote is held among iNFT holders on the TWN Labs platform; vote weights respect tier weights (Gold 10, Silver 5, Bronze 1). If early‑unlock passes, multisig + timelock executes the change on‑chain; otherwise, locks open automatically and immutably at month 12. During the lock period, snapshot‑based monthly distribution eligibility remains in effect. Transparency: off‑chain vote → signed, timestamped report with content hash/CID (Arweave); on‑chain execution (proposal/queue/execute via multisig + timelock) → tx‑hashes listed in the monthly report.
- Snapshot & airdrop (every month):
  - Snapshot time: Month-end (one block/slot reference published).
  - During Months 1–6 (vesting), per‑wallet equality within a tier applies: For a tier with N distinct wallets at snapshot, that month’s tier_budget ÷ N is airdropped per wallet in that tier.
  - Early-minter advantage (example): Month 1: Only 10 Gold wallets exist → each receives ≈3.65M ÷ 10 = ≈0.36M TWN. Month 2: Gold total rises to 60 → each receives ≈3.65M ÷ 60 = ≈0.06M TWN for Month 2.
  - If a tier has N = 0 in a month: The full monthly amount carries forward inside the same tier until wallets exist (tiers do not cross-subsidize).
  - Rounding (deterministic): All TWN calculations at the smallest token unit (1e-6). Per-wallet amounts are floored to whole smallest units; any remainder carries forward to the same tier next month to keep sums exact. SOL fees/transfers are denominated in lamports (1e-9 SOL) and reported accordingly.
  - Per-tier remainders (carryovers) are tracked and published in the monthly report; on-chain references may be added; carryovers are added to the next month’s tier budget before per-wallet splits.

An example table (Month-by-Month per-tier splits at different N) is published alongside the monthly reports.

## 5) Platform Revenues → TWN (monthly)

- Source: Platform NFT mint revenues are accrued in SOL during the month.
- Conversion: SOL platform revenues are converted to TWN using TWAP/DCA execution (Jupiter) as needed, potentially multiple times per month; where available, MEV‑aware/private routing is used.
- Distribution (in TWN): 50% Treasury / 35% Community / 15% Developer into the same program wallets.
- Transparency: Monthly reports publish swap routes, execution parameters (slippage/caps), revenues and expenses, and all related transaction hashes (txids).
 - Unspent balances: Unspent monthly allocations may remain in their respective wallets and roll forward; usage aligns with §6 and is reported in monthly reports.

## 6) Wallet Purposes 

- Treasury: Infrastructure & hosting, data infrastructure & storage, observability & monitoring, audits & security, custody & key management, marketing & partnerships, listings/integrations, vendor services & subscriptions, legal/compliance, insurance, emergency reserves, strategic liquidity support.
- Community: iNFT holder rewards, in‑app rewards, community incentives, activations & grants, games, giveaways & challenges, governance participation.
- Developer: Core team compensation, contributor bounties & grants, R&D & maintenance, training & onboarding.



## 7) Liquidity & Security

- Liquidity: On Pump.fun graduation, a liquidity pool is created on PumpSwap (and/or Raydium) and LP is burned/locked; graduation and LP details are included in the launch report.
- Security & transparency: Multisig wallets, transparent on-chain ops, monthly revenue and expense reports with txids.

## 8) On-chain Costs & Fee Handling (operational)

- Distribution method: Direct airdrop to recipient wallets each month (no claim required).
- ATA creation: We intend to fund required ATAs where feasible; costs vary with network conditions; budgets may be adjusted.
- Cost posture: Solana fees are low and variable with network conditions; exact monthly fee totals (including any funded ATAs) are itemized in the public report with transaction hashes.
- On-chain fees (including ATAs) are generally paid from the **Treasury Wallet** as an operational expense; treatment may be adjusted.

## 9) Post-vesting (Phase 2)

- When vesting ends (the Community monthly budget from §3 concludes at Month 6).
- From Month 7 onward, monthly distributions are intended to continue via the “Platform Revenues → TWN” (§5) mechanism: after the monthly conversion to TWN, allocate 50% Treasury / 35% Community / 15% Developer.
  The 50/35/15 wallet split remains unchanged in Phase 2; the “new rewards‑based distribution model” refers to Community distributions, not the wallet split, unless changed via governance (§12).
- Phase 2 unlocks in‑platform and external usage:
  - Subscriptions: twin/agent use cases (notification assistant, chat/tasking, voice/video/text interactions)
  - APIs: external integrations (e.g., TTS with cloned voice, appearance/character‑based content generation, integrations with third‑party models)
  - OAuth: link twins to user apps and trigger workflows
- A new rewards‑based distribution model will be published in Phase 2:
  - Not profit sharing or dividends; rewards‑oriented only
  - Designed to be collection/tier‑aware and metrics‑driven
  - Portions of the Community wallet may be allocated to games, giveaways, and challenges
- Phase‑2 parameters are adopted via multisig; iNFT identity/transfer policy changes additionally require a 48h timelock (via Squads v4). Changes are forward‑dated and effective from the following distribution cycle.

## 10) Snapshot & SLA

 - Snapshot time: End of month at 23:59:59 UTC. A canonical block/slot reference will be published with the monthly report on twnlabs.com.
 - The snapshot references a finalized slot to avoid reorg inconsistencies.
 - Execution & reporting targets: Direct airdrops and the monthly report are targeted within 7 calendar days after month‑end.

## 11) Eligibility (per snapshot)

- Eligibility is determined strictly by ownership at the snapshot reference. Transfers after the snapshot do not affect that month’s distribution and are reflected in the next month.
- Monthly per-wallet amounts vary based on the fixed tier weights (10:5:1), the caps, and the number of eligible wallets in each tier at snapshot. From Month 7 onward (post‑vesting), performance metrics per twin within each tier inform relative shares as described in §4.

## 12) Governance & Parameter Changes

- Caps and tier weights are immutable (weights fixed at 10:5:1 across tiers/collections).
- No future tier may exceed the core tiers’ weights; the **10:5:1** hierarchy is preserved for any additional tiers.
- Other parameters, such as snapshot policy, are updated via multisig; iNFT identity/transfer policy changes additionally require a 48h timelock. All changes are forward‑dated (never retroactive) and take effect from the next distribution period.
- Initial governance parameters:
  - Multisig threshold: 2-of-3
  - Timelock delay: 2 days

## 13) Transparency & Wallet‑Level Reporting

- Monthly reports include: revenues, expenses, swap routes, slippage, all related transaction hashes (txids), per‑tier carryovers, and downloadable CSV/JSON allocation files.
- A wallet‑level breakdown of distributions is published on `twnlabs.com/transparency/monthly-reports`.

## 14) Anti‑Sybil & Community Conduct

- Platform‑level protections are in place against Sybil behavior. Accounts violating platform policies may be closed.
- Users who share misleading information or publish others’ data as their own will be banned upon detection.
- Community respect is a core principle; participation requires adherence to community guidelines.

## 15) Quarterly Reports — Publication

- Cadence & targets: Targeted within 15 calendar days after each quarter end (Q1/Q2/Q3/Q4).
- Channels: `twnlabs.com/transparency/quarterly-reports` (HTML page + downloadable artifacts) and announcement on official social channels (X/Discord). A GitHub mirror with checksums is maintained.
- Contents (at minimum):
  - Treasury balance and movements; Community and Developer summaries
  - Revenue breakdown (by source), monthly conversions summary (routes, slippage), and distributions (50/35/15)
  - Tier‑level carryover summary and highlights
  - Operating expenses (including on‑chain fees and ATA creations)
  - Security & compliance updates; audit status if applicable
- Artifacts: PDF summary + CSV/JSON data exports; SHA256 checksums published. (Optional) On‑chain MEMO referencing the report hash/CID.

---

## 16) Operational Disclaimers

- All schedules and metrics are non‑binding targets and may change due to technical, market, or regulatory conditions.
- Distribution timing, tx‑hash coverage, and fee handling are best‑effort and depend on network conditions.
- Third‑party platform mechanics (e.g., Pump.fun, PumpSwap, Raydium, Arweave, Squads) may change; the project adapts accordingly.
- Governance may adjust parameters (e.g., fees, budgets, reporting cadence) with forward‑dated decisions.

## 17) Legal Notice & Disclaimers (Summary)

This document is product information and not investment advice. Features and parameters may change. Owning TWN or an iNFT does not grant profit or dividend rights. Regional restrictions and technical/market risks apply.

- Age/eligibility: Access may require that you are of legal age and otherwise eligible under local law; availability varies by jurisdiction.
- Key/wallet responsibility: Keys and wallets are your responsibility; lost private keys and unauthorized on‑chain transactions are generally irreversible and cannot be recovered by TWN Labs.
- Smart‑contract/MEV/network risk: On‑chain transactions may fail, be reordered (MEV), or execute with slippage; transactions are typically final and non‑reversible once confirmed.
- Brand/IP notice: Third‑party marks and names are used for identification only and are the property of their respective owners.
- Utility token; no profit/dividends: TWN is for product access/usage; holding TWN or an iNFT does not entitle holders to profits, revenues, dividends, or ownership rights.
- Jurisdictional restrictions: Availability is subject to applicable law; offerings are not available where prohibited.

For comprehensive terms and privacy information, refer to the Whitepaper “Legal Notice & Disclaimers”, the Privacy Policy, and the Terms of Service. For legal, policy, or security disclosures, contact legal@twnlabs.com.

© 2025 TWN Labs. All rights reserved.
