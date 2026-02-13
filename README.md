# Naamio Wallet — Architecture

Welcome! This repository is where architectural decisions for
[Naamio Wallet](https://naamio.dev) are proposed, discussed, and recorded.

## What is Naamio Wallet?

Naamio Wallet is an open source credential engine built in Rust. It provides
encrypted credential storage with hardware-backed key protection, verifiable
credential protocols (OpenID4VCI/VP, SD-JWT VC, W3C Verifiable Credentials
Data Model 2.0), and on-device intelligence for anticipatory credential
presentation.

The name Naamio is Finnish for "mask" — the face you choose to present. A
credential wallet should give people control over what they reveal, to whom,
and when.

## What this repository is for

This repository tracks architectural decisions using two complementary
approaches:

- **Decisions** capture internal technical and organisational choices — how Naamio Wallet is built, structured, and
  maintained.

- **Comments** handle community-facing proposals — changes
  to public interfaces, features, behaviour, and integration patterns that
  affect how people use Naamio Wallet.

These terms map to well-established practices — decisions are also known as
architecture decision records (ADRs), and comments are also known as requests
for comments (RFCs). We use plainer language to lower the barrier to
contribution.

Both approaches are open to everyone. You don’t need to be a maintainer or a
regular contributor to submit a proposal. If you have an idea or see something
that could be improved, you're welcome here.

## How the process works

1. **Create an issue** using one of the issue templates (decision or comment) to signal
   your intent and invite early feedback.
2. **Draft a proposal** using the document templates in `templates/`.
3. **Submit a merge request** with your proposal in `decisions/` or `comments/`.
4. **Discuss** — for decisions, technical leads review over 7–14 days. For comments,
   the community discusses for a minimum of 14 days.
5. **Decision** — once consensus is reached, the proposal is merged and becomes
   part of the project's record.

The full process, including how consensus works, how disagreements are resolved,
and what happens with urgent decisions, is documented in the
[Omnifi Foundation handbook](https://handbook.omnifi.foundation/engineering/architecture/).

## Projects in scope

Proposals in this repository may affect any part of the Naamio Wallet ecosystem:

**Core**
- Credential storage engine and encryption
- Hardware-backed key protection (Secure Enclave, StrongBox, TPM)
- Credential lifecycle management
- Configuration loading and validation

**Credentials**
- OTP management (TOTP, HOTP)
- W3C Verifiable Credentials Data Model 2.0
- Credential parsing, validation, and serialisation
- Backup, restore, and migration

**Protocols**
- OpenID for Verifiable Credential Issuance (OpenID4VCI)
- OpenID for Verifiable Presentations (OpenID4VP)
- SD-JWT Verifiable Credentials
- Self-Issued OpenID Provider v2 (SIOPv2)
- ISO 18013-5 mobile driving licence (mdoc)

**Authentication**
- FIDO2/WebAuthn passkey management
- Credential Exchange Protocol (CXP/CXF)
- Biometric binding

**Intelligence**
- On-device inference engine
- Context-aware credential selection
- Open service discovery

**Automotive**
- CCC Digital Key 3.0/4.0
- ISO 15118 Plug and Charge
- ISO 23220 mobile identity documents
- Vehicle access protocols

**Sharing**
- Policy-controlled credential delegation
- Time-limited and revocable access
- End-to-end encrypted sharing

**Platforms**
- Android, iOS, desktop, wearable, embedded, vehicle runtimes
- UniFFI bindings and platform-specific integrations
- Platform key storage detection and abstraction

**Security**
- Post-quantum cryptography readiness (ML-KEM, ML-DSA)
- Zero-knowledge selective disclosure
- Offline BLE and NFC presentation

If your proposal spans multiple areas, note all affected projects in your
proposal so the right people can weigh in.

## Governance

Naamio Wallet is governed by the [Omnifi Foundation](https://omnifi.foundation),
a community-driven organisation that stewards open source projects. The
architecture decision process — how proposals are written, reviewed, and
decided — is defined in the
[Omnifi Foundation handbook](https://handbook.omnifi.foundation/engineering/architecture/)
and applies equally to all contributors.

Decisions are made through consensus. Technical leads facilitate the process but
don't dictate outcomes. Every voice carries weight, and dissenting perspectives
are documented and valued. See the
[governance model](https://handbook.omnifi.foundation/engineering/architecture/governance/)
for full details.

## Getting started

New to the project? Here's how to get oriented:

1. **Browse existing proposals** in `decisions/` and `comments/` to see what's been
   decided and how proposals are structured.
2. **Check open merge requests** for proposals currently under discussion.
3. **Read the handbook** for
   [detailed process guidance](https://handbook.omnifi.foundation/engineering/architecture/).
4. **Open an issue** if you have questions — there are no bad questions.

## Repository structure

```
├── README.md              You are here
├── CONTRIBUTING.md        How to submit proposals
├── templates/
│   ├── decision.md        Decision template
│   └── comment.md         Comment template
├── decisions/             Accepted decisions
├── comments/              Accepted comments
└── .gitlab/
    └── issue_templates/
        ├── decision.md    Issue template for proposing a decision
        └── comment.md     Issue template for proposing a comment
```

## Code of conduct

All participation is subject to the
[Omnifi Foundation code of conduct](https://handbook.omnifi.foundation/CODE_OF_CONDUCT/).
We're committed to a welcoming, respectful, and inclusive environment.

## Licence

CC BY-SA 4.0 — see LICENCE for details.
