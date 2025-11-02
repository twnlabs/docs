# Contributing

Thank you for contributing to the TWN Labs documentation.

## Scope
- This repository contains public documentation (Whitepaper, Token Economy, Litepaper, Roadmap, Legal), Architecture Decision Records (ADR), API specs, and market articles.
- No secrets, private keys, or personal data (PII) should ever be added.

## Style & language
- English only; clear and concise writing.
- Headings use `#`/`##`/`###` hierarchy; sentence‑case titles.
- Use code fences for commands or data formats; avoid inline HTML.
- Dates use `YYYY‑MM‑DD` (e.g., `2025‑10‑01`).

## File and directory naming
- Use snake_case for all new file and directory names (e.g., `market_opportunities.md`).
- Transitional note: legacy names MAY exist temporarily; do not introduce new kebab‑case. Prefer `snake_case.md` for new content.

## Document metadata
- Whitepaper/Token Economy/Litepaper should include Version and Date blocks near the top.
- ADRs include Status, Date, Owners; see ADR section below.

## Commit messages
- Use Conventional Commits:
  - `docs:`, `feat:`, `fix:`, `refactor:`, `chore:`, `ci:`
  - Examples:
    - `docs: add market_growth_potential article`
    - `docs: update token_economy EIP transition note (post‑vesting)`

## Branch & PR workflow
- Create feature branches using snake_case: `feature/add_market_articles`.
- Keep PRs focused and small; include a summary of changes and motivation.
- Ensure links render correctly; avoid dead links.
- Reference related issues/ADRs when applicable.

## ADR workflow
- Location: `docs/ADR/ADR-####-short_title.md` (short_title in snake_case).
- States: `Proposed` → `Accepted` → (optionally) `Superseded`.
- Template sections: Context, Decision, Scope/Non‑Goals, Alternatives, Consequences, Risks/Mitigations, KPIs/SLOs, References.
- When an ADR decision changes, add a new ADR that “Supersedes” the previous.

## OpenAPI and API docs
- Public spec is at `docs/API/openapi.yaml`.
- Public/read‑only only: no auth/securitySchemes; set `security: []` globally.
- Use `short_id` for twin routes (e.g., `/twins/G0`), and keep schemas strictly non‑PII.
- Rate‑limit headers should be documented (`X‑RateLimit‑*`, `Retry‑After`).
- Do not expose internal/private endpoints in this repository.

## Market articles
- Place under `docs/market/` using snake_case filenames (e.g., `competitive_landscape.md`).
- Keep content non‑binding and consistent with Whitepaper/Token Economy terminology.
- Add a short “Sources” block if external figures are cited.

## Legal & licensing
- License: MIT for the repository unless otherwise stated.
- Legal contact: `legal@twnlabs.com` for policy/terms questions.

## Security & disclosure
- Do not include secrets or private data.
- Report issues privately to `support@twnlabs.com` with subject “Vulnerability Disclosure – Docs”.
- Coordinated disclosure: initial response target 72h; please avoid public issues for security findings.

## Review & ownership
- CODEOWNERS (if configured) defines reviewers/approvers for key paths.
- Whitepaper/Token Economy changes typically require product + legal review.
- ADR changes require architecture review.

## Checklist (before opening a PR)
- [ ] Filenames/directories use snake_case
- [ ] English language; headings and dates formatted per guide
- [ ] Cross‑links work; no dead external links
- [ ] OpenAPI changes (if any) match actual handlers; no PII
- [ ] ADR updated/added if a decision was made or changed
- [ ] Conventional Commit message used

## Brand assets (brand-kit)
 - Brand assets are maintained in the separate `twnlabs/brand-kit` repository.
   - Structure: `logo/`, `collection_logo/`, `wordmark/`, `icons/`, `banners/`, `wallpapers/`, `guides/`.
   - See that repo’s README for usage, versioning, and releases.
- Prefer SVG for logos; PNG/WebP for banners/wallpapers.
- If Git LFS is used, ensure `.gitattributes` tracks heavy binaries.
- See `twnlabs/brand-kit` → `VERSIONING.md` and `RELEASES.md` for versioning and publishing.
 - Collection logos: see `twnlabs/brand-kit` → `collection_logo/svg/` and `collection_logo/png/`.
   - Naming: `twnlabs_{tier}_collection_logo.svg|png` (e.g., `twnlabs_gold_collection_logo.svg`).
