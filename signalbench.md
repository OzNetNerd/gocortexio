# signalbench

## Summary

SignalBench is a Rust-based endpoint telemetry generator that creates realistic attack patterns aligned with the MITRE ATT&CK framework. It executes actual OS commands that emulate technique-aligned activity while remaining safe and non-destructive, generating observable endpoint signals for security analytics development.

The tool addresses a critical gap in security operations: testing detection logic requires realistic telemetry, but creating authentic attack patterns manually is time-consuming and requires deep expertise. SignalBench automates this process, enabling security analysts, detection engineers, and SOC teams to validate their analytics against 63 techniques across 12 ATT&CK categories without needing offensive security skills.

Built in Rust for performance and safety, SignalBench uses static musl builds for universal Linux compatibility. Its architecture supports both single-host execution and multi-host attack simulation via Voltron Mode, which coordinates distributed techniques across networked systems using encrypted JSON-RPC communication. The tool generates authentic protocol traffic (SSH, VNC) and comprehensive endpoint telemetry (process creation, file operations, network connections) that mirrors real-world adversary behavior.

SignalBench integrates with Cortex XSIAM and XDR platforms through HTTP endpoint ingestion, making it ideal for testing detection rules, correlation searches, and behavioral analytics in Palo Alto Networks security deployments. The tool's dry-run mode, automatic cleanup, and force mode (for bypassing environment checks) make it suitable for both production security testing and research environments.

## Key Use Cases
- Security analytics development and testing
- Research and training scenarios with realistic telemetry
- Multi-host attack simulation via Voltron Mode
- Detection engineering and security product evaluation
- Endpoint threat behavior emulation (63 techniques across 12 categories)

## Prerequisites & Palo Alto Tools

### Prerequisites
- Linux operating system (x86_64 or ARM64 architecture)
- Static musl build provides universal Linux compatibility
- Root/sudo access for some MITRE techniques
- For Voltron Mode: Network connectivity between hosts, TLS certificates for encrypted communication

### Palo Alto Integration
- **Cortex XSIAM** - HTTP endpoint ingestion
  - Ingests generated telemetry via HTTP endpoint for detection rule testing
  - Validates correlation searches and behavioral analytics
- **Cortex XDR** - Endpoint detection
  - Generates attack signals for endpoint detection testing
  - Tests agent behavior and detection capabilities

## Repository Information
- **Last Updated**: 2026-01-18
- **Repository**: https://github.com/gocortexio/signalbench

*Summaries generated with AI from repository documentation and commit history. Please review the source repositories' README files for full and comprehensive descriptions.*

## Recent Changes
- `b07b984` - SignalBench v1.6.47 - Chasing easy wins because not ready for time sink that will be 1.7.x (2026-01-18)
- `7e5db61` - Use secret for SEMGREP_REPO_DISPLAY_NAME (2025-12-21)
- `f6bf585` - Refactor Semgrep workflow for improved clarity (2025-12-21)
- `3c99547` - v1.6.41: Nobody Puts ~~Baby~~ SignalBox In A ~~Corner~~ Container (2025-12-06)
- `58b52ce` - SignalBench v1.6.19: Voltron Mode for multi-host attack simulation (2025-11-23)
- `0ffb4a3` - Expanded to 42 techniques, add 5 new supersized techniques, upgrade 4 existing (2025-11-15)
- `384f25f` - Cleaned up .DS_Store (2025-11-04)
- `90c7355` - Release v1.5.13: The Supersized Menu (2025-11-04)
- `7b74ee5` - Release v1.4.3: Malware simulations, universal Linux compatibility, enhanced reliability (2025-10-24)
- `6450e8f` - Initial commit: SignalBench v1.1.1 - Linux endpoint telemetry generator (2025-09-12)

## Tags
![mitre-attack](https://img.shields.io/badge/mitre--attack-28a745?logo=hackthebox&logoColor=white) ![detection-testing](https://img.shields.io/badge/detection--testing-ff6b35?logo=checkmarx&logoColor=white) ![training](https://img.shields.io/badge/training-ff6b35?logo=googlescholar&logoColor=white)

---
*Auto-generated on 2026-01-19*
