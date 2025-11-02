# TWN Labs — Privacy Policy

Last Updated: September 2025

## 1. Introduction

This Privacy Policy explains how TWN Labs ("we", "our", "us") collects, uses, discloses, and protects information in connection with our products and services, including AI twins/agents, websites, apps, and related features (collectively, the "Services").

## 2. Scope

This policy applies to information we process when you access or use the Services, contact us, or otherwise interact with us. Additional notices may apply in specific regions or for specific features.

## 3. Information We Collect

We collect information in three ways: (a) you provide it to us, (b) we collect it automatically when you use the Services, and (c) we receive it from third parties you connect or that support our operations.

- Identifiers and Contact Information
  - Email address; display name; optional profile photo
  - Pseudonymous user IDs and hashed visitor IDs
- Wallet and On‑Chain Identifiers
  - Public wallet addresses; transaction hashes; token/NFT identifiers
  - Note: on‑chain data is public and immutable
- Twin/Persona Inputs (user‑provided)
  - Voice samples and text prompts used to create your twin
  - Appearance assets (images/video you upload), persona parameters
- Biometric‑Derived Data (with consent)
  - Voice characteristics derived from samples for clone/TTS; confidence scores
  - We do not store raw biometrics beyond what is necessary to fulfill your request
- Device, Network, and Technical Data (collected automatically)
  - IP address, device type, OS, browser, language, screen size, time zone
  - Request headers, crash/diagnostic logs, performance metrics
  - Device/browser signals used for security and fraud prevention (e.g., fingerprint signals) where permitted
- Cookies and Similar Technologies
  - Essential (authentication, security), preferences, analytics/performance
  - SDK/local storage and similar identifiers
- Usage Data and Interactions
  - Feature usage, session events, timestamps, clickstream, audio/text generation counts
- Location (approximate)
  - Country/region inferred from IP for localization/compliance
- Communications and Support
  - Messages you send us, surveys/feedback, recordings where disclosed
- Derived Data
  - Aggregated statistics, risk scores, and analytics derived from other data

We do not intend to collect special categories of data except limited biometric‑derived voice characteristics for twin creation with explicit consent.

## 4. How We Use Information

- Provide and operate the Services
  - Create/configure twins and optional capabilities at your direction
  - Process payments or on‑chain interactions you initiate
- Security, integrity, and abuse prevention
  - Authenticate sessions, prevent fraud/abuse, rate‑limit, and protect accounts
- Improve and develop the Services
  - Debugging, analytics, quality, and performance measurement
- Communication
  - Service notices, support responses, and product updates (you can opt out of non‑essential communications)
- Legal and compliance
  - Satisfy legal obligations, enforce terms, resolve disputes
- Transparency and reporting (aggregate/anonymous)
  - Publish aggregate usage and transparency metrics without identifying individuals

### 4.1 Model Training & Human Review
We do not use Customer Content (your prompts, uploads, or outputs) to train our foundation models unless you opt in. We may use aggregated, de‑identified telemetry to improve system reliability and safety. Any human review (e.g., abuse investigation or model quality checks) is access‑controlled, logged, and limited to the minimum necessary. "Customer Content" means the prompts, inputs, uploads, and outputs you submit or generate via the Services.

## 5. Legal Bases (where applicable)

- Consent: biometrics/voice processing for twin creation; certain cookies; specific marketing
- Contract: to deliver features you request and maintain your account
- Legitimate Interests: security, fraud prevention, improvement, and analytics proportionately
- Legal Obligations: record‑keeping, lawful requests, sanctions/PEP screening where required

### 5.1 Roles: Controller vs Processor
Depending on the feature, TWN Labs may act as:
- Controller for account, support, safety/fraud, and platform operations.
- Processor when delivering enterprise or customer‑directed integrations (e.g., webhooks to endpoints you control), processing data strictly under your instructions.
We describe our role per feature in applicable documentation and agreements.

## 6. On‑Chain vs Off‑Chain Data

- On‑chain data: Public and immutable. Do not include personal data on‑chain beyond what is strictly necessary for provenance/ownership. Deletion/changes on‑chain are generally not possible.
- Off‑chain data: Stored and processed under this policy and applicable privacy rights (access, correction, deletion, objection, portability). We keep off‑chain biometric data only with consent and subject to withdrawal.
- Linking: Wallet addresses and on‑chain identifiers may be linked to your account for eligibility, twin ownership, and transparency features.

