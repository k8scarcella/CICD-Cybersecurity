---
title: "Phase 1: Code and Prebuild"
linkTitle: "Code and Prebuild"
weight: 20
layout: docs
---
## Introduction

Integrating security into every stage of the Software Development Life Cycle (SDLC) is more critical than ever. The code and prebuild stage is foundational to creating secure, reliable, and high-performing applications. Failing to address vulnerabilities early can lead to costly fixes, data breaches, and reputational damage down the line.

This section provides a comprehensive guide to the essential security tools that developers and DevOps teams should use during the code and prebuild phase to ensure vulnerabilities are identified and mitigated before they can cause harm. From Static Application Security Testing (SAST) to dependency scanning and secure CI/CD pipelines, the right tools can help you adopt a proactive approach to software security while maintaining development velocity.



## Open-Source Tooling

### Git Commit Signing 
- [GitHub Signing](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits)
- [GitLab Signing](https://docs.gitlab.com/ee/user/project/repository/signed_commits/)
- [Bit Bucket](https://confluence.atlassian.com/bitbucketserver/using-gpg-keys-913477014.html)

### Repo Security Scanning 
- [GitHub CodeQL](https://codeql.github.com/)
- [AquaSec Trivy](https://www.aquasec.com/products/trivy/)
- [Dependabot](https://docs.github.com/en/enterprise-server@3.4/admin/configuration/configuring-github-connect/enabling-dependabot-for-your-enterprise)
- [FrogBot](https://github.com/jfrog/frogbot)
- [Allstar](https://openssf.org/projects/allstar/)

### SCA Code Scanning Tools
- [Veracode](https://www.veracode.com/)
- [SonarQube](https://www.sonarsource.com/open-source-editions/)
- [Semgrep](https://github.com/semgrep/semgrep)
- [Bandit for Python](https://github.com/PyCQA/bandit)
- [Checkmarx KICS](https://github.com/Checkmarx/kics)
- [Cppcheck for C##](https://github.com/danmar/cppcheck)
- [FindSecBugs](https://github.com/find-sec-bugs/find-sec-bugs)

### Workflow Auditing
- [Intoto](https://in-toto.io/docs/what-is-in-toto/)
