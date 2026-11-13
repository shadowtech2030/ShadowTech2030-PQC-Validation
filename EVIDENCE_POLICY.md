# Public Evidence Policy

Shadow-Tech2030 publishes selected evidence to support security claims while protecting proprietary intellectual property.

## Public evidence may include

- test counts and high-level test categories;
- build or snapshot identifiers that do not expose private repository structure;
- SHA-256 hashes of public artifacts;
- cryptographic standards used;
- sanitized architecture diagrams;
- reproducible non-sensitive benchmarks;
- independent validation reports when available;
- signed public manifests once an official Shadow-Tech signing key is established for this purpose.

## Evidence that remains private

The following are not published by default:

- source code;
- complete internal tests;
- proprietary algorithms and heuristics;
- detailed policy logic;
- private keys and credentials;
- detailed exploit chains or attack-path maps;
- sensitive test vectors;
- production or customer data;
- internal infrastructure details that would materially reduce security.

## Hashes vs signatures

`SHA256SUMS` provides integrity hashes for the public artifacts in this repository.

A hash proves that a file has not changed relative to a known hash. It does **not** prove who published it.

Detached signatures should only be added after Shadow-Tech2030 establishes and protects an official signing key for public evidence. No generated or temporary key should be represented as an official Shadow-Tech signature.

## Publication rule

A public artifact should answer:

1. What claim is being supported?
2. What evidence supports it?
3. What are the limits of that evidence?
4. Can the public artifact be verified without exposing proprietary implementation details?

If those four questions cannot be answered clearly, the artifact should not be published.
