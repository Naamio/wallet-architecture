# Architecture decision record

<!--
This template helps create proposals for technical and organisational decisions.
Architecture decision records are for internal decisions about how Naamio Wallet
is built, structured, and maintained. For community-facing changes, use the
request for comments template instead.

Process details: https://handbook.omnifi.foundation/engineering/architecture/adrs/
-->

## Overview

### Title
### Number
### Status
- [ ] Proposed
- [ ] Accepted
- [ ] Rejected
- [ ] Deprecated
- [ ] Superseded

### Affected projects
- [ ] Core (credential storage engine, encryption, hardware key protection, credential lifecycle, configuration)
- [ ] Credentials (OTP management, W3C VC Data Model 2.0, credential parsing, backup and migration)
- [ ] Protocols (OpenID4VCI/VP, SD-JWT VC, SIOPv2, ISO 18013-5 mdoc)
- [ ] Authentication (FIDO2/WebAuthn, passkeys, Credential Exchange Protocol, biometric binding)
- [ ] Intelligence (on-device inference, context-aware selection, service discovery)
- [ ] Automotive (CCC Digital Key, ISO 15118, ISO 23220, vehicle access)
- [ ] Sharing (credential delegation, time-limited access, encrypted sharing)
- [ ] Platforms (Android, iOS, desktop, wearable, embedded, vehicle runtimes)
- [ ] Security (post-quantum cryptography, zero-knowledge proofs, BLE/NFC)
- [ ] Other:

---

## Problem statement
### Current situation
### Decision drivers
### Constraints

---

## Proposed decision
### Chosen approach
### Rationale
### Consequences

---

## Alternatives considered

---

## Impact summary
### Technical impact
### Contributor impact
### Security impact

---

## Implementation notes
### Approach
### Verification

---

## References
### Related decisions
### External references

---

## Governance

This decision follows the
[Omnifi Foundation governance model](https://handbook.omnifi.foundation/engineering/architecture/governance/).

/label ~"adr" ~"architecture" ~"technical"