## 7. Sharing and Disclosures

- Service Providers and Sub‑processors: Cloud hosting, storage, analytics, support, communications, and security vendors under appropriate agreements. We publish and periodically update a list of core service providers (processors/sub‑processors) on our website. We version and date changes to this list and provide reasonable advance notice where practicable.
- Legal/Compliance: If required by law or to protect rights, safety, or property
- Business Transfers: In connection with a merger, acquisition, or asset sale
- With Your Direction: Publishing a twin, enabling integrations, or sharing content you choose to make public. If you enable webhooks or third‑party integrations, limited data necessary to deliver those events may be sent to the endpoints you configure.
- Aggregated/De‑identified: We may share non‑personal, aggregated statistics

## 7A Public Twins, API and Platform Visibility
If you set a twin to public, you authorize TWN Labs to make the twin’s profile and any public assets or behavior endpoints discoverable and callable by other users or applications via APIs/SDKs, and viewable on TWN Labs platform surfaces (e.g., website/app profiles, search, marketplace), subject to rate limits, quotas, and policy. Public information may be indexed, cached, or mirrored by third parties. Private twins are not indexed nor exposed via public APIs; however, on‑chain metadata described in §19 remains public.

Publicly visible items (depending on your settings and applicable policies) may include:
- Basic profile information (e.g., name/handle, description, tags, languages)
- Appearance assets or references (e.g., image thumbnails or pointers)
- Voice previews/samples, if you explicitly enable previews and where permitted
- Declared capabilities or behavior endpoints, and high‑level usage indicators where applicable
- Creator handle or public identifier (e.g., wallet or profile reference)

Removal from third‑party caches or mirrors is not guaranteed and may require requests to those third parties.

## 8. Cookies and Tracking

We use cookies and similar technologies (e.g., local storage, SDK identifiers, pixels) to operate and improve the Services.

Categories we use:
- Essential & Security
  - Purpose: sign‑in/session continuity, CSRF protection, rate limiting, load balancing
  - Examples: session ID, CSRF token, gateway affinity
  - Retention: session or short‑term (hours to days)
- Preferences
  - Purpose: language, theme, UI choices
  - Examples: ui_theme, locale
  - Retention: up to 12 months (unless you clear them)
- Analytics & Performance
  - Purpose: usage metrics, diagnostics, crash reports, latency measurements
  - Examples: analytics ID, event counters
  - Retention: typically 6–13 months (provider‑dependent)
- Functional/SDK
  - Purpose: enable specific features (e.g., media playback, real‑time events)
  - Examples: feature flags, media buffer settings
  - Retention: session to 12 months
- Advertising/Marketing (if enabled)
  - Purpose: only if/when we introduce such features with consent where required
  - Default: not used by default; we will request consent before enabling

Controls and choices:
- Consent: Where required, we present a banner with granular choices (e.g., analytics, marketing). You can change preferences at any time via cookie settings (where available) or your browser controls.
- Browser controls: You may block or delete cookies; essential cookies may be necessary for the Service to function.
- Opt‑out: Some analytics allow opt‑out; we provide instructions where applicable.
- Do Not Track (DNT): We do not respond to DNT signals at this time.
- Global Privacy Control (GPC) / “Do Not Sell or Share” (CPRA): If and when we engage in activities considered a “sale” or “sharing” under CPRA, we will honor GPC/opt‑out signals for applicable flows.

Identifiers we may set or read include session IDs, CSRF tokens, pseudonymous analytics IDs, and feature flags. Third‑party providers (e.g., analytics) may set their own identifiers; their use is governed by their policies and our agreements.

## 9. Biometrics and Sensitive Data

- Consent: We collect/process voice samples and derive voice characteristics solely with your explicit consent to create/operate your twin
- Purpose Limitation: Used only to provide the requested features (e.g., TTS/voice clone) and safety, fraud, and abuse prevention related to those features
- Withdrawal: You may withdraw consent at any time in account settings or by contacting us; we will stop future processing and delete off‑chain copies subject to legal/operational constraints
- Storage and Access: Off‑chain biometric data is encrypted and access‑controlled; we avoid storing raw samples longer than necessary
- On‑Chain: We do not put biometric data on‑chain

## 10. Data Retention

