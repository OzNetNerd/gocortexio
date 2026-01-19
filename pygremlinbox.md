# pygremlinbox

## Summary

PyGremlinBox is a specialized Python testing platform containing 71 independent modules, each implementing a different software license for supply chain security validation. It serves as a comprehensive test suite for dependency scanning tools, license compliance systems, and software composition analysis (SCA) platforms, with particular focus on Cortex Cloud's package security scanning capabilities.

The tool addresses a critical validation gap in DevSecOps: organizations need to verify that their security tools correctly identify license risks, malicious packages, and policy violations before relying on them in production. PyGremlinBox provides a controlled test environment with known license types (weak copyleft, permissive, proprietary) and simulated malware packages that security tools should detect, enabling teams to validate scanner accuracy and policy enforcement.

Built as a collection of minimal Python packages published to PyPI, each module implements a specific SPDX-compliant license with correct metadata for scanner validation. The project includes authentic license text, proper package structure, and dependency declarations that mirror real-world Python projects. Recent additions include malware simulation packages for tabletop exercises, providing safe examples of supply chain attack patterns without actual malicious code.

PyGremlinBox is essential for security teams deploying Cortex Cloud or other SCA tools. It provides objective evidence that scanning tools are correctly configured and functioning, validates that security policies trigger as expected, and serves as a training platform for security awareness programs focused on software supply chain risks.

## Key Use Cases
- Dependency scanning tool validation for licence detection
- Security policy enforcement testing
- SPDX compliance testing and verification
- Supply chain analysis and reporting
- Malware simulation packages for tabletop exercises

## Prerequisites & Palo Alto Tools

### Prerequisites
- Python 3.x environment (any version supporting pip)
- PyPI access for installing test packages
- Dependency scanning tool to validate (SCA, license scanner, etc.)
- Test Python project for installing PyGremlinBox packages

### Palo Alto Integration
- **Cortex Cloud** - Package scanning
  - Tests package security scanning and license detection accuracy
  - Validates supply chain security policy enforcement
  - Verifies identification of malicious or non-compliant packages

## Repository Information
- **Last Updated**: 2025-12-21
- **Repository**: https://github.com/gocortexio/pygremlinbox

*Summaries generated with AI from repository documentation and commit history. Please review the source repositories' README files for full and comprehensive descriptions.*

## Recent Changes
- `4117b84` - Refactor Semgrep workflow configuration (2025-12-21)
- `f842f66` - Release v1.4.6 - Major expansion and malware simulation packages (2025-11-29)
- `a614413` - Fixed license specifications in all 21 pyproject.toml files (2025-09-29)
- `35a3162` - Initial commit: PyGremlinBox policy testing platform with 22 licence packages (2025-09-20)

## Tags
![supply-chain](https://img.shields.io/badge/supply--chain-6f42c1?logo=dependabot&logoColor=white) ![policy-testing](https://img.shields.io/badge/policy--testing-ff6b35?logo=terraform&logoColor=white)

---
*Auto-generated on 2026-01-19*
