# Security Policy

Scope
- This repository hosts public documentation (Whitepaper, Token Economy, Litepaper, Roadmap, Legal), ADRs, and API specs. It MUST NOT contain secrets, private keys, wallet seeds, or personal data (PII).
- Security reports here concern document integrity (e.g., malicious links), API spec errors leading to unsafe guidance, or build/publish pipeline exposure.

Supported versions
- We recommend using the most recently released documents/specs. Errata or amendments are published via PR and release notes.

Reporting a vulnerability
- Please do NOT open public issues for vulnerabilities.
- Email: support@twnlabs.com with subject "Vulnerability Disclosure - Docs".
- Include: affected documents/paths, version/date, impact, reproduction steps, and a minimal PoC if applicable.
- Optional encryption: We will publish a PGP public key prior to public launch. Until then, plain email is accepted. If you require encryption now, mention it and we will provide a key.

Coordinated disclosure
- Initial response target: 72 hours.
- Triage and severity assessment: within 7 days.
- Fix window: we aim to remediate or provide mitigation within 90 days (or sooner where feasible). We may request extensions for complex cases.
- Please avoid public disclosure until coordination is agreed.

Safe harbor (good-faith research)
- Non-destructive testing only; do not exploit beyond the minimum required to demonstrate impact.
- No exfiltration of data; do not access, modify, or delete data that is not yours.
- No privacy violations, social engineering, spam, or denial-of-service.
- Acting in good faith to report a vulnerability will not be the basis for legal action by TWN Labs.

Out of scope (examples)
- Typos or style preferences without a security impact.
- Issues in third-party linked sites (report to the vendor).
- DoS, volumetric attacks, or findings that require impractical preconditions.

Operational security
- CI may include link checking and security scanning for known malicious patterns in documentation. Results and cadence may evolve.
- Researcher privacy: we treat your report confidentially and will not share your identity without permission unless legally required.

Contact
- support@twnlabs.com
