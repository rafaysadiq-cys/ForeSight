# Changelog

All notable releases for **ForeSight Workstation** and **ForeSight Headquarters** are documented in this file.

## [v2.4.0-pro] — 2026-11-25

### Security & Governance
- Enforced authenticated per-workstation token verification on remote command acknowledgments and WebSocket channels.
- Enabled mandatory first-login temporary-to-permanent password rotation for newly provisioned examiners.
- Enforced real-time non-dismissible Workstation Lock Screen synchronized with Headquarters WebSocket & heartbeat state.
- Hardened backend authentication with sliding-window rate limiting, production schema lockdown, and strict multi-tenant isolation.

### Workstation & Analytics
- Full `.NET 9` WPF Workstation release (`win-x64` standalone) with minimal HQ-linked sign-in flow.
- Integrated evidence acquisition sealing and automated report submission to Headquarters Vault.
- Validated Python deep forensic engine (`MBR`/`GPT`, `NTFS`/`FAT32`, carving, `EVTX`/`REGF`, timestomp detection).

### Headquarters Web Platform
- Added live cloud portal support (`https://foresight.byrs.online`), direct installer streaming, and automated examiner credential notifications.
- Upgraded interactive topology map, audit category filtering, custom dropdown controls, and SVG brand identity.

### Release Checksum (`Foresight.exe` — Windows x64 Standalone, 135 MB)
- **SHA-256:** `A9159C566E647850195CD4E2683473F3EFBEB516FDEF9CFD2DFE7A763CF9E4CE`
