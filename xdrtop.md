# xdrtop

## Summary

XDRTop is a Rust-based terminal monitoring tool that provides real-time, interactive case tracking for Cortex XSIAM, Cortex Cloud, and Cortex XDR platforms. It delivers an htop-style interface that security analysts can use directly from the command line, enabling rapid case triage and investigation without browser overhead.

The tool solves a critical workflow problem for SOC analysts: managing security cases requires constant context switching between browser tabs, API queries, and manual filtering. XDRTop consolidates this into a single, keyboard-driven terminal interface that updates in real-time, allowing analysts to monitor case queues, filter by severity and status, and drill down into case details using intuitive keyboard shortcuts.

Built in Rust for performance and resource efficiency, XDRTop uses the Cortex Cases API to fetch and display security incidents with sub-second refresh rates. The tool's architecture includes intelligent pagination, caching, and domain-based filtering that lets analysts focus on specific threat categories. It integrates MITRE ATT&CK framework annotations directly in the terminal view, providing immediate context about adversary tactics without additional lookups.

XDRTop is ideal for SOC environments where analysts need lightweight, scriptable access to case data. Its terminal interface works seamlessly over SSH sessions, making it perfect for remote SOC operations, automated monitoring scripts, and analysts who prefer keyboard-driven workflows. The tool's filtering capabilities and real-time updates make it especially valuable during incident response when rapid case assessment is critical.

## Key Use Cases
- Real-time terminal monitoring of Cortex Platform security cases
- Case triage and investigation without browser access
- Severity and status filtering for focused incident response
- MITRE ATT&CK framework integration for threat intelligence
- Domain-based filtering for security and posture management

## Prerequisites & Palo Alto Tools

### Prerequisites
- Linux, macOS, or Windows operating system
- Rust toolchain (for building from source)
- Valid Cortex Platform API credentials (API key and tenant URL)
- Network access to Cortex API endpoints
- Terminal with ANSI color support (for optimal display)

### Palo Alto Integration
- **Cortex XSIAM** - REST API (Cases API)
  - Real-time case monitoring via Cases API
  - Fetches case details, severity, status, and MITRE ATT&CK mappings
- **Cortex Cloud** - REST API (Cases API)
  - Monitors cloud security posture cases
  - Domain-based filtering for cloud security events
- **Cortex XDR** - REST API (Cases API)
  - Tracks endpoint detection and response cases
  - Interactive drill-down for case investigation

## Repository Information
- **Last Updated**: 2025-12-26
- **Repository**: https://github.com/gocortexio/xdrtop

*Summaries generated with AI from repository documentation and commit history. Please review the source repositories' README files for full and comprehensive descriptions.*

## Recent Changes
- `2b4ef45` - v2.1.0: Domain filtering and performance optimisation (2025-12-26)
- `d38a100` - Refactor Semgrep workflow for improved clarity (2025-12-21)
- `effb9b1` - Improve how XDRTop fetches detailed issue information for cases (2025-12-05)
- `e518fee` - v2.0.3: Cases API migration (2025-12-05)
- `56c1231` - Critical performance optimisation: resolved issue where pagination executed on every UI refresh (2025-08-22)
- `1128242` - Cortex CLI Code Scan (2025-08-11)
- `3e54ad0` - Update application to the latest version with security enhancements (2025-07-23)
- `6b06028` - Drill-down is faster with proper loading feedback and smarter error handling (2025-07-08)
- `b8c7528` - Forget Windows GitHub build scripts (2025-06-27)
- `624df6f` - Forget Windows GitHub build scripts (2025-06-27)

## Tags
![soc-operations](https://img.shields.io/badge/soc--operations-ff6b35?logo=securityscorecard&logoColor=white) ![monitoring](https://img.shields.io/badge/monitoring-ff6b35?logo=prometheus&logoColor=white)

---
*Auto-generated on 2026-01-19*
