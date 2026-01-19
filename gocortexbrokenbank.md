# gocortexbrokenbank

## Summary

GoCortex Broken Bank is an intentionally vulnerable Python web application specifically designed for Palo Alto Networks Cortex Platform training and security testing. It implements a realistic banking application with deliberately embedded vulnerabilities that mirror real-world security flaws, providing a safe environment for testing security tools, training analysts, and validating detection capabilities.

The tool addresses a critical need in security operations: training and testing require realistic vulnerable applications, but using production systems or generic training apps doesn't demonstrate platform-specific capabilities. Broken Bank is purpose-built for Cortex Cloud, XSIAM, and XDR, with log shipping, security scanning integration, and CI/CD pipeline examples that showcase how these platforms detect and respond to application security threats.

Built with Python and Flask, the application includes SQL injection, cross-site scripting (XSS), insecure authentication, and other OWASP Top 10 vulnerabilities. It ships comprehensive application logs to Cortex XSIAM for detection rule testing, integrates with Cortex Cloud for application security policy validation, and provides Kubernetes deployment configurations for infrastructure-as-code security testing scenarios.

Broken Bank serves as both a training platform and a CI/CD security validation tool. Security teams can use it to demonstrate how Cortex platforms identify vulnerabilities through static analysis, dynamic testing, and runtime protection. The application's deliberate flaws make it ideal for penetration testing exercises, security awareness training, and validating that security controls are properly configured and functioning.

## Key Use Cases
- Cortex Cloud Application Security testing and validation
- CI/CD pipeline integration for DevSecOps workflows
- Security tool benchmarking (SAST/DAST)
- Educational training on application security vulnerabilities
- Penetration testing and exploit validation

## Prerequisites & Palo Alto Tools

### Prerequisites
- Python 3.11 or higher (with pre-built wheels for dependencies)
- Docker and Docker Compose (for containerized deployment)
- Kubernetes cluster (optional, for IaC security testing)
- Cortex XSIAM HTTP endpoint credentials (for log shipping)
- Network access to Cortex platforms for log ingestion

### Palo Alto Integration
- **Cortex Cloud** - Security scanning
  - Tests application security policies through SAST/DAST scanning
  - Validates vulnerability detection in CI/CD pipelines
- **Cortex XSIAM** - Log ingestion
  - Ships application logs via HTTP endpoint for detection rule testing
  - Demonstrates log-based threat detection capabilities
- **Cortex XDR** - Detection testing
  - Validates security control effectiveness in CI/CD workflows
  - Tests runtime application security monitoring

## Repository Information
- **Last Updated**: 2026-01-10
- **Repository**: https://github.com/gocortexio/gocortexbrokenbank

*Summaries generated with AI from repository documentation and commit history. Please review the source repositories' README files for full and comprehensive descriptions.*

## Recent Changes
- `f9d44b6` - v1.3.2 – Log shipping, IaC security testing, and Kubernetes deployment (2026-01-09)
- `6f84796` - Use secret for SEMGREP_REPO_DISPLAY_NAME (2025-12-21)
- `cc1a6b0` - Refactor Semgrep workflow for improved clarity (2025-12-21)
- `dc43ce8` - Add Semgrep workflow for code scanning (2025-12-21)
- `65a79c1` - Updated packages requiring Python 3.11 pre-built wheels: (2025-12-05)
- `46c2edf` - Updated packages requiring Python 3.11 pre-built wheels: (2025-12-05)
- `e09471f` - GoCortex Broken Bank is an intentionally vulnerable application designed specifically to support Palo Alto Networks Cortex Cloud + Palo Alto Networks Cortex XSIAM/XDR training... (2025-11-30)
- `3166fa1` - GoCortex Broken Bank is an intentionally vulnerable application designed specifically to support Palo Alto Networks Cortex Cloud + Palo Alto Networks Cortex XSIAM/XDR training... (2025-11-29)

## Tags
![appsec](https://img.shields.io/badge/appsec-6f42c1?logo=owasp&logoColor=white) ![training](https://img.shields.io/badge/training-ff6b35?logo=googlescholar&logoColor=white) ![cicd](https://img.shields.io/badge/cicd-28a745?logo=githubactions&logoColor=white)

---
*Auto-generated on 2026-01-19*
