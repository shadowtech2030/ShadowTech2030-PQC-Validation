# Shadow-Tech2030 PQC Engine — Public Validation

**Shadow-Tech2030 Inc.**  
**Public validation repository — no proprietary source code**

Shadow-Tech2030 PQC Engine is the cryptographic trust and post-quantum security engine of the Shadow-Tech2030 ecosystem.

This public repository exists for one reason:

> **Publish evidence, boundaries and reproducible high-level validation results without exposing proprietary intellectual property.**

## Current public validation snapshot

**1 291 automated tests passed — 0 failed**

The current internal validation suite covers areas including:

- cryptographic controls;
- fail-closed policy behavior;
- anti-replay protections;
- post-quantum key establishment;
- compromise-recovery mechanisms;
- process hardening;
- software-supply-chain controls;
- authority and trust boundaries;
- evidence integrity and auditability;
- safe local behavior when central services are unavailable.

Post-quantum operations using **ML-KEM-768** and **ML-DSA-65** are exercised through OpenSSL in the current validation environment.

## Architecture boundary

Shadow-Tech2030 PQC Engine is **not** the OT decision engine.

- **central coordination service** orchestrates the HUB, presents state and decision support, and remains the point where important operational actions are presented to humans.
- **Shadow-Tech2030 PQC Engine** establishes cryptographic trust: identities, attestations, keys, certificates, policies, evidence integrity and cryptographic guardrails.
- **edge security component / industrial OT component / IT component** remain responsible for their own observation and operational context.
- **Human operators remain in the loop** for meaningful OT remediation and operational decisions.

Quantum may fail closed on intrinsically cryptographic operations when trust cannot be established. It does **not** independently stop a PLC, close a valve, alter industrial logic or make business-process decisions.

See: [`docs/ARCHITECTURE_BOUNDARY.md`](docs/ARCHITECTURE_BOUNDARY.md)

## What is public here

This repository may contain:

- high-level architecture diagrams;
- validation summaries;
- reproducible non-sensitive benchmarks;
- cryptographic standards used;
- security principles and authority boundaries;
- hashes of public evidence artifacts;
- independent validation results when available.

## What is intentionally not public

This repository does **not** contain:

- Shadow-Tech2030 source code;
- proprietary algorithms or heuristics;
- internal policy logic;
- private keys, credentials or secrets;
- sensitive test vectors;
- detailed attack-path maps;
- customer or production data;
- internal repositories or implementation details that would reduce security.

## Files

- [`VALIDATION_SNAPSHOT.md`](VALIDATION_SNAPSHOT.md) — current public validation summary
- [`SECURITY_BOUNDARIES.md`](SECURITY_BOUNDARIES.md) — what Quantum may and may not do
- [`EVIDENCE_POLICY.md`](EVIDENCE_POLICY.md) — rules for publishing public evidence
- [`docs/ARCHITECTURE_BOUNDARY.md`](docs/ARCHITECTURE_BOUNDARY.md) — sanitized architecture diagram
- [`docs/VALIDATION_FLOW.md`](docs/VALIDATION_FLOW.md) — sanitized validation flow
- [`evidence/README.md`](evidence/README.md) — evidence publication rules
- [`SHA256SUMS`](SHA256SUMS) — SHA-256 hashes of the published repository artifacts

## Important validation limits

The current public result is an **internal software-validation milestone**. It is not:

- an independent third-party certification;
- HSM/TPM hardware certification;
- physical tamper-resistance certification;
- side-channel resistance certification;
- proof that every possible attack path has been eliminated.

Hardware-backed trust and physical/side-channel resistance require dedicated validation on target hardware.

## Project principles

**Passive & Secure by Design**  
**Fail Closed where cryptographic trust is required**  
**Evidence by Default**  
**Human-in-the-Loop for OT decisions**

---

© 2026 Shadow-Tech2030 Inc. All rights reserved.  
https://shadowtech2030.ca