We retain off‑chain personal data only as long as needed for the purposes above or as required by law. Indicative periods (subject to change):
- Account data: for the life of the account and up to 24 months after closure (or longer if required by law)
- Logs/diagnostics: 12–18 months
- Support communications: up to 24 months after resolution
- Biometric‑derived data: retained only while consent is active and necessary for the feature; deleted upon withdrawal where feasible
- Financial/transaction records: per statutory requirements
On‑chain data is not deleted.

## 11. Security

We employ technical and organizational safeguards, including encryption in transit/at rest, least‑privilege access, key management, WAF/CSP, rate‑limiting, monitoring/alerts, and regular backups. No method of transmission or storage is fully secure.

### 11.1 Incident & Breach Notification
We maintain incident response procedures. Where required by law, we will notify users or authorities of a data breach within the applicable time frames, taking into account the nature of the incident and regional requirements.

## 12. International Transfers

Where data is transferred internationally, we rely on Standard Contractual Clauses (SCCs) and, for the UK, the International Data Transfer Agreement (IDTA) or UK Addendum, or other mechanisms permitted by law. Where required, we designate an EU and/or UK representative and publish contact details on our website. We also honor data residency/localization requirements and may apply geofencing as applicable.

## 13. Your Rights and Choices

Subject to law and region, you may have rights to:
- Access, correct, or delete your personal data
- Object to or restrict certain processing
- Data portability (we provide data in a commonly used, machine‑readable format, e.g., JSON/CSV)
- Withdraw consent (where processing is based on consent)
- Lodge a complaint with a supervisory authority

Timelines and verification: We respond to verified requests within the time allowed by law (typically 30–45 days, with a permissible extension where complex). We may request information to verify your identity and protect your account.

Appeals: Where required by applicable privacy laws, you may appeal a denied request; instructions will be provided in our response.

Profiling/automated decisions: We do not make solely automated decisions that produce legal or similarly significant effects without appropriate safeguards; where applicable, you may opt out or request human review.

## 14. Children’s Privacy

The Services are not directed to children under 13 (or the minimum age required by local law where higher, such as 16 in parts of the EU/UK). We do not knowingly collect personal data from children without required consent. If you believe a child has provided data to us, contact us to request deletion.

## 15. Changes to this Policy

We may update this policy from time to time. Material changes will be communicated as appropriate. Your continued use of the Services after the effective date constitutes acceptance of the updated policy.

## 16. Region‑Specific Notices

- EU/EEA/UK: TWN Labs processes data as a controller for account, support, and platform operations. Legal bases are listed above. Where we rely on consent, you may withdraw at any time. For international transfers, we use appropriate safeguards. Contact us for details.
- Canada (PIPEDA / Quebec Law 25): You may have rights to access, correction, and deletion, and to object to certain processing. Where applicable, we apply privacy impact assessments, incident reporting, and cross‑border safeguards.
- State Privacy Laws: You may have rights to opt out of targeted advertising, certain profiling, or the "sale"/"sharing" of personal information. We do not "sell" personal information; if and when activities qualify as "sharing," we will honor applicable opt‑out signals (including GPC) and provide controls.
- Biometrics (e.g., Illinois BIPA; Texas; Washington): Where these laws apply, we obtain written consent, disclose purpose/retention, and delete biometric identifiers within a commercially reasonable period after the initial purpose is satisfied or consent is withdrawn, unless a longer retention is required by law.
- California (CPRA): We do not “sell” personal information as defined by CPRA. We may “share” limited identifiers for cross‑context behavioral purposes only if and when such functionality is enabled; you may have the right to opt‑out of such sharing. We honor applicable CPRA rights (access, deletion, correction, portability, and non‑discrimination).
- Other Regions: Additional rights or disclosures may apply as required by local law.

## 17. Misuse, Impersonation, and User Responsibility

