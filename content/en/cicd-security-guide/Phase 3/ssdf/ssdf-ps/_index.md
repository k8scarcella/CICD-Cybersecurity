---
title: "Protect the Software (PS)"
linkTitle: "Protect the Software (PS)"
weight: 6
description: >
 Protect the Software (PS) Post-Deployment Steps
---


**PS.32 Provide a Mechanism for Verifying Software Release Integrity**

<br>

  <table style="width:100%">
  <tr>
    <th style="width: 50%">Tasks</th>
    <th style="width: 50%">Tools</th>
  </tr>
  <tr>
    <td rowspan="5">
      <strong>PS.2.1:</strong>
      <p>
   Preserve software releases in order to help identify, analyze, and eliminate vulnerabilities discovered in the software after release. 
      </p>
      <div style="height: 16px"></div>
      <p style="font-style: italic">
       Make software integrity verification information available to software acquirers.
      </p>
    </td>
    <td>
     <a href="https://github.com/anchore/syft"> Anchore Syft - Software Bill of Materials></a>
    </td>
  </tr>
  <tr>
    <td>
       <a href="https://github.com/microsoft/sbom-tool"> Microsoft SBOM Tool</a>
    </td>
  </tr>
   <tr>
    <td>
       <a href="https://github.com/opensbom-generator/spdx-sbom-generator">OpenSSF SPDX SBOM</a>
    </td>
  </tr>
  <tr>
    <td>
       <a href="https://openssf.org/projects/bomctl/">OpenSSF bomctl - SBOM Aggregation</a>
    </td>
  </tr> <tr>
    <td>
       <a href="https://ortelius.io">Ortelius - SBOM Aggregation and Sharing</a>
    </td>
  </tr>


### DAST

- [OWASP Zap](https://github.com/OWASP/www-project-zap)
- [W3AF](https://github.com/andresriancho/w3af)
- [Arachni](https://github.com/Arachni/arachni)
- [Nikto](https://github.com/sullo/nikto)

### Vulnerability Databases
- [OSV.dev](https://osv.dev/)

### Continuous Vulnerability Patch Management
- [Ortelius](https://www.ortelius.io)

### Application Security Compliance Reporting
- [OpenSSF Scorecard](https://openssf.org/projects/scorecard/)


