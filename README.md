# Awesome-Application-Cloud-Security

# Awesome-Application-Cloud-Security
**Top Application Cloud Security (Opensource) 🌟 Star if you like it! 🌟**

**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Application Security Posture Management (ASPM), Cloud Security Posture Management (CSPM), SAST, SCA & Container Security*
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Application & Cloud Security**. These tools enable security and development teams to discover vulnerabilities in code and cloud infrastructure, manage open-source risk, scan containers, and unify findings across the software development lifecycle—from fully managed enterprise platforms with AI-powered triage and unified risk correlation to self-hosted scanners and ASPM dashboards that give teams complete control over their security telemetry and remediation workflows.

**Examples** include Wiz, Snyk, Prisma Cloud, GitHub Advanced Security, Veracode, Checkmarx, Aqua Security, Mend.io, Datadog AppSec, and Atlassian Security (the category leaders in commercial space).

**Open-source emphasis**: This section is expanded with every relevant project for self-hosted application security, cloud posture, and open security infrastructure. **Critical note**: The open-source AppSec landscape is fragmented by category—**Foxnode ASPM** is the most complete open-source ASPM dashboard, **CloudRec** and **OpenShield** address cloud posture, **Semgrep** and **CodeQL** dominate SAST, and **TRUSCA** handles SCA with SBOM. No single open-source project matches Wiz's unified graph or Snyk's developer-first platform breadth.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Wiz](https://www.wiz.io/)**
  **Cloud security platform** with a unified security graph correlating cloud infrastructure, workloads, and code. **Pricing**: Quote-only; enterprise contracts. **Free tier**: None. **Best for**: enterprises wanting agentless cloud discovery with risk correlation across the full stack.

- **[Snyk](https://snyk.io/)**
  **Developer-first security platform** covering SCA, SAST, containers, and IaC. **Pricing**: Free tier for open source; paid plans per developer. **Free tier**: Yes, limited tests. **Best for**: development teams wanting to embed security into IDEs and CI/CD with minimal friction.

- **[Prisma Cloud](https://www.paloaltonetworks.com/prisma/cloud)** (Palo Alto Networks)
  **Cloud native application protection platform (CNAPP)** with CSPM, CWPP, and code security. **Pricing**: Quote-only. **Free tier**: None. **Best for**: enterprises wanting comprehensive cloud security from code to runtime.

- **[GitHub Advanced Security](https://github.com/features/security)**
  **Native security for GitHub** with CodeQL, secret scanning, and dependency review. **Pricing**: Per-committer for private repos; free for public. **Free tier**: CodeQL free for public repos. **Best for**: GitHub-centric teams wanting integrated code scanning without third-party tools.

- **[Veracode](https://www.veracode.com/)**
  **Application security testing** platform with SAST, DAST, and SCA. **Pricing**: Quote-only. **Free tier**: None. **Best for**: enterprises wanting a mature, compliance-oriented AppSec suite.

- **[Checkmarx](https://checkmarx.com/)**
  **Application security platform** with SAST, SCA, and API security. **Pricing**: Quote-only. **Free tier**: None. **Best for**: organizations wanting deep code analysis with strong enterprise integrations.

- **[Aqua Security](https://www.aquasec.com/)**
  **Cloud native security** with container scanning, runtime protection, and CSPM. **Pricing**: Quote-only. **Free tier**: Limited. **Best for**: teams prioritizing container and Kubernetes security.

- **[Mend.io](https://www.mend.io/)** (formerly WhiteSource)
  **SCA and application security** platform with automated remediation. **Pricing**: Quote-only. **Free tier**: Limited for open source. **Best for**: organizations needing deep open-source license and vulnerability management.

- **[Datadog AppSec](https://www.datadoghq.com/)**
  **Application security** integrated into Datadog's observability platform. **Pricing**: Quote-only; bundled with Datadog. **Free tier**: None for AppSec. **Best for**: Datadog customers wanting security findings alongside observability data.

- **[Atlassian Security](https://www.atlassian.com/security)**
  **Security capabilities** across Atlassian Cloud products. **Pricing**: Included with Atlassian subscriptions; advanced features quote-based. **Free tier**: Limited. **Best for**: Atlassian-centric organizations wanting security visibility across Jira, Confluence, and Bitbucket.

## Open-Source GitHub Projects

- **[Foxnode ASPM](https://github.com/valinorintelligence/foxnode-aspm)**
  **Open-source Application Security Posture Management platform** — **the most complete open-source ASPM dashboard** found in this research, with a modern dark UI and 16+ security tool parsers . **Features**: **AI Finding Triage** with false positive detection, auto-grouping, and contextual scoring; **Security Scorecard** (A–F) per product with trend tracking; **Compliance Mapping** to OWASP Top 10, PCI-DSS, SOC 2, CIS Benchmarks, and ISO 27001; SLA Tracker and risk heatmap; **Attack Path Analysis** visualizing exploitable chains with blast radius; **LLM/AI Security Scanner** detecting prompt injection and data poisoning mapped to OWASP LLM Top 10; **SBOM & supply chain** tracking; **AI Remediation Copilot**; Jira and Slack integrations; RBAC with four roles . **Supported scanners**: Semgrep, SonarQube, Bandit (SAST); OWASP ZAP, Nuclei (DAST); Trivy, Snyk, OWASP Dependency-Check (SCA); Prowler (cloud); Checkov, tfsec (IaC); Gitleaks, TruffleHog (secrets); SARIF universal . **Tech stack**: Python (FastAPI), React, PostgreSQL, Redis. **Deploy**: Docker Compose (one command) . **Trade-off**: **Aggregation and triage platform, not a scanner**—it does not perform scanning itself; you must run and feed results from the supported scanners. AI features require configuration. Newer project with growing but limited community validation compared to individual scanners. **Best for**: security teams wanting a centralized ASPM dashboard to aggregate findings from multiple open-source scanners, with AI-assisted triage and compliance mapping—without commercial ASPM pricing.

- **[CloudRec](https://github.com/antgroup/CloudRec)**
  **Multi-cloud security posture management (CSPM) platform** (Apache 2.0) — **the most mature open-source CSPM with full server deployment and CloudRec Lite** . **Features**: **Resource discovery** across 30+ cloud services and 200+ resource types on Alibaba Cloud, AWS, GCP; **OPA-based policy engine** for declarative rules without hardcoding; risk detection covering network protection, identity security, data protection, and log auditing; **CloudRec Lite** single-binary CLI for local-first quick posture checks without server stack . **Tech stack**: Java (backend), Docker. **Deploy**: Full server via Docker Compose; Lite via CLI binary . **Trade-off**: **Alibaba Cloud origin**—strongest support for Alibaba Cloud, with AWS/GCP support present but less mature. Full server deployment requires MySQL and multi-user operational overhead. Lite is newer and focused on quick checks. **Best for**: organizations running multi-cloud (especially Alibaba Cloud/AWS) wanting a self-hosted CSPM with OPA policy flexibility—or CloudRec Lite for lightweight local posture checks.

- **[OpenShield](https://github.com/OWASP/openshield)**
  **OWASP open-source CSPM for Azure** — **the most focused open-source CSPM for Microsoft Azure**, with remediation playbooks . **Features**: Azure misconfiguration scanning; **quantum-unsafe cryptography detection**; compliance mapping to CIS, NIST, ISO 27001, SOC 2; **remediation via Azure CLI playbooks**; React security dashboard; REST API; Microsoft Sentinel integration with KQL rules . **Tech stack**: Python (Flask), React, PostgreSQL, Azure SDK. **Deploy**: Docker or manual (requires Azure credentials and JWT_SECRET for production) . **Trade-off**: **Azure-only**—no AWS or GCP support. Requires Azure subscription credentials with appropriate permissions. Newer OWASP project with active development but limited production validation. **Best for**: Azure-centric organizations wanting an OWASP-backed, self-hosted CSPM with one-command remediation and Sentinel integration.

- **[TRUSCA](https://github.com/trustedoss/trusca)**
  **Self-hosted SCA portal with SBOM management and license compliance** (Apache 2.0) — **the most complete open-source SCA platform with a web UI and approval workflows** . **Features**: Component detection across **30+ language ecosystems** (based on cdxgen); vulnerability detection from Trivy's unified database (NVD, OSV, GitHub Advisory, EPSS, KEV) with **seven-state VEX triage** and EPSS-based prioritization; **license classification** (allowed/conditional/forbidden) with obligation tracking and automatic NOTICE generation; **SBOM export** (CycloneDX JSON/XML, SPDX JSON/Tag-Value) and ingestion; component approval workflow (pending/review/approved/rejected); audit log and RBAC; GitHub Action, GitLab CI, and Jenkins examples . **Tech stack**: Per repository. **Deploy**: Docker Compose (dev and production with Traefik/Let's Encrypt) or Kubernetes Helm . **Trade-off**: **SCA-focused**—it does not scan code for SAST issues or cloud infrastructure. Requires feeding SBOMs or connecting to repositories for scanning. **Best for**: organizations wanting a self-hosted SCA portal with SBOM management, license compliance, and approval workflows—replacing commercial SCA tools for open-source governance.

- **[Semgrep](https://github.com/semgrep/semgrep)**
  **Lightweight, fast SAST tool** (LGPL-2.1) — **the most widely adopted open-source SAST tool** for modern AppSec teams . **Features**: YAML-based rules that mirror code patterns for easy custom rule writing; community rule registry covering OWASP Top 10 across Python, JavaScript, Go, Java, and more; runs locally with `pip install semgrep` and `semgrep --config=auto ./src` . **Tech stack**: OCaml, Python. **Deploy**: CLI, CI/CD, or Semgrep Cloud (commercial). **Trade-off**: **SAST only**—no SCA, cloud posture, or container scanning. Commercial Semgrep adds advanced features like cross-file analysis and AI triage. **Best for**: development teams wanting fast, customizable SAST that fits into any CI pipeline with minimal configuration.

- **[CodeQL](https://github.com/github/codeql)**
  **Semantic code analysis engine** (MIT for queries; free for public repos) — **the most powerful open-source SAST for deep data-flow analysis**, powering GitHub Advanced Security . **Features**: Treats code as a database queried with QL; models data flow and taint tracking across functions; free for public repos and open-source projects; private repos require GitHub Advanced Security . **Tech stack**: QL, C++, C#. **Deploy**: GitHub Actions (native), CLI. **Trade-off**: **Free only for public repos**—private repository use requires GitHub Advanced Security licensing. Steeper learning curve for custom queries compared to Semgrep. **Best for**: open-source projects and GitHub organizations already on Advanced Security wanting deep semantic analysis.

- **[Ansede Static](https://pypi.org/project/ansede-static/)**
  **Open-source SAST with CWE-639 IDOR detection** (PyPI) — **the most specialized open-source SAST for authorization flaws**, claiming 100% CVE recall on a benchmark of 164 vulnerabilities . **Features**: **CWE-639 IDOR detection** (world-first according to project); missing auth (CWE-862); ownership bypass; SQLi, XSS, SSRF, path traversal, command injection; **route-aware analysis** mapping HTTP routes → auth guards → data sinks; framework profiles (Django, Flask, Express, Spring, ASP.NET, Gin); incident clustering (~49% noise reduction); confidence scoring; fully offline . **Tech stack**: Python (pip install). **Deploy**: CLI (`ansede-static src/`). **Trade-off**: **5 languages deep** (Python, JS/TS, Go, Java, C#) vs. Semgrep's 30+ shallow. Claims are self-reported—independent validation is limited. **Best for**: teams wanting SAST that catches authorization flaws (IDOR, missing auth) that Semgrep and CodeQL miss—especially for web applications.

- **[Scanr CLI](https://www.npmjs.com/package/@openlabs/scanr_cli)**
  **Open-source SCA and dependency vulnerability scanner** (npm) — **the most developer-friendly open-source SCA CLI** for Node.js, Python, and Rust . **Features**: Dependency scanning across `package-lock.json`, `requirements.txt`, `pyproject.toml`, `Cargo.lock`; CVE/OSV vulnerability lookup with severity and remediation hints; **CI policy checks** (`scanr.toml`) with deterministic exit codes; license compliance policy; baseline security debt tracking; CycloneDX SBOM generation and diff; JSON and SARIF output . **Tech stack**: Node.js. **Deploy**: `npm install -g @openlabs/scanr_cli` . **Trade-off**: **3 ecosystems only**—not as broad as TRUSCA or commercial SCA. CLI-only, no web UI or approval workflows. **Best for**: developers and small teams wanting fast, scriptable SCA with SBOM generation and policy gates in CI—without a platform.

### Additional Strong Open-Source Options

- **DockerDNA** — Dockerfile and docker-compose security scanner (PyPI) with CIS Benchmark mapping, secrets detection (regex + Shannon entropy), SBOM, and AI remediation . **Note**: Container configuration scanning, not application code or cloud posture. **Best for**: teams wanting focused Dockerfile/compose hardening.
- **docker-security (dsecrat)** — Unified container security tool in Go (18 modules: SBOM, vuln scanning, secrets, CIS/NIST compliance, admission control, eBPF runtime) . **Note**: Container lifecycle security, not AppSec or CSPM. **Best for**: platform teams wanting a single-binary container security tool.
- **Magpie** — Cloud Security Posture Manager (Java, Apache 2.0, ~188 stars) focused on modern cloud threats including ransomware and supply chain . **Note**: Smaller community than CloudRec; last push ~10 months ago per metadata. **Best for**: teams wanting a lightweight CSPM alternative to evaluate.

**Frameworks for building custom systems**: Combine **Foxnode ASPM** as the aggregation and triage dashboard with **Semgrep** or **CodeQL** for SAST, **TRUSCA** or **Scanr** for SCA, **CloudRec** or **OpenShield** for cloud posture, and **DockerDNA** for container scanning—creating a complete open-source AppSec stack. **None of these match Wiz's unified graph or Snyk's developer-first platform breadth**, but Foxnode ASPM provides the orchestration layer that most open-source stacks lack.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Application and cloud security platforms handling vulnerability data and infrastructure credentials must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate access controls for security findings.
- **The "unified platform" vs. "ASPM aggregation" vs. "individual scanner" distinction is critical.** **Wiz, Snyk, Prisma Cloud, and GitHub Advanced Security** are **unified platforms**—they scan, aggregate, and correlate across code, cloud, and runtime. **Foxnode ASPM** is an **ASPM aggregation layer**—it unifies findings from 16+ scanners but does not scan itself . **Semgrep, CodeQL, Ansede, and Scanr** are **individual scanners**—they find issues but do not aggregate or triage across categories. **CloudRec and OpenShield** are **cloud posture scanners**—they focus on infrastructure, not application code. **Choose based on whether you need a platform, an aggregation layer, or specific scanning capabilities.**
- **Foxnode ASPM is the most complete open-source ASPM dashboard** in this list, with AI triage, compliance mapping, attack path analysis, and 16 scanner parsers . **The trade-off**: it requires you to run and feed results from the supported scanners—it does not scan on its own. For teams wanting a Wiz-like aggregation experience without commercial pricing, it is the closest open-source option.
- **CloudRec is the most mature open-source CSPM** with full server deployment and the newer CloudRec Lite for local-first checks . **OpenShield is the best Azure-specific option** with OWASP backing and remediation playbooks . **Choose CloudRec for multi-cloud (especially Alibaba/AWS); choose OpenShield for Azure-centric organizations.**
- **TRUSCA is the most complete open-source SCA platform** with SBOM management, license compliance, and approval workflows . **Scanr** is the lightweight CLI alternative for developers wanting fast SCA without a platform .
- **Semgrep is the pragmatic default for open-source SAST**—fast, customizable, and broad language support . **CodeQL is more powerful but gated** for private repos. **Ansede claims to catch authorization flaws that both miss**—but its claims are self-reported and language coverage is narrower . **Combine Semgrep with Ansede for coverage of both injection and authorization bugs.**
- **Pricing opacity is universal across commercial vendors.** Wiz, Snyk (enterprise), Prisma Cloud, Veracode, Checkmarx, Aqua, Mend, Datadog AppSec, and Atlassian (advanced) require sales contact. GitHub Advanced Security publishes per-committer pricing. **Validate with direct vendor conversations against your repository count and cloud footprint.**
- Self-hosted open-source solutions require proper setup, API credentials for cloud scanning, scanner execution orchestration, and ongoing maintenance. **Security findings contain sensitive vulnerability data**—ensure your deployment meets your organization's security standards before scanning production code or cloud environments.

---

**Made for security engineers, AppSec teams, and organizations building transparent application and cloud security solutions.**
Let's make Application & Cloud Security more open, data-driven, and developer-friendly.
