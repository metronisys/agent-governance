# Security Tier 1: Technical Sandboxing & Isolation

To ensure that agent code is "Safe," Metronisys enforces a strict separation between the **Governor (Decision Layer)** and the **Executor (Action Layer)**.

## 1. Ephemeral Execution Environments
All agent actions must be executed in a non-persistent, hardware-isolated container (e.g., Docker, WASM, or Firecracker microVM).
- **No Persistence:** The environment is wiped after every task to prevent malware "nesting."
- **Resource Quotas:** Hard limits on CPU (max 2 cores) and RAM (max 1GB) to prevent denial-of-service (DoS) on the user's machine.

## 2. Network Air-Gapping
By default, the Executor has **zero** outbound network access. 
- Access to specific domains (e.g., a specific API) must be explicitly requested by the Executor and cryptographically signed-off by the Governor Layer.

## 3. System Call Filtering
The Executor is restricted from sensitive system calls. It cannot:
- Access the root file system (outside of a dedicated `/agent/work/` directory).
- Spawn new processes or shell environments.
- Access hardware drivers (Camera, Mic) without a specific Human-in-the-loop (HITL) prompt.

---

## Trademark & Usage

**Metronisys™** is a trademark of John A. Nudd.  
Commercial use of the name requires permission.  
Open-source usage is permitted under the license of this repository.

---

Metronisys exists to ensure that as AI agents gain autonomy,  
**governance is embedded — not bolted on**.
