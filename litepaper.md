# TWN Labs — Litepaper

**Identity-Native AI Twin Platform**  

**Version:** 1.0  

**Date:** October 2025

> **TWN Labs leverages on‑chain identity to power creator‑owned AI twins and agents, with integrated governance and verifiable provenance.**

---

## Table of Contents

1. Executive Summary
2. Mission, Tagline & Vision
3. Product & Experience (Twins‑First)
4. Roadmap Snapshot
5. Platform & Technology
6. Token Economy (TWN)
7. Governance, Transparency & DAO
8. Security & Privacy (Summary)
9. Business Model & Revenue Streams
10. Metrics & KPIs
11. Real‑World Use Cases (Examples)
12. Conclusion
13. Legal Notice & Disclaimers (Summary)

---

## 1) Executive Summary
TWN Labs is an identity‑native AI twin platform that enables creator‑owned AI Twins and Agents anchored by an identity NFT (iNFT) and verifiable provenance. Identity comes first: every twin, agent capability, and transaction is cryptographically tied to on‑chain identity, ensuring creator sovereignty and transparent attribution. Twins are progressively configured across voice, appearance, and persona, and can be extended via opt‑in, policy‑guarded capability packs (modular agent features). Distribution, governance, and operations are designed for transparency: monthly reports (CSV/JSON + checksums), public dashboards, and multisig + timelock controls. Utility‑first economics couple subscriptions/APIs with a transparent token model. This document is informational and not investment advice.

Foundational principles:
- User sovereignty: creator‑owned twins, bound to verifiable on‑chain identity
- Fair market design: bonding‑curve launch; no whitelist/private sale; LP lock/burn per graduation mechanics, designed to improve liquidity resilience and transparency
- Radical transparency: monthly public reporting with wallet‑level distributions and artifacts
- Utility‑first economics: usage‑based subscriptions, APIs, marketplace
- Secure, stable delivery: quarterly execution cadence with auditable milestones

---

## 2) Mission, Tagline & Vision
- Tagline: TWN Labs leverages on‑chain identity to power creator‑owned AI twins and agents, with integrated governance and verifiable provenance.
- Mission: Empower creators and users to build safe, transparent, cross‑platform twins/agents.
- Vision: Progressively decentralize into an on‑chain governed ecosystem—a “virtual state” metaphor—where iNFT holders are citizens with explicit rules, and twins/agents interoperate with games, VR/AR, and emerging surfaces.

---

## 3) Product & Experience (Twins‑First)
- Create Twin: configure voice, appearance, persona; ownership anchored via iNFT (Identity NFT: an identity NFT minted under a verified collection representing twin ownership and entitlements).
- Extend Capabilities (opt‑in): modular agent packs with explicit scopes, human‑in‑the‑loop approvals, and budgets/limits.
- Publish & Monetize: subscriptions, API keys, marketplace listings; transparency via public dashboards and monthly reports.
- Developer flow: versioned SDKs/REST, webhooks, staging flows; clear scopes and approval gates.
- Transparency & operations: bonding‑curve launch, LP lock/burn per graduation mechanics; multisig; timelock limited to non‑spending iNFT identity/transfer controls; monthly CSV/JSON artifacts.

---

## 4) Roadmap Snapshot
- Phase 1 — Foundation (2024–2025): architecture/security baseline, auth/session, programs (locker, iNFT minting, multisig/timelock), voice + text MVP, transparency/reporting pipeline, Airdrop Engine (monthly snapshot→allocation→distribution), public access prep and token launch via Pump.fun graduation mechanics.
- Phase 2 — Enhancement (Q1–Q2 2026): appearance cloning v1, LLM orchestration, subscriptions/API monetization, OAuth/linking, real‑time disclosures, early‑unlock signal (off‑chain) executed via multisig + timelock; rewards model rollout; security hardening.
- Phase 3 — Expansion (Q3–Q4 2026): DAO Go‑Live (community‑focused), marketplace features, developer portal & API marketplace (initial), mobile app (beta→GA), productization & compliance.
- Phase 4 — Ecosystem (2027+): cross‑platform interoperability (games/VR), SDK hooks, global expansion and partnerships.

Targets/SLOs: airdrop and report publication targeted within 7 days after month‑end; reliability and tx‑hash coverage tracked; community governance readiness Apr 2026.

---

## 5) Platform & Technology
Blockchain: Deployed initially on Solana (a high‑throughput, low‑fee L1 with fast finality); portability under evaluation. Verified collections and on‑chain provenance; durable storage and operational caches; multisig/timelock and scheduled audits; voice cloning and model endpoints; wallet integration and deep‑links; containerized services with gateway, caching, rate limiting, CSRF/session integrity, and observability.

---

