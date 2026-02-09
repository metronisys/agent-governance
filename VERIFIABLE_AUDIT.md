# Governance Tier 2: Verifiable Auditability

A "Governed" agent must be able to prove *why* it did what it did. Metronisys implements an immutable logging standard to ensure transparency.

## 1. The Governance Ledger
Every decision made by the Governor—especially blocks, delays, or task modifications—is recorded in a local `governance.log` with the following schema:
- **Timestamp:** ISO 8601.
- **Input Hash:** Hash of the user's original request.
- **Governor Rationale:** The specific principle triggered (e.g., "Burnout Risk detected: User has worked 10+ hours").
- **Signature:** A cryptographic signature ensuring the log has not been tampered with by the Executor.

## 2. Reasoning Transparency
Users can query the Governor at any time using the command `metronisys --why`. 
The system will provide a human-readable explanation of the internal "Human Sustainability Check" that influenced the last 10 actions.

---

## Trademark & Usage

**Metronisys™** is a trademark of John A. Nudd.  
Commercial use of the name requires permission.  
Open-source usage is permitted under the license of this repository.

---

Metronisys exists to ensure that as AI agents gain autonomy,  
**governance is embedded — not bolted on**.
