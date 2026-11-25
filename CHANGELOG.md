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
- Added split cloud deployment readiness (Vercel frontend + Render backend + PostgreSQL + Resend transactional email).
- Upgraded interactive topology map, audit category filtering, custom dropdown controls, and SVG brand identity.