- You must not upload or use content (voice, images, likeness, persona, text) that you do not have the right to use. This includes cloning or attempting to clone another person’s voice or appearance without their explicit permission and applicable legal basis.
- You are responsible for the content you provide and for ensuring it complies with law and our policies. We may suspend or terminate access for violations and may notify affected parties or authorities where required by law.
- We are not responsible for false, misleading, infringing, or unlawful content provided by users or third parties, including any misuse of twins, voices, or likenesses outside our control. To the extent permitted by law, we disclaim liability for third‑party misuse.
- Creators/holders are solely responsible for the content, claims, and activities expressed by or through their twins and iNFTs. TWN Labs does not endorse such content and assumes no liability for compliance, accuracy, or infringement. Creators must ensure compliance with applicable laws and third‑party rights. We may moderate, disable, or remove content or features that violate policy or law.
- You agree not to misrepresent your identity or affiliation and not to mislead others about the nature, source, or authorization of a twin or its outputs.
- Report abuse: If you believe your rights are being infringed (e.g., voice/likeness misuse), contact us at legal@twnlabs.com with details so we can review.

## 18. On‑Chain Twin Metadata and Permanence

Certain twin metadata written to the blockchain is public and generally cannot be changed or deleted. This may include, for example:
- Twin profile name and display name
- Profile image or pointer/reference to an image (e.g., Arweave/IPFS link)
- Description or summary text
- Declared attributes such as language, date of birth (if you choose to publish), and other characteristics
- Twin ID or token/NFT identifiers
- Creator/owner wallet address
- Timestamps and program‑level references necessary for provenance/ownership

Because on‑chain records are permanent and transparent, you should not include personal data in on‑chain metadata beyond what is strictly necessary and what you are comfortable making public. Where possible, we use off‑chain storage and references for personal data so that off‑chain deletion or updates remain feasible.

Selecting “private” inside the app restricts off‑chain surfaces and API access. It does not hide or remove on‑chain records (e.g., name, image pointer, description, language, twin ID, creator wallet), which remain publicly visible.

## 19. No Warranties; Limitation of Liability

To the fullest extent permitted by law, the Services and all content are provided "as is" and "as available" without warranties of any kind, whether express, implied, statutory, or otherwise, including without limitation warranties of merchantability, fitness for a particular purpose, title, and non‑infringement. We do not warrant uninterrupted, timely, secure, or error‑free operation.

To the fullest extent permitted by law, in no event shall TWN Labs or its affiliates, officers, employees, or agents be liable for any indirect, incidental, special, consequential, exemplary, or punitive damages, or for any loss of profits, revenues, goodwill, data, or use, arising out of or related to your use of (or inability to use) the Services, whether based in contract, tort (including negligence), strict liability, or otherwise, even if we have been advised of the possibility of such damages.

To the fullest extent permitted by law, our aggregate liability for all claims arising out of or relating to the Services shall not exceed USD 0. If a zero liability cap is not enforceable under applicable law, then the cap shall be the greater of (a) USD 100 or (b) the amounts you paid to us (if any) for the Services giving rise to the claim in the twelve (12) months preceding the event.

## 20. Indemnification

You agree to defend, indemnify, and hold harmless TWN Labs and its affiliates, officers, employees, and agents from and against any claims, liabilities, damages, losses, and expenses (including reasonable attorneys’ fees) arising out of or related to: (a) your content, including any voice, image, likeness, persona, or data you provide; (b) your misuse of the Services or violation of law; (c) infringement or misappropriation of any intellectual property, privacy, or publicity rights; (d) your integrations, webhooks, or third‑party services you enable; and (e) disputes between you and any third party related to twins or outputs. We reserve the right, at your expense, to assume the exclusive defense and control of any matter subject to indemnification.

## 21. Notice‑and‑Action; Repeat Infringer Policy

If you believe your rights are being infringed (e.g., unauthorized use of voice, image, or likeness), please send a detailed notice to legal@twnlabs.com including: (i) your contact information; (ii) a description of the content and location (URLs, wallet/twin IDs); (iii) the basis for your claim; and (iv) a statement that you have a good‑faith belief the use is unauthorized. We may remove, restrict, or disable access to reported content and may suspend related accounts as appropriate. We maintain a repeat infringer policy and may terminate accounts that repeatedly infringe others’ rights.

## 22. Governing Law and Dispute Resolution

Except where prohibited by applicable law or provided otherwise for consumers in specific jurisdictions, this Policy and any disputes arising out of or relating to it or the Services are governed by applicable law without regard to conflict of laws principles. You agree to the jurisdiction and venue of courts of competent jurisdiction for all disputes that are not subject to arbitration or that proceed in court. Consumers in the EU/UK may have the right to bring claims in their country of residence under mandatory law.

## 23. Contact

legal@twnlabs.com
