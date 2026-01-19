# sigma2xsiam

## Summary

Sigma2XSIAM is a specialized pySigma backend that converts industry-standard Sigma detection rules into Cortex XSIAM XQL (eXtended Query Language) queries. It enables security teams to leverage the extensive Sigma rule repository for XSIAM deployments, automatically translating generic detection logic into platform-specific queries that work correctly with Cortex XDM data schemas.

The tool addresses a critical interoperability challenge: Sigma has become the universal standard for sharing detection rules across platforms, but each SIEM uses different query languages and data models. Sigma2XSIAM bridges this gap by providing accurate field mappings from generic Sigma field names to Cortex XDM schema fields, handling complex Sigma modifiers (contains, startswith, endswith), and generating clean, optimized XQL syntax that XSIAM's query engine processes efficiently.

Built as a Python package using the pySigma framework, Sigma2XSIAM includes comprehensive field mapping tables for Windows, Linux, network, cloud, and web logs. It handles challenging conversion scenarios like PowerShell command detection, complex boolean logic, and multi-condition rules. The tool supports both single-rule and batch conversion workflows, with output formatting designed for direct copy-paste into the XSIAM console.

Sigma2XSIAM is essential for security teams adopting XSIAM who want to leverage existing Sigma rule investments. Rather than manually rewriting hundreds of detection rules, teams can convert their Sigma rule libraries automatically, preserving detection logic while adapting to XSIAM's query syntax and data model. The tool accelerates XSIAM deployment by making the vast Sigma community rule repository immediately accessible.

## Key Use Cases
- Convert Sigma rules to XSIAM XQL query syntax
- Map generic Sigma fields to Cortex XDM schema
- Handle complex Sigma modifiers and PowerShell rules
- Batch conversion of multiple Sigma rules
- Generate clean, readable XQL output for XSIAM console

## Prerequisites & Palo Alto Tools

### Prerequisites
- Python 3.x environment
- pySigma library and framework
- Sigma rule files in YAML format
- Understanding of Sigma rule structure
- Access to Cortex XSIAM for testing converted queries

### Palo Alto Integration
- **Cortex XSIAM** - XQL query generation (pySigma backend)
  - Converts Sigma rules to functional XQL queries
  - Maps Sigma fields to Cortex XDM data model
  - Generates queries compatible with XSIAM query engine and correlation rules

## Repository Information
- **Last Updated**: 2025-10-09
- **Repository**: https://github.com/gocortexio/sigma2xsiam

*Summaries generated with AI from repository documentation and commit history. Please review the source repositories' README files for full and comprehensive descriptions.*

## Recent Changes
- `8564046` - Add new detection rules for emerging threats and exploits (2025-10-09)
- `cf783bf` - Add new detection rules for various malware and exploit attempts (2025-10-09)
- `8048b50` - Fix issue where output file directory is not created (2025-10-09)
- `248a034` - Update conversion summary statistics in the documentation (2025-10-09)
- `759f3c8` - Add ability to convert multiple Sigma rules from a directory (2025-10-09)
- `6710c66` - Add option to save converted queries to an output file (2025-10-09)
- `0b310fe` - Ensure all string values in queries are correctly quoted (2025-10-07)
- `7a3c1e8` - Add field mapping for cloud and web rules to fix conversion errors (2025-10-07)
- `b3dc13d` - Fix type errors in Sigma rule conversion and update reporting (2025-10-07)
- `19ec90d` - Add comprehensive testing for Sigma rule conversion to XSIAM (2025-10-07)

## Tags
![rule-conversion](https://img.shields.io/badge/rule--conversion-ff6b35?logo=convertio&logoColor=white) ![xql](https://img.shields.io/badge/xql-28a745?logo=paloaltonetworks&logoColor=white) ![sigma](https://img.shields.io/badge/sigma-28a745?logo=github&logoColor=white)

---
*Auto-generated on 2026-01-19*
