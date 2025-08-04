---
title: "Produce Well-Secured Software (PW)"
linkTitle: "Produce Well-Secured Software (PW)"
weight: 7
description: >
 Produce Well-Secured Software (PW) CI/CD Steps
---

## Produce Well-Secured Software (PW)

### PW.4 Reuse Existing, Well-Secured Software When Feasible Instead of Duplicating Functionality

Lower the costs of software development, expedite software development, and decrease the likelihood of introducing additional security vulnerabilities into the software by reusing software modules and services that have already had their security posture checked. This is particularly important for software that implements security functionality, such as cryptographic modules and protocols.

<br>

<table style="width:100%">
    <tr>
        <th style="width: 50%">Tasks</th>
        <th style="width: 50%">Tools</th>
    </tr>
    <tr>
        <td rowspan="5">
            <strong>PW.4.1</strong>:
            <p>Acquire and maintain well-secured software components (e.g., software libraries, modules, middleware,
                frameworks) from commercial, opensource, and other third-party developers for use by the organization’s
                software.</p>
        </td>
    </tr>
    <tr>
        <td>
            SBOM Generation and Attestation Tools
            <ul>
                <li><a href="https://cyclonedx.org/">CycloneDX</a></li>
                <li><a href="https://github.com/opensbom-generator/spdx-sbom-generator">SPDX</a></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            Binary Repositories
            <ul>
                <li><a href="https://artifacthub.io/">ArtifactHub</a></li>
                <li><a href="https://jfrog.com/community/download-artifactory-oss/">JFrog Artifactory OSS</a></li>
                <li><a href="https://www.sonatype.com/products/nexus-community-edition-download">Sonatype Nexus OSS</a>
                </li>
                <li><a href="https://goharbor.io/">Harbor</a></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            Git Commit Signing
            <ul>
                <li><a
                        href="https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits">GitHub
                        Signing</a></li>
                <li><a href="https://docs.gitlab.com/ee/user/project/repository/signed_commits/">GitLab Signing</a></li>
                <li><a
                        href="https://confluence.atlassian.com/bitbucketserver/using-gpg-keys-913477014.html">Bitbucket</a>
                </li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            Repo Security Scanning
            <ul>
                <li><a href="https://codeql.github.com/">GitHub CodeQL</a></li>
                <li><a href="https://www.aquasec.com/products/trivy/">AquaSec Trivy</a></li>
                <li><a
                        href="https://docs.github.com/en/enterprise-server@3.4/admin/configuration/configuring-github-connect/enabling-dependabot-for-your-enterprise">Dependabot</a>
                </li>
                <li><a href="https://github.com/jfrog/frogbot">FrogBot</a></li>
                <li><a href="https://openssf.org/projects/allstar/">Allstar</a></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td rowspan="2">
            <strong>PW.4.2</strong>: <p>Create and maintain well-secured software components in-house following SDLC
                processes to meet common internal software development needs that cannot be better met by third-party
                software components.</p>
        </td>
    </tr>
    <tr>
        <td>
        </td>
    </tr>
    <tr>
        <td rowspan="2">
            <strong>PW.4.3</strong>: <p>Moved to PW.1.3</p>
        </td>
    </tr>
    <tr>
        <td>
        </td>
    </tr>
    <tr>
        <td rowspan="2">
            <strong>PW.4.4</strong>: <p>Verify that acquired commercial, open-source, and all other third-party software components comply with the requirements, as defined by the organization, throughout their life cycles.</p>
        </td>
    </tr>
    <tr>
        <td>
        </td>
    </tr>
    <tr>
        <td rowspan="2">
            <strong>PW.4.5</strong>: <p>Moved to PW.4.1 and PW.4.4</p>
        </td>
    </tr>
    <tr>
        <td>
        </td>
    </tr>
</table>

<br>

## PW.7 Review and/or Analyze Human-Readable Code to Identify Vulnerabilities and Verify Compliance with Security Requirements

Help identify vulnerabilities so that they can be corrected before the software is released to prevent exploitation. Using automated methods lowers the effort and resources needed to detect vulnerabilities. Human-readable code includes source code, scripts, and any other form of code that an organization deems humanreadable.

<br>
<table style="width:100%">
    <tr>
        <th style="width: 50%">Tasks</th>
        <th style="width: 50%">Tools</th>
    </tr>
    <tr>
        <td rowspan="2">
            <strong>PW.7.1</strong>:
            <p>Determine whether code review (a person looks directly at the code to find issues) and/or code analysis
                (tools are used to find issues in code, either in a fully automated way or in conjunction with a person)
                should be used, as defined by the organization.</p>
        </td>
    </tr>
    <tr>
        <td>
            <ul>
                <li><a href="https://owasp.org/www-project-dependency-check/">OWASP Dependency-Check</a></li>
                <li><a href="https://github.com/DependencyTrack/dependency-track">Dependency-Track</a></li>
                <li><a href="https://www.zaproxy.org/">OWASP ZAP</a></li>
                <li><a
                        href="https://www.sonarsource.com/open-source-editions/sonarqube-community-edition/">SonarQube</a>
                </li>
                <li><a
                        href="https://www.sonarsource.com/open-source-editions/sonarqube-community-edition/">Retire.js</a>
                </li>
                <li><a href="https://fossa.com/product/open-source-vulnerability-management">Fossa</a></li>
                <li><a href="https://www.veracode.com/">Veracode</a></li>
                <li><a href="https://www.sonarsource.com/open-source-editions/">SonarQube</a></li>
                <li><a href="https://github.com/semgrep/semgrep">Semgrep</a></li>
                <li><a href="https://github.com/PyCQA/bandit">Bandit for Python</a></li>
                <li><a href="https://github.com/Checkmarx/kics">Checkmarx KICS</a></li>
                <li><a href="https://github.com/danmar/cppcheck">Cppcheck for C++</a></li>
                <li><a href="https://github.com/find-sec-bugs/find-sec-bugs">FindSecBugs</a></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td rowspan="2">
            <strong>PW.7.2</strong>:
            <p>Perform the code review and/or code analysis based on the organization’s secure coding standards, and record and triage all discovered issues and recommended remediations in the development team’s workflow or issue tracking system.</p>
        </td>
    </tr>
    <tr>
        <td>
        </td>
    </tr>
</table>
<br>

---
