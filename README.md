# Awesome-Developer-Secrets-Scanning

# Top Developer Secrets Scanning Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Credential Leak Detection, Git History Scanning & Secret Rotation Workflows*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Developer Secrets Scanning**. These tools detect leaked API keys, tokens, passwords, and private keys in source code, git history, CI pipelines, and cloud storage before attackers can exploit them.

**Examples** include GitGuardian, TruffleHog, GitHub Secret Scanning, Gitleaks, SpectralOps, Sentra, Checkmarx Secrets Detection, Cycode, Veracode, and GitLab Secret Detection (the category leaders).

**Open-source emphasis**: Secrets scanning is one of the strongest open-source security domains. **Gitleaks**, **TruffleHog**, **detect-secrets**, and **Kingfisher** power detection pipelines worldwide, with **TruffleHog** leading on validated-secret detection (89% recall, 96% precision) and **Gitleaks** remaining the default for fast, config-driven pre-commit scanning .

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[GitGuardian](https://www.gitguardian.com/)**  
  Leading commercial platform for real-time secrets detection and alerts, with 74% share of voice in AI recommendations . Scans private repositories and public GitHub commit streams in real time, offering incident management workflows, honeytokens, and integrations across CI/CD platforms and ticketing systems. Free tier for smaller teams .

- **[TruffleHog (Commercial)](https://trufflesecurity.com/)**  
  Enterprise version of the leading open-source scanner, adding live credential verification against provider APIs for 800+ secret types, auto-rotation for AWS/GCP, and policy/assignment workflows. Verifier coverage cuts false positives by confirming whether a flagged key actually works .

- **[GitHub Secret Scanning](https://docs.github.com/en/code-security/secret-scanning)**  
  Native GitHub integration with push protection (blocks secrets before they land) and post-commit scanning. GitHub Advanced Security scored highest on precision (75%) in an academic comparison, though recall was low (6%) without custom configuration .

- **[SpectralOps](https://spectralops.io/)**  
  AI-powered scanning for code, binaries, and configurations within DevOps pipelines. Offers Developer, Security, and Audit scanning modes with different precision/recall tradeoffs .

- **[Sentra](https://sentra.io/)**  
  DSPM platform that scans source code secrets across the **entire cloud estate** — not just Git repositories. Covers 600+ file extensions, .env files, cryptographic keys, IaC, and documentation where secrets routinely leak outside version control .

- **[Checkmarx Secrets Detection](https://checkmarx.com/)**  
  Secrets detection integrated into Checkmarx's broader AppSec platform, covering code, IaC, and CI/CD pipelines.

- **[Cycode](https://cycode.com/)**  
  SDLC-wide platform scanning secrets beyond code into docs, wikis, build logs, ticketing systems, and messaging tools. Uses Context Intelligence Graph to correlate findings and claims 94% false-positive reduction. Gartner Leader in Software Supply Chain Security 2026 .

- **[Veracode](https://www.veracode.com/)**  
  Enterprise AppSec platform with secrets detection integrated into its scanning suite.

- **[GitLab Secret Detection](https://docs.gitlab.com/ee/user/application_security/secret_detection/)**  
  Native GitLab CI job powered by Gitleaks, scanning diffs and optionally full history. Reports to the MR Security widget and standard gl-secret-detection-report.json artifact .

## Open-Source GitHub Projects

- **[Gitleaks](https://github.com/gitleaks/gitleaks)**  
  The default open-source git secrets scanner: free, fast, actively maintained, single binary, MIT licensed. Scans full git history with transparent TOML rule configuration (180+ default rules) . Scored 81% recall and 87% precision in a 2026 field test . **No built-in validity checking** — a match means "looks like a secret," not "is live" . Best for pre-commit hooks and CI where speed matters .

- **[TruffleHog](https://github.com/trufflesecurity/trufflehog)**  
  The most capable open-source scanner, AGPL-3.0 licensed. v3 rewrite in Go delivered major performance and detection quality gains . Roughly 1,200 detectors covering AWS, GCP, Snowflake, Stripe, Anthropic, OpenAI, and the long tail of vendor-specific tokens . Scans git repos, filesystems, S3, GCS, Docker, CircleCI, Hugging Face, and more . **The open-source version lacks the live credential verification** that makes the commercial tier most useful .

- **[detect-secrets (Yelp)](https://github.com/Yelp/detect-secrets)**  
  Enterprise-friendly secret detection with a plugin architecture for custom detectors and baseline management. Wraps well into GitHub Actions and CI pipelines . Python-based, actively maintained.

- **[Kingfisher](https://github.com/mongodb/kingfisher)**  
  Broad-source scanner from MongoDB covering git history, local files, GitHub, GitLab, Azure Repos, Bitbucket, Gitea, Hugging Face, Jira, Confluence, Slack, Teams, Postman, Docker, S3, GCS, compressed files, SQLite databases, and Python bytecode . **The widest source coverage of any open-source scanner** .

- **[Whispers (Skyscanner)](https://github.com/Skyscanner/whispers)**  
  Apache-2.0 licensed scanner identifying hardcoded secrets in static structured text, source code, and configuration files. 476 stars. Last release signal 2021 — **stable but not actively feature-developed** .

- **[Talisman](https://github.com/thoughtworks/talisman)**  
  Pre-commit hook from Thoughtworks that scans for secrets and other sensitive data before they leave the developer machine.

- **[git-secrets (AWS Labs)](https://github.com/awslabs/git-secrets)**  
  AWS Labs tool preventing secrets from being committed by scanning commits, commit messages, and git history against configurable patterns. Last update September 2025 .

- **[gitleaks-action](https://github.com/gitleaks/gitleaks-action)**  
  Official GitHub Action wrapping Gitleaks for repository scanning in workflows, with SARIF output for GitHub Code Scanning .

- **[tartufo (GoDaddy)](https://github.com/godaddy/tartufo)**  
  GoDaddy's fork of TruffleHog, digging deep into commit history for high-entropy strings. 381 stars, more actively maintained than many TruffleHog forks .

- **[Git-all-secrets](https://github.com/anshumanbh/git-all-secrets)**  
  Tool that clones and scans all repositories within an organization or user account for secrets across GitHub, Gist, GitLab, and BitBucket .

### Additional Strong Open-Source Options

- **ggshield (GitGuardian CLI)** — Free CLI that uses GitGuardian's public API to scan files, repositories, Docker images, PyPI packages, AI coding assistants, CI/CD pipelines, and git hooks .
- **earlybird (American Express)** — Scans local files, directories, remote git repos, git history, staged files, tracked files, and streamed input .
- **Credential Digger (SAP)** — Scans git repositories, pull requests, wiki pages, local files/folders, and GitHub organizations .
- **Trivy** — Primarily a vulnerability scanner that also detects secrets in container images, filesystems, git repos, VM images, and Kubernetes .
- **Checkov** — IaC scanner that detects secrets in infrastructure-as-code files, CI/CD pipelines, container images, and open-source packages .
- **SecretScanner (ThreatMapper)** — Scans container images and filesystems for secrets .
- **shhgit** — Scans GitHub, Gist, GitLab, BitBucket, and local directories for secrets in real time .
- **Git-hound** — Scans GitHub repositories, Gists, and git history for secrets with regex patterns .

**Frameworks for building custom secrets scanning pipelines**: Layer **Gitleaks** for pre-commit and fast CI scanning (MIT, single binary, TOML rules) with **TruffleHog** for validated-secret detection in CI and historical scans (1,200+ detectors, broad source coverage) . Add **detect-secrets** for baseline management and custom plugin detectors. Deploy **Kingfisher** when you need to scan beyond git into Jira, Slack, Confluence, Hugging Face, and Postman . For full program maturity, pair open-source detection with a commercial workflow layer (GitGuardian, TruffleHog Enterprise) for rotation playbooks, honeytokens, and org-wide incident management . **No single tool achieves both high precision and high recall** — use at least two layered scanners .

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Secrets scanning tools must be used only against systems you own or are explicitly authorized to test. Scanning public repositories for secrets is generally permitted, but accessing or exploiting found credentials is illegal.
- Self-hosted open-source solutions require proper infrastructure, rule tuning, and ongoing maintenance. High false-positive rates are common — every flagged finding requires human validation before rotation or incident response .
- The open-source ecosystem provides strong detection engines and broad source coverage, but enterprise workflow features (incident management, rotation automation, honeytokens, org-wide dashboards) remain primarily commercial offerings .

---

**Made for security engineers, DevSecOps teams, platform engineers, and application security professionals.**  
Let's make secrets scanning more open, transparent, and effective.
