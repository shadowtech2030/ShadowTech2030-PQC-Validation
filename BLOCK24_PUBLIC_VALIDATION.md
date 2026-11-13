# Shadow-Tech2030 PQC Engine — Block 24 Public Validation

**Snapshot ID:** `SQ-PUBLIC-B24-2026-10-06`  
**Date:** 2026-10-06  
**Status:** Internal software-validation milestone  
**Public scope:** Sanitized high-level evidence only

## Current milestone

Shadow-Tech2030 PQC Engine reached **Block 24 — Cryptographic Survivability** in the current internal roadmap.

| Campaign | Result |
|---|---:|
| Successive Crypto Transition Campaign | **24/24 PASS** |
| Central / Quantum / Edge E2E Validation | **10/10 PASS** |
| E2E Failure Campaign | **14/14 PASS** |
| Secure Local Continuity | **VALIDATED** |
| Crypto Diversity Slots | **READY** |

## Preferred cryptographic baseline

- **ML-KEM-1024** — preferred KEM
- **ML-DSA-65** — preferred signature

## Diversity state

- **SLH-DSA-SHA2-256s** — alternate signature family, lifecycle **ALLOWED**
- **HQC** — future KEM diversity candidate, lifecycle **LAB / FUTURE**
- Synthetic next-generation KEM slot — simulation-only for migration testing; not a real cryptographic primitive

## High-level survivability behaviors exercised

The Block 24 milestone validates, at a public level:

- explicit cryptographic lifecycle transitions;
- rejection of silent downgrade;
- algorithm deprecation and retirement;
- rejection of forbidden-algorithm resurrection;
- controlled historical verification during deprecation;
- SAFE_LOCAL preservation of approved cryptographic guardrails;
- preservation of hardware-custody requirements;
- rejection when required hardware trust is unavailable;
- lifecycle checkpoint persistence;
- rollback / tamper-anchor rejection;
- separation of cryptographic trust from OT operational authority.

## Hardware and QKD limits

The software architecture contains PKCS#11 / HSM custody boundaries and optional QKD paths.

This milestone does **not** claim:

- certification of a physical HSM;
- TPM / secure-element certification;
- QKD hardware certification;
- side-channel certification;
- physical tamper-resistance certification;
- independent third-party certification.

## Public milestone anchor

- Tag: `Shadow-Tech2030 PQC Engine-block24`
- Commit (short): `ab1fe09`

No proprietary source implementation is included.