## 6) Token Economy (TWN)
- Supply & Parameters: total supply 1,000,000,000 TWN (fixed); no inflation/additional mint.
- Launch & Liquidity: bonding‑curve launch; no whitelist/private sale; liquidity pool creation on PumpSwap (and/or Raydium) and any potential lock/burn depend on platform mechanics and market conditions; not a firm commitment.
- T₀ Team Acquisition & Vesting: 6‑month linear; ≈33.33M TWN per month (6 months = 200,000,000 TWN total, 20% T₀ pool).
- Monthly Allocation of Unlocks: 50% Treasury / 35% Community / 15% Developer.
- Community Distribution — iNFT Tiers: 1 account = 1 iNFT; caps and weights 10:5:1 (Gold:Silver:Bronze). Monthly iNFT distribution budget ≈5.83M TWN (= vesting‑derived Community allocation × 50% ÷ 6), funded solely from vesting during Months 1–6; equal per‑wallet within tiers in Months 1–6; deterministic rounding; carryover; no cross‑subsidy when a tier has N=0. From Month 7 onward, distributions continue from Platform Revenues → TWN and are performance‑weighted within each tier.
- Monthly Revenues → TWN: convert platform revenues (SOL) via time‑sliced execution (TWAP/DCA); distribute 50/35/15; report swaps and tx hashes.
- Eligibility: snapshot‑based; transfers after snapshot affect next month.
- Post‑Vesting: After vesting‑sourced Community budgets complete, monthly distributions continue from Revenues→TWN at the same 50/35/15 split.
- Parameter Changes: caps and 10:5:1 weights fixed; other parameters are updated via multisig; iNFT identity/transfer policy changes additionally require a 48h timelock. All changes are forward‑dated (never retroactive) and take effect from the next period.
- Reporting: monthly wallet‑level distributions and artifacts (CSV/JSON + checksums); quarterly summaries and SHA‑256 checksums.
- Token Utility: access and payments for features; discounts; opening quota/limit tiers; feature gates where applicable; no staking or yield.
- Anti‑Sybil & Community Rules: protections enforced; policy‑led conduct expectations.

---

## 7) Governance, Transparency & DAO
- Core: multisig (2‑of‑3) for all treasury/program wallets and upgrade authority; timelock applied only to non‑spending iNFT identity/transfer controls; monthly/quarterly reports; SLAs target snapshot/airdrop/report within 7 days.
- DAO (Decentralized Autonomous Organization) Vision: iNFT “citizenship,” constitution v0, budgeting, on‑chain traces, roles/safety mechanisms.
- Progressive Decentralization: 2026 H1 parameter signals; 2026 Q3 DAO Go‑Live; ongoing DAO influence thereafter.

---

## 8) Security & Privacy (Summary)
On‑chain program safety and governance controls; OWASP practices, WAF/CSP, input validation, rate‑limits; backups/DR, observability, structured logging; audits planned; privacy boundaries (on‑chain provenance vs. off‑chain personal data), explicit consent for biometrics, retention schedules, role‑based access, encryption in transit/at rest. Biometric samples are stored off‑chain with explicit consent, regional residency where required, and defined retention/deletion schedules.

---

## 9) Business Model & Revenue Streams
Usage‑based subscriptions (twins/agents), metered APIs (speech, models, visuals/presence), and a marketplace (iNFT sales, capability packs, service bundles). Partnerships and integrations complement core revenues. Pricing is transparent and introduced progressively; creator recognition is rewards‑based and not profit sharing.

---

## 10) Metrics & KPIs
Product activation/retention and latency/error budgets; economy conversions/distributions/carryovers; community distribution by tier; developer integrations and API success/throttling; agent approvals/budget safety; security/compliance incidents and audit closure; transparency timeliness and tx‑hash coverage; privacy‑safe analytics.

---

## 11) Real‑World Use Cases (Examples)
Creators (podcast/video), education/institutions, branded activations, games/NPC presence, monitoring/notifications, live co‑presence & community, trading assistance (approval‑gated, not financial advice), communications/support/commerce, knowledge & search (citation‑backed), developer ops, analytics/reporting, VR/metaverse co‑presence, marketplace bundles.

---

## 12) Conclusion
TWN Labs unites AI Twins & Agents with on‑chain ownership and governance to build a sustainable, transparent, creator‑centric economy—expanding scope pragmatically as the ecosystem matures.

---

## 13) Legal Notice & Disclaimers (Summary)

This document is product information and not investment advice. Features and parameters may change. Owning TWN or an iNFT does not grant profit or dividend rights. Regional restrictions and technical/market risks apply.

- Age/eligibility: Access may require that you are of legal age and otherwise eligible under local law; availability varies by jurisdiction.
- Key/wallet responsibility: Keys and wallets are your responsibility; lost private keys and unauthorized on‑chain transactions are generally irreversible and cannot be recovered by TWN Labs.
- Smart‑contract/MEV/network risk: On‑chain transactions may fail, be reordered (MEV), or execute with slippage; transactions are typically final and non‑reversible once confirmed.
- Brand/IP notice: Third‑party marks and names are used for identification only and are the property of their respective owners.
- Utility token; no profit/dividends: TWN is for product access/usage; holding TWN or an iNFT does not entitle holders to profits, revenues, dividends, or ownership rights.
- Jurisdictional restrictions: Availability is subject to applicable law; offerings are not available where prohibited.

For comprehensive terms and privacy information, refer to the Whitepaper “Legal Notice & Disclaimers”, the Privacy Policy, and the Terms of Service. For legal, policy, or security disclosures, contact legal@twnlabs.com.

© 2025 TWN Labs. All rights reserved.

