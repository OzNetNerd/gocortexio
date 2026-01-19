# gcgit

## Summary

GCGit is a Rust-based command-line tool that bridges Git version control with the Cortex XSIAM REST API, enabling security teams to manage XSIAM configurations using Git workflows. It provides CRUD operations for Correlation Rules, Dashboards, BIOCs, and Scripts, treating security content as code with full version history and collaboration capabilities.

The tool solves a critical operational challenge: managing Cortex XSIAM content through the web console lacks version control, change tracking, and collaboration features that development teams rely on for code. GCGit brings Git-based workflows to security operations, enabling teams to track who changed what, review changes before deployment, roll back problematic updates, and collaborate on detection logic using standard Git practices like branches, pull requests, and code review.

Built in Rust with embedded libgit2, GCGit requires zero external dependencies and works entirely through local Git repositories and the XSIAM REST API. The tool uses human-readable YAML formats for all XSIAM objects, making content easy to review, diff, and merge. Its module architecture supports both XSIAM and Cortex Cloud, with specialized pull strategies for different object types like Scripts (which use ScriptCode for content retrieval).

GCGit is essential for security teams practicing detection-as-code. It enables mature DevSecOps workflows where detection rules are peer-reviewed, tested in branches, and deployed through controlled Git workflows rather than ad-hoc console edits. The tool's local-first design means no CI/CD infrastructure is required—analysts can manage content directly from their workstations using familiar Git commands.

## Key Use Cases
- Version control for Cortex XSIAM configurations (Correlation Rules, Dashboards, BIOCs, Scripts)
- Local content management with Git-based workflow
- Multi-module support for Cortex XSIAM and Cortex Cloud
- YAML configuration with human-readable formats
- Zero-dependency deployment with embedded libgit2

## Prerequisites & Palo Alto Tools

### Prerequisites
- Git installed and configured locally
- Valid Cortex XSIAM or Cortex Cloud API credentials
- Network access to Cortex API endpoints
- Local file system for Git repository storage
- Rust toolchain (for building from source)

### Palo Alto Integration
- **Cortex XSIAM** - REST API
  - CRUD operations for Correlation Rules, Dashboards, BIOCs, Scripts
  - Version control and Git-based deployment workflows
  - ScriptCode retrieval for script content management
- **Cortex Cloud** - REST API
  - Configuration management through Git workflows
  - Multi-module architecture for different object types

## Repository Information
- **Last Updated**: 2025-12-21
- **Repository**: https://github.com/gocortexio/gcgit

*Summaries generated with AI from repository documentation and commit history. Please review the source repositories' README files for full and comprehensive descriptions.*

## Recent Changes
- `37316b8` - Refactor Semgrep workflow for improved clarity (2025-12-21)
- `b19f352` - v2.1.9: Implement ScriptCode pull strategy for XSIAM scripts (2025-11-03)
- `0932b79` - Release v2.1.8: Complete module architecture migration (2025-11-02)
- `c201db6` - Release v1.1.0 (2025-09-14)
- `b9fc32a` - Remove unused file (2025-08-24)
- `98c5345` - gcgit v1.0.2 release (2025-08-24)
- `dcd5fbd` - Removed random action (2025-08-11)
- `61a55bb` - Cortex CLI Code Scan (2025-08-11)
- `f54f4af` - Merged v1.0.0 (2025-07-26)

## Tags
![detection-as-code](https://img.shields.io/badge/detection--as--code-6f42c1?logo=git&logoColor=white) ![version-control](https://img.shields.io/badge/version--control-28a745?logo=git&logoColor=white)

---
*Auto-generated on 2026-01-19*
