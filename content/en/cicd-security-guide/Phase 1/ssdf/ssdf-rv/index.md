---
title: "Respond to Vulnerabilites"
linkTitle: "Respond to Vulnerabilities (RV)"
weight: 8
description: >
 Respond to Vulnerabilities (RV) CI/CD Steps
---


## Respond to Vulnerabilities (RV)

### RV.1 Identify and Confirm Vulnerabilities on an Ongoing Basis

Help ensure that vulnerabilities are identified more quickly so that they can be remediated more quickly in accordance with risk, reducing the window of opportunity for attackers.

<br>

<table style="width:100%">
    <tr>
        <th style="width: 50%">Tasks</th>
        <th style="width: 50%">Tools</th>
    </tr>
    <tr>
        <td rowspan="2">
            <strong>RV.1.1</strong>:
            <p>Gather information from software acquirers, users, and public sources on potential vulnerabilities in the
                software and third-party components that the software uses, and investigate all credible reports.</p>
        </td>
    </tr>
    <tr>
        <td>
        </td>
    </tr>
    <tr>
        <td rowspan="2">
            <strong>RV.1.2</strong>:
            <p>Review, analyze, and/or test the software’s code to identify or confirm the presence of previously
                undetected vulnerabilities.</p>
        </td>
    </tr>
    <tr>
        <td>
        </td>
    </tr>
    <tr>
        <td rowspan="2">
            <strong>RV.1.3</strong>:
            <p>Have a policy that addresses vulnerability disclosure and remediation, and implement the roles,
                responsibilities, and processes needed to support that policy.</p>
        </td>
    </tr>
    <tr>
        <td>
        </td>
    </tr>
</table>
<br>

### RV.2 Assess, Prioritize, and Remediate Vulnerabilities

Help ensure that vulnerabilities are remediated in accordance with risk to reduce the window of opportunity for attackers.

<br>

<table style="width:100%">
    <tr>
        <th style="width: 50%">Tasks</th>
        <th style="width: 50%">Tools</th>
    </tr>
    <tr>
        <td rowspan="2">
            <strong>RV.2.1</strong>:
            <p>Analyze each vulnerability to gather sufficient information about risk to plan its remediation or other risk response.</p>
        </td>
    </tr>
    <tr>
        <td>
        </td>
    </tr>
    <tr>
        <td rowspan="2">
            <strong>RV.2.2</strong>:
            <p>Plan and implement risk responses for vulnerabilities.</p>
        </td>
    </tr>
    <tr>
        <td>
        </td>
    </tr>
</table>
<br>


### RV.3 Analyze Vulnerabilities to Identify Their Root Causes

Help reduce the frequency of vulnerabilities in the future.
<br>

<table style="width:100%">
    <tr>
        <th style="width: 50%">Tasks</th>
        <th style="width: 50%">Tools</th>
    </tr>
    <tr>
        <td rowspan="2">
            <strong>RV.3.1</strong>:
            <p>: Analyze identified vulnerabilities to determine their root causes.</p>
        </td>
    </tr>
    <tr>
        <td>
        </td>
    </tr>
    <tr>
        <td rowspan="2">
            <strong>RV.3.2</strong>:
            <p>Analyze the root causes over time to identify patterns, such as a particular secure coding practice not
                being followed consistently.</p>
        </td>
    </tr>
    <tr>
        <td>
        </td>
    </tr>
    <tr>
        <td rowspan="2">
            <strong>RV.3.3</strong>:
            <p>Review the software for similar vulnerabilities to eradicate a class of vulnerabilities, and proactively
                fix them rather than waiting for external reports.</p>
        </td>
    </tr>
    <tr>
        <td>
        </td>
    </tr>
    <tr>
        <td rowspan="2">
            <strong>RV.3.4</strong>:
            <p>Review the SDLC process, and update it if appropriate to prevent (or reduce the likelihood of) the root
                cause recurring in updates to the software or in new software that is created.</p>
        </td>
    </tr>
    <tr>
        <td>
        </td>
    </tr>
</table>
<br>

_Static Application Security Testing (SAST):_

- [Semgrep](https://semgrep.dev/)
- [SonarQube](https://www.sonarqube.org/)
- [CodeQL](https://codeql.github.com/)

_Dynamic Application Security Testing (DAST):_

- [OWASP ZAP](https://www.zaproxy.org/)
- [w3af](https://github.com/andresriancho/w3af)

_Software Composition Analysis (SCA):_

- [OWASP Dependency-Check](https://owasp.org/www-project-dependency-check/)
- [Trivy]( https://github.com/aquasecurity/trivy)
- [Grype](https://github.com/anchore/grype)

**RV.2 Assess, Prioritize, and Remediate Vulnerabilities**

- [OWASP Defectdojo](https://www.defectdojo.org/)
- [GitLab Security Scanning](https://docs.gitlab.com/ee/user/application_security/)
- [Tsunami Security Scanner](https://github.com/google/tsunami-security-scanner)


**RV.3 Identify Root Cause and help to reduce frequency of vulnerabilities in the future**
- [Open Policy Agent (OPA)]( https://www.openpolicyagent.org/)
- [Sigstore](https://www.sigstore.dev/)
- [in-toto](https://in-toto.io/)
