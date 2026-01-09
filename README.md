# Open Sustainability Commitments on IPFS (OSCI)

Open-source tooling to store, version, and verify sustainability commitment evidence (documents + metadata) on IPFS, with optional Filecoin persistence for durable storage and retrieval.

## Why this exists

Many real-world “impact” and “sustainability” programs fail because they lack verifiable data and consistent evidence trails. Teams often store documents in centralized systems, making proofs hard to audit, easy to tamper with, and difficult to reference across applications and smart contracts.

This project provides a simple, reusable, open-source framework to:
- Package evidence (e.g., invoices, certificates, reports, proofs) with a standard metadata schema
- Generate and manage IPFS CIDs with versioning
- Persist data to Filecoin (optional, but supported as a first-class path)
- Enable verification and retrieval for applications, dashboards, and on-chain references

## What we are building (grant deliverables)

*OSCI* will ship as:
1. *A metadata schema* for “commitment evidence bundles” (JSON)
2. *A CLI + library* to:
   - create an evidence bundle
   - add files + metadata
   - pin to IPFS
   - (optionally) persist to Filecoin via storage providers / integrations
   - verify integrity and bundle history
3. *Reference implementations*
   - Example bundle types (energy invoices, recycling proofs, certifications)
   - Example retrieval + verification flow
4. *Documentation*
   - Quickstart
   - Integration guide for apps
   - Best practices for privacy and redaction

## How it uses IPFS & Filecoin

- *IPFS* is used for content addressing, integrity guarantees, and retrieval via CID.
- *Filecoin* is used (optionally) for durable, decentralized persistence of the same content, enabling long-term availability and auditability.

The project is designed to be modular: IPFS-first, with Filecoin persistence as an optional storage layer.

## Target users

- Developers building “proof-of-impact” and sustainability applications
- Communities, DAOs, and NGOs that need verifiable evidence trails
- Municipalities and companies that want auditable sustainability programs
- Teams integrating verifiable data into smart contracts and incentive systems

## Milestones (initial)

*M1 — Spec & Foundations*
- Publish schema v1 (evidence bundle)
- Repo structure + docs scaffold
- CLI skeleton and bundle creation/validation

*M2 — IPFS Integration*
- Add files + metadata, produce deterministic bundle output
- Pin to IPFS, generate CIDs, verify integrity
- Retrieval + verification commands

*M3 — Filecoin Persistence*
- Implement optional Filecoin persistence path (documented integration)
- End-to-end demo: create → IPFS CID → Filecoin persistence → retrieval

*M4 — Examples & Docs*
- 2–3 example bundle templates (e.g., energy invoice proof)
- Integration guide + demo walkthrough
- Release v0.1

## Open source

This project is open-source by design to maximize reuse across the Filecoin/IPFS ecosystem. It is intended to become a building block for many applications, not a single product.

License: MIT (with optional Apache-2.0 dual licensing if required).

## Status

Currently in specification and repository bootstrap phase. Contributions and feedback are welcome.

## Contact

For questions or collaboration: contact@sustaintoken.org
