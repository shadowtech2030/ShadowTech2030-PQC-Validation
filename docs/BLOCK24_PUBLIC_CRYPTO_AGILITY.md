# Shadow-Tech2030 PQC Engine — Block 24 Public Crypto-Agility

Shadow-Tech2030 PQC Engine is designed around replaceable cryptographic roles rather than permanent dependence on one algorithm or provider.

## Public lifecycle model

```text
LAB -> ALLOWED -> PREFERRED -> DEPRECATED -> FORBIDDEN
```

## Current preferred baseline

- KEM: **ML-KEM-1024**
- Signature: **ML-DSA-65**

## Signature diversity

- Alternate: **SLH-DSA-SHA2-256s**
- Lifecycle: **ALLOWED**
- Mathematical family: hash-based

Its presence does not imply automatic substitution.

## Future KEM diversity

- Candidate: **HQC**
- Lifecycle: **LAB**
- Role: future diversity candidate

Provider support alone is not sufficient to promote a future algorithm.

## Synthetic migration slot

Block 24 uses a synthetic next-generation KEM slot solely to validate migration and lifecycle survivability.

It is:

- not a standard;
- not a real cryptographic primitive;
- not production-ready;
- not custom cryptography.

## Custody agility

Algorithm choice is separated from key custody.

Policies can require hardware-backed custody and non-exportable private keys.

If required hardware custody is unavailable, the intended behavior is denial rather than silent software fallback.
