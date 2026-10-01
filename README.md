# 🔑 Awesome Developer Secrets Scanning & Credential Leak Detection 🛡️

<p align="center">
  <img src="assets/banner.svg" alt="Awesome Developer Secrets Scanning Banner" width="100%">
</p>

<p align="center">
  <a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome"><img src="https://img.shields.io/badge/Awesome-%E2%9C%94-blueviolet?style=flat-square&logo=github" alt="Awesome"/></a><a href="https://discord.gg/jc4xtF58Ve"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a> <a href="https://github.com/ishandutta2007/Awesome-Developer-Secrets-Scanning/stargazers"><img src="https://img.shields.io/github/stars/ishandutta2007/Awesome-Developer-Secrets-Scanning?style=flat-square" alt="Stars"/></a> <a href="https://github.com/ishandutta2007/Awesome-Developer-Secrets-Scanning/network/members"><img src="https://img.shields.io/github/forks/ishandutta2007/Awesome-Developer-Secrets-Scanning?style=flat-square" alt="Forks"/></a> <a href="https://github.com/ishandutta2007/Awesome-Developer-Secrets-Scanning/blob/main/LICENSE"><img src="https://img.shields.io/github/license/ishandutta2007/Awesome-Developer-Secrets-Scanning?style=flat-square" alt="License"/></a> <a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow" /></a>
</p>

---

## 📌 Ecosystem Overview & SEO Meta Summary

Welcome to the definitive, community-curated list of **Developer Secrets Scanning** software, **Credential Leak Detection** engines, **Git History Scanners**, and **DevSecOps Security Workflows**. 

Secrets scanning tools actively prevent data breaches by inspecting source code, commit history, build logs, docker images, and cloud storage for exposed **API keys**, **OAuth tokens**, **AWS/GCP/Azure credentials**, **private SSH/PGP keys**, and **passwords** before malicious actors can exploit them.

---

## 📑 Table of Contents

