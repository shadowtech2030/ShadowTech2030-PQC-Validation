# Shadow-Tech2030 PQC Engine — Block 24 Public Security Boundaries

This document describes only sanitized, public authority boundaries.

## Cryptographic authority

Shadow-Tech2030 PQC Engine may enforce high-level cryptographic trust decisions such as:

- allow / deny of cryptographic operations;
- identity or credential revocation;
- key / certificate rotation;
- re-authentication or attestation requirements;
- downgrade prevention;
- SAFE_LOCAL cryptographic guardrails;
- evidence integrity and sealing.

## No direct OT process authority

Shadow-Tech2030 PQC Engine does not independently:

- stop a PLC;
- open or close a valve;
- change a process setpoint;
- alter industrial logic;
- start or stop production equipment;
- make business-process decisions.

Meaningful OT remediation remains under the authority of the relevant Shadow-Tech2030 engine, central coordination service and human operators.

## Fail-closed principle

When a required cryptographic trust condition cannot be met, the affected cryptographic operation is denied instead of silently selecting a weaker path.

## SAFE_LOCAL principle

When central coordination service is unavailable, SAFE_LOCAL preserves the last approved cryptographic policy and guardrails.

Loss of Central connectivity does not authorize weaker:

- custody requirements;
- algorithm restrictions;
- QKD requirements;
- trust requirements;
- rollback protections.

## Hardware-custody principle

The current milestone validates software contracts and routing behavior for hardware-backed custody.

It does not certify any physical HSM, TPM or secure element.

## Algorithm lifecycle principle

Public lifecycle states include:

- LAB
- ALLOWED
- PREFERRED
- DEPRECATED
- FORBIDDEN

A forbidden algorithm is not automatically resurrected.
