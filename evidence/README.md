# Shadow-Tech2030 PQC Engine — Public Evidence

This directory is reserved for public, non-sensitive validation evidence related to Shadow-Tech2030 PQC Engine.

Its purpose is to support technical claims without exposing proprietary intellectual property.

## Suitable public evidence

Future artifacts published here may include:

- sanitized validation reports;
- validation summaries;
- benchmark results;
- public test statistics;
- independent review summaries;
- hardware validation summaries;
- reproducible non-sensitive test outputs;
- evidence manifests;
- SHA-256 hashes;
- signed public manifests;
- architecture snapshots;
- release-specific validation records.

## Evidence requirements

A public evidence artifact should clearly identify:

- what was tested;
- when it was tested;
- the relevant validation snapshot or version;
- the expected result;
- the observed result;
- the validation status;
- known limitations.

Where appropriate, evidence should include a cryptographic hash so that later modification can be detected.

## Hashes

The repository-level `SHA256SUMS` file contains SHA-256 integrity hashes for published artifacts.

A cryptographic hash can demonstrate that an artifact matches a known version.

A hash alone does **not** prove who created or published the artifact.

## Digital signatures

Shadow-Tech2030 may later publish detached digital signatures for selected evidence artifacts.

Official signatures should only be produced using a dedicated Shadow-Tech2030 signing identity whose private key is appropriately protected.

Temporary, development or personal keys must not be represented as official Shadow-Tech2030 validation signatures.

## Evidence that must remain private

This directory must not contain:

- Shadow-Tech2030 source code;
- complete internal automated tests;
- proprietary algorithms;
- proprietary heuristics;
- internal trust policies;
- private keys;
- credentials;
- authentication secrets;
- sensitive test vectors;
- detailed exploit chains;
- detailed attack-path maps;
- customer information;
- production data;
- private repository information;
- confidential partner information.

## Evidence philosophy

Shadow-Tech2030 follows three principles:

**Evidence over claims**

Security statements should be supported by measurable evidence.

**Transparency without disclosure**

Validation results can be shared without publishing proprietary implementation details.

**Limits are part of the evidence**

Every public result should identify what it demonstrates and what it does not demonstrate.

---

## Current public milestone

**Shadow-Tech2030 PQC Engine**

**838 automated tests passed — 0 failed**

This is an internal software-validation milestone.

It is not presented as independent certification.

See:

- [`../VALIDATION_SNAPSHOT.md`](../VALIDATION_SNAPSHOT.md)
- [`../EVIDENCE_POLICY.md`](../EVIDENCE_POLICY.md)
- [`../docs/VALIDATION_FLOW.md`](../docs/VALIDATION_FLOW.md)

---

**Shadow-Tech2030 Inc.**

*Passive & Secure by Design*

https://shadowtech2030.ca
