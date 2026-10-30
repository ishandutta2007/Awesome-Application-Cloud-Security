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

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The Application Security market is estimated at ~$12.6B–$15.9B in 2026, while the broader Cloud Security sector is projected at ~$46.1B–$60.3B. The market remains **moderately fragmented**—populated by numerous niche point tools across SAST, SCA, and posture management—but is rapidly consolidating into unified platforms (CNAPP & ASPM) led by tech giants and top cybersecurity platforms.

## SaaS/Hosted Platforms

| Company / Product | Category & Description | Scale (Revenue / Valuation) | Pricing (Starting Tier) | Free Tier / Trial Limits | Best For |
|---|---|---|---|---|---|
| **[GitHub Advanced Security](https://github.com/features/security)** | Native code security (CodeQL SAST, secret scanning, dependency review) | ~$3.1T parent (Microsoft) / ~$4B+ ARR | $19/committer/mo (Secret Protection) or $30/committer/mo (Code Security); $49/committer/mo full suite (annual contract, req. Team/Enterprise) | **Permanently Free** for public open-source repositories; 30-day trial with GitHub Enterprise Cloud | GitHub-centric teams wanting integrated scanning without third-party agents |
| **[Prisma Cloud](https://www.paloaltonetworks.com/prisma/cloud)** | Comprehensive CNAPP (CSPM, CWPP, code security, runtime defense) | ~$115B+ market cap (Palo Alto Networks) / ~$4.2B+ ARR (NGS) | Starts at ~$18,000/year (CSPM entry pool) or ~$45,000/year (Full CNAPP suite) via credit licensing | **15-day free trial** (via AWS Marketplace PAYG) or sales-coordinated enterprise POC | Enterprises requiring end-to-end cloud protection from code to runtime |
| **[Datadog AppSec](https://www.datadoghq.com/)** | Application Security Management (ASM) & API protection in observability platform | ~$40B+ market cap (Datadog) / ~$2.6B+ ARR | $31 per host / month (billed annually, requires Datadog APM/Infrastructure) | **14-day free trial** with full access to App & API Protection and unified telemetry | Datadog observability users seeking unified telemetry and application runtime threat defense |
| **[Atlassian Security](https://www.atlassian.com/security)** (Atlassian Guard) | Centralized identity, access management, and threat detection across Jira, Confluence & Bitbucket | ~$35B–$40B market cap (Atlassian) / ~$4.4B+ ARR | $4.00–$4.35/user/mo (Guard Standard) or $8.00–$8.55/user/mo (Guard Premium); included in Cloud Enterprise | **30-day free trial** for Guard Standard/Premium; test policies configurable for up to 5 pilot users | Atlassian-centric organizations managing user governance and data loss prevention |
| **[Wiz](https://www.wiz.io/)** | Agentless cloud security platform & ASPM with unified security graph | $12B valuation (Series E) / ~$500M+ ARR | Starts at ~$24,000/year for 100 workloads (Wiz Essential) or ~$38,000/year (Wiz Advanced) | **No public automated free tier**; sales-led Proof of Value (POV) evaluation scoped for 14–30 days | Large multi-cloud enterprises needing agentless discovery with cross-stack risk correlation |
| **[Snyk](https://snyk.io/)** | Developer-first security platform (SCA, SAST, containers, IaC) | $7.4B valuation / ~$250M+ ARR | $25 per contributing developer / month (Team plan, max 10 devs); custom quote for Enterprise | **Permanently Free**: max 5 projects, 100 SAST tests/mo, 200 SCA tests/mo, 100 container tests/mo, 300 IaC tests/mo | Developer teams looking to embed automated security testing into IDEs and CI/CD pipelines |
| **[Veracode](https://www.veracode.com/)** | Enterprise application security testing platform (SAST, DAST, SCA) | $2.5B valuation (TA Associates / Thoma Bravo) / ~$300M+ revenue | Starts at ~$10,000–$15,000/year (SAST base tier) to ~$20,000+/year (DAST); bundled suites from $50k+/year | **No public permanent free tier**; targeted 14-day trials for select modules (e.g., Dynamic Analysis / Labs) and sales POCs | Enterprises with stringent compliance needs wanting mature, enterprise-wide AppSec programs |
| **[Checkmarx](https://checkmarx.com/)** | Application security testing platform (SAST, SCA, DAST, API Security) | $1.15B valuation (Hellman & Friedman) / ~$150M–$200M revenue | Starts at ~$30,000/year minimum via AWS Marketplace / private offers; mid-market ~$50k–$200k/year | **No public permanent free tier**; 30-day trials for developer IDE extensions & sales-coordinated custom POCs | Organizations seeking deep AST analysis and strong enterprise developer tool integration |
| **[Aqua Security](https://www.aquasec.com/)** | Cloud-native security platform (container security, runtime defense, CSPM) | $1B+ valuation (Series E unicorn) / ~$90M ARR | Enterprise tiers start at ~$10,000–$25,000/year depending on protected workload/cluster count | **Permanently Free open-source scanner (Trivy)**; commercial platform available via 14–30 day sales POC | Organizations with heavy container, Kubernetes, and cloud-native runtime security priorities |
| **[Mend.io](https://www.mend.io/)** | Application security and open-source vulnerability/license governance | ~$500M+ valuation / ~$70M+ ARR | Starts at ~$1,000/developer/year (core modules); enterprise agreements average ~$60,000/year | **Permanently Free (Mend Bolt)**: up to 5 scans per repository/day on unlimited public & private repositories | Security teams prioritizing open-source license compliance and automated dependency remediation |

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
