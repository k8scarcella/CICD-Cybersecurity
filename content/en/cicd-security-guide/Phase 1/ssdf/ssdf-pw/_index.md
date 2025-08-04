---
title: "Produce Well-Secured Software (PW)"
linkTitle: "Produce Well-Secured Software (PW)"
weight: 7
description: >
 Produce Well-Secured Software (PW) CI/CD Steps
---

### Produce Well-Secured Software (PW)

**PW.4.1 Acquire and Maintain Well-secured Software**

Ensure safe use of components (e.g., software libraries, modules, middleware, frameworks) from commercial, open-source, and other third-party developers for use by the organization’s software. Implement a Software Bill of Materials (SBOM) scan to obtain provenance information for each software component. Establish one or more software repositories to host sanctioned and vetted open-source components.

<u>Open-Source Tools to Achieve:</u>

_SBOM Generation and Attestation Tools:_

- [CycloneDX](https://cyclonedx.org/)
- [SPDX](https://github.com/opensbom-generator/spdx-sbom-generator)

_Binary Repositories:_

- [ArtifactHub](https://artifacthub.io/)
- [JFrog Artifactory OSS](https://jfrog.com/community/download-artifactory-oss/)
- [Sonatype Nexus OSS](https://www.sonatype.com/products/nexus-community-edition-download)
- [Harbor](https://goharbor.io/)

_Git Commit Signing:_

- [GitHub Signing](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits)
- [GitLab Signing](https://docs.gitlab.com/ee/user/project/repository/signed_commits/)
- [Bit Bucket](https://confluence.atlassian.com/bitbucketserver/using-gpg-keys-913477014.html)

_Repo Security Scanning_
- [GitHub CodeQL](https://codeql.github.com/)
- [AquaSec Trivy](https://www.aquasec.com/products/trivy/)
- [Dependabot](https://docs.github.com/en/enterprise-server@3.4/admin/configuration/configuring-github-connect/enabling-dependabot-for-your-enterprise)
- [FrogBot](https://github.com/jfrog/frogbot)
- [Allstar](https://openssf.org/projects/allstar/)


**PW.7 Review and/or Analyze Human-Readable Code**

Help identify vulnerabilities so that they can be corrected before the software is released to prevent exploitation. Using automated methods lowers the effort and resources needed to detect vulnerabilities. Human-readable code includes source code, scripts, and any other form of code that an organization deems human-readable.

<u>Open-Source Tools to Achieve:</u>

- [OWASP Dependency-Check](https://owasp.org/www-project-dependency-check/)
- [Dependency-Track](https://github.com/DependencyTrack/dependency-track)
- [OWASP ZAP](https://www.zaproxy.org/)
- [SonarQube](https://www.sonarsource.com/open-source-editions/sonarqube-community-edition/)
- [Retire.js](https://www.sonarsource.com/open-source-editions/sonarqube-community-edition/)
- [Fossa](https://fossa.com/product/open-source-vulnerability-management)
- [Veracode](https://www.veracode.com/)
- [SonarQube](https://www.sonarsource.com/open-source-editions/)
- [Semgrep](https://github.com/semgrep/semgrep)
- [Bandit for Python](https://github.com/PyCQA/bandit)
- [Checkmarx KICS](https://github.com/Checkmarx/kics)
- [Cppcheck for C##](https://github.com/danmar/cppcheck)
- [FindSecBugs](https://github.com/find-sec-bugs/find-sec-bugs)


<br>

---
