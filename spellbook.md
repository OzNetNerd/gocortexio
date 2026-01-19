# spellbook

## Summary

Spellbook is a Python-based toolset that streamlines the creation, validation, and deployment of Cortex Platform content packs. It provides a simplified interface layer over the demisto-sdk, abstracting complex configuration and reducing the learning curve for content developers working with Cortex XSIAM and XSOAR platforms.

The tool solves a critical workflow challenge: building content packs with demisto-sdk requires understanding complex directory structures, YAML schemas, and validation rules. Spellbook automates this complexity, enabling security engineers and detection developers to focus on content logic rather than infrastructure. It generates properly structured content packs, validates them against platform schemas, and packages them for deployment with a streamlined command-line interface.

Built in Python with CI/CD integration support, Spellbook provides templates for common XSIAM content types (CorrelationRules, ParsingRules, ModelingRules) and handles the entire content lifecycle from initialization to upload. The tool supports both manual workflows and automated CI/CD pipelines, with GitLab and GitHub Actions integration for DevSecOps teams building content at scale.

Spellbook directly integrates with Cortex XSIAM and XSOAR through the demisto-sdk, making it the standard toolchain for content development teams. Its container-ready architecture and check-init command ensure consistent development environments across teams, while direct upload capabilities streamline testing and deployment workflows.

## Key Use Cases
- Creating new content pack instances with correct structure
- Generating XSIAM content templates (CorrelationRules, ParsingRules, ModelingRules)
- Validating content against Cortex Platform schemas
- Packaging content into uploadable zip files
- Direct upload to Cortex Platform instances

## Prerequisites & Palo Alto Tools

### Prerequisites
- Python 3.11 or higher
- demisto-sdk (automatically installed as dependency)
- Docker (optional, for containerized workflows)
- GitLab or GitHub (for CI/CD integration)
- Valid Cortex Platform API credentials (for direct upload)

### Palo Alto Integration
- **Cortex XSIAM** - demisto-sdk
  - Builds and validates XSIAM-specific content packs (CorrelationRules, ParsingRules, ModelingRules)
  - Direct upload to XSIAM instances via API
- **Cortex XSOAR** - demisto-sdk
  - Builds and validates XSOAR content packs (Integrations, Scripts, Playbooks)
  - Package creation for marketplace distribution

## Repository Information
- **Last Updated**: 2026-01-15
- **Repository**: https://github.com/gocortexio/spellbook

*Summaries generated with AI from repository documentation and commit history. Please review the source repositories' README files for full and comprehensive descriptions.*

## Recent Changes
- `7c5bb33` - Release v1.18.10 - Additional GitLab CI/CD support, new template example and check-init to confirm everything is well with the universe (2026-01-15)
- `27e682a` - Version 1.18.0 - GitLab CI/CD support, tagging improvements (2026-01-07)
- `4d90d84` - Release v1.17.5: Container permission fix and version command enhancement (2025-12-23)
- `fa6ca43` - Release v1.17.5: Container permission fix and version command enhancement (2025-12-23)
- `b4441e8` - Release v1.17.3: Should have been in 1.17.0 ! (2025-12-22)
- `9a3c9c1` - Version 1.17.1 - Bug fixes and documentation improvements (2025-12-22)
- `cca3ecf` - Update semgrep.yml (2025-12-21)
- `7de0a55` - Update SEMGREP_REPO_DISPLAY_NAME and add SARIF file (2025-12-21)
- `9df9bd5` - Refactor Semgrep workflow configuration (2025-12-21)
- `eaa69e2` - Add Semgrep workflow for code scanning (2025-12-21)

## Tags
![content-pack](https://img.shields.io/badge/content--pack-6f42c1?logo=npm&logoColor=white) ![cicd](https://img.shields.io/badge/cicd-28a745?logo=githubactions&logoColor=white)

---
*Auto-generated on 2026-01-19*