- [☁️ SaaS / Hosted Security Platforms](#-saas--hosted-security-platforms)
- [🔓 Open-Source GitHub Repositories](#-open-source-github-repositories)
- [💡 Detection Engine Framework & Architecture Best Practices](#-detection-engine-framework--architecture-best-practices)
- [💖 Support & Sponsorship](#-support--sponsorship)
- [🤝 How to Contribute](#-how-to-contribute)
- [⚠️ Security & Legal Disclaimer](#%EF%B8%8F-security--legal-disclaimer)
- [📈 Star History](#-star-history)

---

## ☁️ SaaS / Hosted Security Platforms

📊 **Secrets Scanning Market Overview**: The global Application Security (AppSec) & Developer Secrets Scanning market size is estimated at **$3.8 Billion** (growing at ~22.5% CAGR). The sector is **moderately fragmented**: while cloud hyperscalers (GitHub/Microsoft, GitLab) hold strong native distribution (*winner-take-most* for developer workflow integration), specialized standalone security providers (GitGuardian, Truffle Security, Cycode, Checkmarx) thrive by providing multi-cloud coverage, validated credential verification, and governance workflows across non-git assets.

*The table below lists leading SaaS security platforms sorted by **Company Size / Valuation / Market Cap** (descending order):*

| 🏢 Platform / SaaS Product | 📝 Description & Core Features | 💰 Starting Tier Pricing | 🎁 Free Tier / Free Trial Limit | 📊 Company Size (Valuation / Market Cap) |
| --- | --- | --- | --- | --- |
| **[GitHub Secret Scanning](https://docs.github.com/en/code-security/secret-scanning)** 🐙 | Native GitHub integration featuring push protection (pre-commit blocking) and post-commit historical repository scanning. | $19 / active committer / month (Secret Protection standalone; $49/mo for full GHAS suite) | Free forever for all public repositories; 30-day free trial on GitHub Enterprise Cloud (up to 300 licenses) | **$3.1 Trillion** (Parent Microsoft Market Cap) |
| **[SpectralOps](https://spectralops.io/)** 🛡️ | AI-powered secret scanner for code, binaries, configuration files, and CI/CD DevOps pipelines by Check Point. | $12 / developer / month ($250 / month CloudGuard Code Security starter tier) | 30-day free trial via Check Point CloudGuard trial program | **$20.0 Billion** (Parent Check Point Market Cap) |
| **[GitLab Secret Detection](https://docs.gitlab.com/ee/user/application_security/secret_detection/)** 🦊 | Native GitLab CI scanning job powered by Gitleaks, inspecting diffs, MR security widgets, and historical git commits. | $29 / user / month (Premium plan; $99/user/month for Ultimate) | Free forever on Free tier (includes 400 CI/CD compute minutes/month); 30-day free trial of GitLab Ultimate | **$7.5 Billion** (Public Market Cap) |
| **[Veracode](https://www.veracode.com/)** 🔒 | Enterprise Application Security (AppSec) platform incorporating secret scanning across codebase and pipeline builds. | $400 / application / month ($4,800 / application / year entry license) | 14-day free trial for select modules (e.g., Security Labs / DAST) | **$2.5 Billion** (Private Equity Valuation) |
| **[Checkmarx Secrets Detection](https://checkmarx.com/)** 🎯 | Secrets detection integrated into the Checkmarx One AppSec platform, covering source code, IaC, and build pipelines. | $67 / developer / month ($800 / developer / year entry tier) | 14-day free trial on Checkmarx One via AWS Marketplace | **$2.5 Billion** (Private Equity Valuation) |
| **[Cycode](https://cycode.com/)** 🌐 | Complete SDLC security platform scanning code, docs, wikis, build logs, and messaging tools with Context Intelligence Graph. | $162.50 / developer / month ($1,950 / developer / year AWS Marketplace tier) | 14-day free trial upon request | **$350 Million** (Venture Valuation) |
| **[GitGuardian](https://www.gitguardian.com/)** ⚡ | Real-time secrets detection & incident management for private repos and public GitHub commit streams, honeytokens, and CI/CD integrations. | $18 / developer / month (Business plan, billed annually) | Free forever for up to 25 contributing developers (90-day active committers) | **$300 Million** (Venture Valuation, $25M ARR) |
| **[Sentra](https://sentra.io/)** ☁️ | Data Security Posture Management (DSPM) platform scanning secrets across cloud storage, IaC, .env files, and repositories. | $4,166 / month ($50,000 / year base enterprise DSPM package) | 30-day Proof of Value (POV) guided enterprise trial | **$200 Million** (Venture Valuation) |
| **[TruffleHog (Commercial)](https://trufflesecurity.com/)** 🐷 | Enterprise scanner with live credential verification for 800+ secret types, auto-rotation for AWS/GCP, and policy workflows. | $15 / developer / month ($300 / month base tier) | Open-source CLI is free forever (unlimited developers); 14-day Enterprise trial | **$75 Million** (Venture Valuation) |

---

## 🔓 Open-Source GitHub Repositories

Open-source credential scanning software powers security pipelines globally. Below is the curated list of top open-source scanners, sorted by **GitHub Star Count** (descending order). 

*Click on any star badge to visit the official stargazers page for that repository:*

1. **[aquasecurity/trivy](https://github.com/aquasecurity/trivy)** <a href="https://github.com/aquasecurity/trivy/stargazers"><img src="https://img.shields.io/github/stars/aquasecurity/trivy?style=social&color=white" alt="Trivy Stars"/></a>  
   Comprehensive vulnerability & secret scanner for container images, filesystems, git repositories, and Kubernetes configurations.

2. **[gitleaks/gitleaks](https://github.com/gitleaks/gitleaks)** <a href="https://github.com/gitleaks/gitleaks/stargazers"><img src="https://img.shields.io/github/stars/gitleaks/gitleaks?style=social&color=white" alt="Gitleaks Stars"/></a>  
   The industry-standard open-source git secret scanner: lightning fast single Go binary with transparent TOML rule engine and pre-commit hook integration.

3. **[trufflesecurity/trufflehog](https://github.com/trufflesecurity/trufflehog)** <a href="https://github.com/trufflesecurity/trufflehog/stargazers"><img src="https://img.shields.io/github/stars/trufflesecurity/trufflehog?style=social&color=white" alt="TruffleHog Stars"/></a>  
   Deep git history scanner supporting 800+ secret detectors across git repos, S3 buckets, Docker images, CircleCI, Hugging Face, and local filesystems.

4. **[awslabs/git-secrets](https://github.com/awslabs/git-secrets)** <a href="https://github.com/awslabs/git-secrets/stargazers"><img src="https://img.shields.io/github/stars/awslabs/git-secrets?style=social&color=white" alt="git-secrets Stars"/></a>  
   AWS Labs git hook tool preventing AWS access keys and secret tokens from landing in commit messages or repository history.

5. **[bridgecrewio/checkov](https://github.com/bridgecrewio/checkov)** <a href="https://github.com/bridgecrewio/checkov/stargazers"><img src="https://img.shields.io/github/stars/bridgecrewio/checkov?style=social&color=white" alt="Checkov Stars"/></a>  
   Infrastructure-as-Code (IaC) static analysis tool scanning Terraform, CloudFormation, Kubernetes, and CI/CD for security flaws and hardcoded secrets.

6. **[michenriksen/gitrob](https://github.com/michenriksen/gitrob)** <a href="https://github.com/michenriksen/gitrob/stargazers"><img src="https://img.shields.io/github/stars/michenriksen/gitrob?style=social&color=white" alt="Gitrob Stars"/></a>  
   Reconnaissance tool for GitHub organizations, helping security teams find sensitive files and leaked keys across public repositories.

7. **[Yelp/detect-secrets](https://github.com/Yelp/detect-secrets)** <a href="https://github.com/Yelp/detect-secrets/stargazers"><img src="https://img.shields.io/github/stars/Yelp/detect-secrets?style=social&color=white" alt="detect-secrets Stars"/></a>  
   Enterprise Python framework by Yelp designed for baseline management, custom detector plugins, and zero false-positive pre-commit workflows.

8. **[thoughtworks/talisman](https://github.com/thoughtworks/talisman)** <a href="https://github.com/thoughtworks/talisman/stargazers"><img src="https://img.shields.io/github/stars/thoughtworks/talisman?style=social&color=white" alt="Talisman Stars"/></a>  
   Thoughtworks tool installed as a pre-commit/pre-push hook that prevents secrets and proprietary credentials from leaving developer workstations.

9. **[eth007/shhgit](https://github.com/eth007/shhgit)** <a href="https://github.com/eth007/shhgit/stargazers"><img src="https://img.shields.io/github/stars/eth007/shhgit?style=social&color=white" alt="shhgit Stars"/></a>  
   Real-time monitoring engine scanning public GitHub commits, Gists, GitLab, and Bitbucket event streams for secrets as they are published.

10. **[GitGuardian/ggshield](https://github.com/GitGuardian/ggshield)** <a href="https://github.com/GitGuardian/ggshield/stargazers"><img src="https://img.shields.io/github/stars/GitGuardian/ggshield?style=social&color=white" alt="ggshield Stars"/></a>  
    GitGuardian CLI wrapper for scanning local commits, CI/CD pipelines, Docker containers, PyPI dependencies, and developer environment variables.

11. **[tillson/git-hound](https://github.com/tillson/git-hound)** <a href="https://github.com/tillson/git-hound/stargazers"><img src="https://img.shields.io/github/stars/tillson/git-hound?style=social&color=white" alt="Git-hound Stars"/></a>  
    Batch pattern scanner evaluating GitHub search results, Gists, and repository histories for high-entropy strings and API keys.

12. **[securing/DumpsterDiver](https://github.com/securing/DumpsterDiver)** <a href="https://github.com/securing/DumpsterDiver/stargazers"><img src="https://img.shields.io/github/stars/securing/DumpsterDiver?style=social&color=white" alt="DumpsterDiver Stars"/></a>  
    Dynamic tool analyzing file entropy, rules, and compressed archives to uncover hardcoded secrets hidden in binary data or source code.

13. **[mongodb/kingfisher](https://github.com/mongodb/kingfisher)** <a href="https://github.com/mongodb/kingfisher/stargazers"><img src="https://img.shields.io/github/stars/mongodb/kingfisher?style=social&color=white" alt="Kingfisher Stars"/></a>  
    Broadest-source scanner by MongoDB covering git history, Jira, Confluence, Slack, Teams, Postman collections, SQLite, Hugging Face, and S3.

14. **[deepfence/SecretScanner](https://github.com/deepfence/SecretScanner)** <a href="https://github.com/deepfence/SecretScanner/stargazers"><img src="https://img.shields.io/github/stars/deepfence/SecretScanner?style=social&color=white" alt="SecretScanner Stars"/></a>  
    Container image and filesystem secret scanner from Deepfence designed for cloud-native DevSecOps pipelines.

15. **[SAP/credential-digger](https://github.com/SAP/credential-digger)** <a href="https://github.com/SAP/credential-digger/stargazers"><img src="https://img.shields.io/github/stars/SAP/credential-digger?style=social&color=white" alt="Credential Digger Stars"/></a>  
    Machine-learning powered scanner by SAP that filters out false positives in git repositories and pull requests using custom trained models.

16. **[Skyscanner/whispers](https://github.com/Skyscanner/whispers)** <a href="https://github.com/Skyscanner/whispers/stargazers"><img src="https://img.shields.io/github/stars/Skyscanner/whispers?style=social&color=white" alt="Whispers Stars"/></a>  
    Static structured text scanner by Skyscanner targeting JSON, YAML, XML, properties files, and python source files for leaked credentials.

17. **[americanexpress/earlybird](https://github.com/americanexpress/earlybird)** <a href="https://github.com/americanexpress/earlybird/stargazers"><img src="https://img.shields.io/github/stars/americanexpress/earlybird?style=social&color=white" alt="earlybird Stars"/></a>  
    American Express secret scanning tool designed to inspect local files, remote git repositories, staged files, and live streaming input.

18. **[godaddy/tartufo](https://github.com/godaddy/tartufo)** <a href="https://github.com/godaddy/tartufo/stargazers"><img src="https://img.shields.io/github/stars/godaddy/tartufo?style=social&color=white" alt="tartufo Stars"/></a>  
    GoDaddy's enhanced Python scanner digging deep into git commit history for high-entropy strings and signatures.

19. **[anshumanbh/git-all-secrets](https://github.com/anshumanbh/git-all-secrets)** <a href="https://github.com/anshumanbh/git-all-secrets/stargazers"><img src="https://img.shields.io/github/stars/anshumanbh/git-all-secrets?style=social&color=white" alt="Git-all-secrets Stars"/></a>  
    Multi-provider scanner cloning and aggregating secret detection across all repositories within a GitHub, GitLab, or BitBucket organization.

20. **[gitleaks/gitleaks-action](https://github.com/gitleaks/gitleaks-action)** <a href="https://github.com/gitleaks/gitleaks-action/stargazers"><img src="https://img.shields.io/github/stars/gitleaks/gitleaks-action?style=social&color=white" alt="gitleaks-action Stars"/></a>  
    Official GitHub Action bringing Gitleaks scanning into workflows with direct SARIF upload to GitHub Code Scanning alerts.

---

## 💡 Detection Engine Framework & Architecture Best Practices

When architecting an enterprise secret scanning strategy:

1. **Pre-Commit Defense**: Deploy fast single-binary scanners like **Gitleaks** or **Talisman** as pre-commit hooks to block secrets before commits hit remote repositories.
2. **CI/CD Pipeline Guardrails**: Integrate scanners in GitHub Actions, GitLab CI, or CircleCI for mandatory pull-request checks.
3. **Live Credential Verification**: Use engines with active API validation (such as **TruffleHog**) to verify whether detected keys are live, active, or inactive, cutting false-positive noise by up to 90%.
4. **Broad Asset Coverage**: Extend scanning beyond git repositories into cloud storage (S3/GCS), Jira tickets, Slack channels, and Postman collections with multi-source tools like **Kingfisher** or **Sentra**.

---

## 💖 Support & Sponsorship

Thank you for visiting and supporting **Awesome Developer Secrets Scanning**! 🛡️

If you find this curated security resource helpful for your team, company, or personal DevSecOps workflow, please consider supporting the project:

- 🌟 **Star this repository** on GitHub to help other security engineers find it.
- 🍴 **Fork the repo** to keep a copy and contribute new scanners or updates.
- 📢 **Share with your network** on LinkedIn, Twitter/X, Reddit, or developer forums.
- ☕ **Buy me a coffee / Sponsor**: Support ongoing maintenance and security research via [GitHub Sponsors](https://github.com/sponsors/ishandutta2007).

[![Sponsor ishandutta2007](https://img.shields.io/badge/Sponsor-%E2%9D%A4-ea4aaa?style=for-the-badge&logo=github-sponsors&logoColor=white)](https://github.com/sponsors/ishandutta2007)

---

## 🤝 How to Contribute

Contributions are welcome! Please follow these simple guidelines:

1. Fork this repository.
2. Add or update entries in `README.md` keeping descriptions objective and factual.
3. Submit a Pull Request (PR) with a brief summary of your additions.

---

## ⚠️ Security & Legal Disclaimer

- This list is maintained for educational, defensive, and authorized security auditing purposes only.
- Scanning public or private systems for exposed credentials must only be performed on assets you own or have explicit authorization to test. Unauthorized credential exploitation is illegal.

---

## 📈 Star History

[![Star History Chart](https://star-history.dera.page/svg?repos=ishandutta2007/Awesome-Developer-Secrets-Scanning&type=date&legend=top-left)](https://star-history.dera.page/#ishandutta2007/Awesome-Developer-Secrets-Scanning&type=date&legend=top-left)
