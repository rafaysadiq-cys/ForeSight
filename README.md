<p align="center">
  <img src="assets/foresight_logo_full.svg" alt="ForeSight Digital Forensics" width="380" />
</p>

<h3 align="center">Enterprise Digital Forensics Workstation &amp; Centralized Governance Platform</h3>

<p align="center">
  ISO/IEC 27037 &amp; NIST SP 800-86 aligned acquisition, deep artifact analysis, and real-time lab supervision.
</p>

---

## Latest Release — ForeSight Workstation `v2.4.0-pro`

| Component | Platform | Status | Download |
| :--- | :--- | :--- | :--- |
| **ForeSight Workstation (`Foresight.exe`)** | Windows 10 / 11 (x64) | Latest Stable (`v2.4.0-pro`) | [Download via Releases](https://github.com/rafaysadiq-cys/ForeSight/releases/latest) |
| **ForeSight Headquarters Portal** | Web Command Center | Live Portal | [foresight.byrs.online](https://foresight.byrs.online) |

> Check [CHANGELOG.md](CHANGELOG.md) for release notes and SHA-256 verification instructions.

---

## Platform Overview

ForeSight separates field forensic execution from centralized organizational governance across two dedicated components:

1. **ForeSight Workstation (Windows x64 Desktop Client + Analytics Engine)**
   - **Evidence Integrity:** Hardware-style software write-blocking with dual streaming `SHA-256` & `MD5` verification.
   - **Deep Forensic Analysis:** Native `MBR`/`GPT` partition parsing, `NTFS` `$MFT` fixup recovery, `FAT32`, Windows `EVTX` / Registry (`REGF`) / `Prefetch` / `LNK` artifact extraction, signature carving, and timestomp detection.
   - **Zero-Trust Examiner Session:** Provisioned strictly by your Organization Administrator with enforced temporary-to-permanent password setup, USB/network policy enforcement, and real-time session locking.

2. **ForeSight Headquarters (Web Portal & Telemetry Server)**
   - **Real-Time Lab Monitoring:** Live WebSocket telemetry for CPU, RAM, active forensic processes, and workstation seat assignment.
   - **Cryptographic Chain of Custody:** Immutable Merkle-linked audit ledger sealing every acquisition, verification, and administrative intervention.
   - **Remote Incident Control:** Instant workstation session locking, session termination, and hardware restriction policies.

---

## Installation & Verification

1. Download `Foresight.exe` from the [Latest Release](https://github.com/rafaysadiq-cys/ForeSight/releases/latest) page.
2. Verify file integrity before execution:
   ```powershell
   Get-FileHash .\Foresight.exe -Algorithm SHA256
   ```
3. Launch `Foresight.exe` and sign in using the Examiner Email, API Key, temporary password, and Headquarters Endpoint issued by your Organization Administrator.

---

## Standards Compliance

Built in accordance with **ISO/IEC 27037:2012** digital evidence handling guidelines, **NIST SP 800-86** forensic integration standards, and **FRE 902** self-authenticating cryptographic audit verification.
