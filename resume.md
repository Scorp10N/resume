# Yarin M

**Information Security Engineer | Security Architect**

yarin@scorp.solutions · [linkedin.com/in/cyberquantumcat](https://linkedin.com/in/cyberquantumcat) · [github.com/Scorp10N](https://github.com/Scorp10N)

---

## Executive Summary

Security Architect and Information Security Engineer with 20+ years spanning telco, enterprise IT, pharma, crypto, and Fortune 500 financial services. Designed and operated security programs at Mastercard Acquisition Security and TEVA Pharmaceuticals; built cloud-native SIEM and DevSecOps pipelines from scratch; now running an independent security consultancy focused on cloud-native architecture, threat modeling (MITRE ATT&CK, Zero Trust), and AI security. Known for building what others only advise.

---

## Professional Experience

**Security Consultant (Freelance), Scorp Solutions** — *Jul 2022 – Nov 2022 · Mar 2025 – Present*
Remote / Israel

- Provide cloud security consulting, security architecture reviews, and penetration testing for diverse clients.
- Deliver DevSecOps and CI/CD security assessments, compliance audits (GDPR, ISO 27001), and risk mitigation strategies.
- Apply AI security practices in client engagements: LLM threat modeling, secure agentic pipeline design, and Zero Trust integration patterns.

**Lead Information Security Engineer, Mastercard — Acquisition Security** — *November 2022 – February 2025* · Israel

- Led security integration for large-scale acquisition programs across AWS, GCP, and Azure, ensuring enterprise compliance.
- Conducted 100+ security reviews identifying 1,200+ risks; critical security incidents dropped 40% year-over-year. <!-- TODO AC-08: confirm 1,200+ risks and 40% YoY with exact time period -->
- Established threat intelligence and SOC-aligned risk triage processes for third-party software and custom integrations.
- Advised cross-functional stakeholders on incident response, MITRE ATT&CK-based threat modeling, and cloud-native security controls.

**Senior Security Engineer, Celsius Network** — *February 2022 – July 2022* · Israel
*(Celsius Network: crypto lending platform; filed Chapter 11 bankruptcy July 2022)*

- Designed and implemented a custom Cloud SIEM with CI/CD integration, reducing mean time to detect (MTTD) by 30% across 15+ cloud data sources. <!-- TODO AC-17: confirm MTTD % and source count -->
- Served as primary security consultant for development and integration projects; enforced secure SaaS integrations and Zero Trust access controls.

**Professional Services Integration Expert, Bynet Data Communications** — *January 2018 – January 2022* · Israel

- Led security integrations across AWS, GCP, Azure, and private cloud environments for enterprise clients.
- Mentored 15 junior engineers; cut average onboarding time from 12 to 4 weeks and team delivery throughput increased 3× in H2 2019. Awarded 'Outstanding Worker' (2019). <!-- TODO AC-07: confirm specifics or revert to original if unverifiable -->

**Global IT SecOps — Security Engineer, TEVA Pharmaceuticals (via Bynet OS)** — *January 2012 – January 2018* · Israel

- Designed HLD/LLD security architectures for major M&A integrations; supported 3 acquisition security programs. <!-- TODO AC-16: add outcome metric (audit result, environment count, incident rate) -->
- Managed multi-vendor security systems (Palo Alto, CheckPoint, CrowdStrike) across 10+ global environments.
- Established the organization's first security zone standards, forming the baseline for current Zero Trust segmentation policy.

**Security & Network Engineer / Solutions Expert, Bezeq International** — *January 2006 – January 2012* · Israel

- Delivered security and network solutions (firewalls, VPNs, DNS) for enterprise clients.
- Led site migrations, mentored team members, and achieved 20% faster incident resolution.

---

## Education

**Computer Science & Chemistry**
September 1997 – June 2000

---

---

## Projects

**SecOps Pipeline Platform** *(GitHub Actions, Trivy, TruffleHog, CodeQL, Semgrep, YAML)*
Centralized reusable GitHub Actions security platform enforcing DevSecOps governance across consuming repositories via GitOps sync.

- Built reusable CI/CD security workflows covering secrets scanning (TruffleHog), container image scanning (Trivy), SAST (CodeQL, Semgrep), and CODEOWNERS enforcement.
- Implemented supply chain security controls: signed commits, SLSA provenance, and pre-commit hook distribution at scale.

**cvetool** *(Go, Claircore, SQLite, SARIF)*
CVE scanner and vulnerability manager for filesystems, container images, and VMs with multi-format reporting.

- Built on Claircore; produces plain-text, SARIF, and Clair-format reports for integration into CI/CD pipelines and security dashboards.
- Supports local vulnerability database sync, enabling air-gapped scanning for regulated environments.

**env-pilot** *(Python, YAML, Zero-Secret Access architecture)*
Secure development environment orchestrator enforcing a zero-secret access model across human dotfiles, agent skills, and local stack components.

- Designed and implemented least-privilege sandbox controls preventing agents from accessing SSH keys, SOPS keys, and GPG material.
- Bridges dotfile management, agent rules, and local stack registry under a unified security policy.

**Security Posture Store** *(GitOps, GitHub Actions, SOPS, age, SARIF, Semgrep, Trivy, TruffleHog)*
GitOps-backed security state store aggregating automated scan findings and posture snapshots across the project portfolio.

- CI pipelines push findings from 7 scanners (Semgrep, Trivy, TruffleHog, govulncheck, pip-audit, npm-audit, SARIF) into version-controlled state on every push — zero human intervention.
- Daily posture snapshots roll up severity counts across tracked repositories, enabling trend tracking and drift detection over time.
- Secrets managed with SOPS + age using a TPM-backed hardware key; private key sealed in the TPM chip and never written to disk.

---

## Technical Skills

| Area | Technologies |
|---|---|
| **Cloud Security** | AWS, Azure, GCP, Office 365, Prisma Cloud, Aqua Security, Snyk |
| **SIEM & Monitoring** | Splunk, ELK Stack, LogRhythm, Grafana, Prometheus, Loki |
| **Firewalls & Network Security** | Palo Alto Networks, Fortigate, CheckPoint, Cisco, Radware, Tufin, Skybox |
| **Vulnerability Management** | Tenable, BridgeCrew, Wireshark, Burp Suite, CrowdStrike |
| **Automation & DevSecOps** | Terraform, Kubernetes, Docker, GitOps, Python, Bash, PowerShell, IaC |
| **Identity & Access Management** | OAuth, SSO, SAML, MFA, FIDO2, Kerberos, CyberArk, IAM |
| **Compliance & Frameworks** | GDPR, ISO 27001, NIST, SOC 2, MITRE ATT&CK, Zero Trust, Risk Assessment |
| **Threat Intelligence & SOC** | Threat intelligence, SOC operations, incident response, cloud-native detection, threat modeling |
| **Programming** | Python, Node.js, Golang, Java, TypeScript, PowerCLI |
| **Virtualization & Databases** | VMware, Hyper-V, Docker, Kubernetes, QEMU, PostgreSQL, MySQL, MongoDB, Elasticsearch |

## Currently Building

AI Security & Agentic Infrastructure: Secure self-hosted AI inference with OpenAI-compatible gateway and virtual key routing across providers; containerized MCP server fleet for agent tooling; zero-secret agent harness design using SOPS-encrypted secrets and RAM-backed tmpfs isolation; anti-detection headless browser automation for agentic security research; LLM threat modeling, agentic pipeline security (LangChain, LangGraph), Langfuse observability, LiteLLM, OpenTelemetry for AI
