# mocktaxii

## Summary

MockTAXII is a full-featured TAXII 2.x server specifically designed for Cortex XSIAM and XSOAR Threat Intelligence Management (TIM) integration testing and demonstrations. It implements the complete TAXII 2.1 and STIX 2.1 specifications, serving authentic threat intelligence indicators at enterprise scale with production-ready deployment options.

The tool solves a critical testing challenge for threat intelligence operations: validating TIM integrations requires realistic TAXII feeds, but production threat intelligence sources are expensive, rate-limited, or unavailable during development and testing. MockTAXII provides a fully functional TAXII server with authentic CISA KEV data, MITRE ATT&CK mappings, and custom STIX bundles that teams can use for integration testing, demonstrations, and training without dependency on external threat intelligence vendors.

Built with Python and Flask, MockTAXII serves over 1,388 CVE indicators with full CVSS scores, vectors, and CPE details. It supports API key-based targeting for custom STIX bundle delivery, includes supply chain attack simulation with malicious package indicators, and provides realistic threat intelligence campaigns and reports. The server implements complete TAXII 2.1 discovery endpoints, collections, and manifest APIs that mirror production TAXII servers.

MockTAXII is essential for security teams deploying XSIAM or XSOAR TIM capabilities. It enables thorough integration testing before connecting to production feeds, provides realistic demonstrations for stakeholder presentations, and serves as a training platform for analysts learning TAXII/STIX protocols. The tool's Docker deployment and configurable authentication make it suitable for both development environments and isolated training networks.

## Key Use Cases
- Testing XSIAM and XSOAR Threat Intelligence Management integrations
- Realistic threat intelligence demonstrations at enterprise scale
- Custom STIX bundle serving with API key targeting
- Supply chain attack simulation with malicious package indicators
- CISA KEV and MITRE ATT&CK framework integration

## Prerequisites & Palo Alto Tools

### Prerequisites
- Python 3.x environment
- Flask and STIX2 Python libraries
- Docker and Docker Compose (for containerized deployment)
- Network accessibility for TAXII clients (HTTPS recommended)
- Optional: SSL certificates for production-like HTTPS deployment

### Palo Alto Integration
- **Cortex XSIAM TIM** - TAXII 2.1/STIX 2.1
  - Tests threat intelligence feed integration via standard TAXII 2.1 protocol
  - Validates STIX 2.1 indicator ingestion and processing
  - Provides realistic feed data for correlation rule development
- **Cortex XSOAR TIM** - TAXII 2.1/STIX 2.1
  - Tests TIM feed configurations and indicator enrichment
  - Validates playbook automation with threat intelligence data
  - Demonstrates threat intelligence sharing capabilities

## Repository Information
- **Last Updated**: 2025-12-21
- **Repository**: https://github.com/gocortexio/mocktaxii

*Summaries generated with AI from repository documentation and commit history. Please review the source repositories' README files for full and comprehensive descriptions.*

## Recent Changes
- `51f60e9` - Refactor Semgrep workflow for improved clarity (2025-12-21)
- `665be08` - Remove test .env file (2025-11-29)
- `b98527d` - MockTAXII v0.7.0 - I can't believe they locked me up for driving on the sidewalk! (2025-11-29)
- `70bf17d` - Logo redesign, child of the 80s (2025-09-21)
- `af475a7` - Major campaign and report expansion with security updates v0.6.0 (2025-09-21)
- `ee7bb3b` - Update software to address security vulnerabilities and improve stability (2025-08-21)
- `76e32b3` - Minor README.md Update (2025-07-25)
- `16be7dd` - Added CVSS (score, version, vector) and CPE details to all 1,388 CVE entries... (2025-07-25)
- `c2779a3` - Adds CSRF token to login form, disables CSRF in Docker Compose for development... (2025-06-27)
- `9e25632` - Resolved uv.lock (2025-06-26)

## Tags
![threat-intel](https://img.shields.io/badge/threat--intel-6f42c1?logo=virustotal&logoColor=white) ![testing](https://img.shields.io/badge/testing-ff6b35?logo=pytest&logoColor=white)

---
*Auto-generated on 2026-01-19*
