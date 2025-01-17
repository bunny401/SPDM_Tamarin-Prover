# Secure Platform Device Measurement (SPDM)

## Overview
SPDM (Secure Platform Device Measurement) is a standardized protocol developed by the DMTF (Distributed Management Task Force). It is designed to facilitate secure communication and authentication between devices, ensuring trust in their identities and integrity. SPDM is widely used in environments where device attestation and secure channels are critical, such as IoT, data centers, and enterprise networks.

## Key Features
- **Device Authentication**:
  - Verifies the identity of devices using certificates issued by a trusted Certificate Authority (CA).
- **Integrity Measurement**:
  - Ensures the integrity of device firmware and configuration through cryptographic attestation.
- **Secure Communication**:
  - Establishes an authenticated and encrypted communication channel between devices.
- **Capability Negotiation**:
  - Devices negotiate supported protocol versions, cryptographic algorithms, and capabilities during the VCA (Version-Capabilities-Algorithms) phase.


## Why Use SPDM?
SPDM provides a robust framework for secure communication and trust establishment between devices. It ensures:
- **Authentication**: Only trusted devices are allowed to participate.
- **Confidentiality**: Sensitive data is encrypted during transmission.
- **Integrity**: Firmware and configurations are verified to prevent tampering.
- **Interoperability**: A standardized protocol enables integration across diverse platforms.

## Project Details
This repository models a simplified version of SPDM focusing on:
- **A single trusted CA**: Directly signs device certificates with no intermediate hierarchies.
- **Role initialization**: Assigning devices as Initiator or Responder.
- **VCA phase**: Modeling the exchange of versions, capabilities, and algorithms.
- **Simplified trust model**: Assumes secure, trusted communication channels for initialization.

---

## References
- [SPDM Specification by DMTF](https://www.dmtf.org/standards/spdm)
- [Tamarin Prover](https://tamarin-prover.github.io/) - Used for formal verification of the protocol.

