---
title: "Protect the Software (PS)"
linkTitle: "Protect the Software (PS)"
weight: 6
description: >
 Protect the Software (PS) Post-Deployment Steps
---

### Protect the Software (PS)
Organizations should protect all components of their software from tampering and unauthorized access. 

The following task achieve the goals of PS post deployment. 

Note: There are no Post Deploy Tasks for PS.1

<br>


**PS.2 and PS.3**

<strong>Provide a Mechanism for Verifying Software Release Integrity (PS.2):</strong> Help software acquirers ensure that the software they acquire is legitimate and has not been tampered with. Make software integrity verification information available to software acquirers.

<br>

<strong> Archive and Protect Each Software Release (PS.3):</strong> Preserve software releases in order to help identify, analyze, and eliminate vulnerabilities discovered in the software after release.




<br>

<table style="width:100%">
  <tr>
    <th style="width: 50%">Tasks</th>
    <th style="width: 50%">Tools</th>
  </tr>
  <tr>
    <td rowspan="3">
      <strong>PS.2.1</strong>:
      <p>Make software integrity verification information available to software acquirers.</p>
    </td>
    <td>
      <a href="https://docs.sigstore.dev/cosign/"> cosign Sigstore</a>
      </a>
      <p>Sign container images, SBOMs, and binaries post-deployment. Verify those signatures using a public key or keyless (OIDC) identity. Create signed attestations showing how, where, and by whom the software was built—even after it’s deployed.</p>
    </td>
  </tr>
  <tr>
    <td>
      <a href="https://docs.sigstore.dev/logging/overview/">Rekor Sigstore Transparency Log</a>
      <p>Publishes signatures to a tamper-proof public ledger. Acquirers can verify your deployment artifacts were signed and published.</p>
    </td>
  </tr>
  <tr>
    <td>
      <a href="https://ortelius.io">Ortelius Evidence Store </a>
      <p>Track deployed versions, their components, and associated SBOMs. Gives acquirers access to historical release metadata for verification.</p>
    </td>
  </tr>
  <tr>
    <td rowspan="7">
      <strong>PS.3.1</strong>:
      <p>Make software integrity verification information available to software acquirers.</p>
      <div style="height: 16px"></div>
      <p style="font-style: italic">Use code-based configuration for toolchains (e.g., pipelines-as-code, toolchains-as-code).</p>
    </td>
    <td>
      <a href=" https://in-toto.io">In-Toto</a>
      <p>Signs and verifies metadata (“link files”) associated with the build and release process. Acquirers can confirm that software went through a trusted, verified build process.</p>
    </td>
  </tr>
  <tr>
    <td>
      <a href="https://spdx.dev">SPDX</a>
      <p>Signed SBOMs can be shared alongside artifacts so acquirers verify the software’s component integrity.</p>
    </td>
  </tr>
  <tr>
    <td>
      <a href="https://cyclonedx.org">CycloneDX</a>
      <p>Signed SBOMs can be shared alongside artifacts so acquirers verify the software’s component integrity.</p>
    </td>
  </tr>
  <tr>
    <td>
      <a href="https://ortelius.io">Ortelius Evidence Store</a>
      <p>Continuously synchronizes SBOM data for each deployed release against OSV.dev to identify new vulnerabilities post deployment. </p>
    </td>
  </tr>
  <tr>
    <td>
      <a href="https://gnupg.org">GNU Private Guard</a>
      <p>Sign binary releases, SBOMs, and changelogs so acquirers can verify authenticity using public key</p>
    </td>
  </tr>
  <tr>
    <td>
      <a href="https://oss.sonatype.org">Sonatype Nexus OSS - Store Build Artifacts</a>
      <p>Hosts signed artifacts and associated metadata in a publicly or securely accessible location for acquirers.</p>
    </td>
  </tr>
  <tr>
    <td>
       <a href="https://jfrog.com/community/download-artifactory-oss/">JFrog Artifactory OSS - Store Build Artifacts</a>
       <p>Hosts signed artifacts and associated metadata in a publicly or securely accessible location for acquirers.</p>
    </td>
  </tr>
  <tr>
    <td rowspan="10">
      <strong>PS.3.2</strong>:
      <p>Collect, safeguard, maintain, and share provenance data for all components of each software release.  </p>
      <div style="height: 16px"></div>
      <p style="font-style: italic">e.g., in a software bill of materials.</p>
    </td>
    <tr>
    <td>
      <a href="https://spdx.dev">SPDX Generator</a>
      <p>Automatically generates SBOMs from containers, filesystems, and source code. Supports multiple language ecosystems.</p>
    </td>
  </tr>
  <tr>
    <td>
      <a href="https://cyclonedx.org">CycloneDX CLI</a>
      <p>Automatically generates SBOMs from containers, filesystems, and source code. Validates, signs, and transforms SBOMs.</p>
    </td>
  </tr>
  <tr>
    <td>
      <a href="https://trivy.dev/latest/">Trivy</a>
      <p>Combines SBOM generation and vulnerability scanning</p>
    </td>
  </tr>
  <tr>
    <td>
      <a href="https://ortelius.io">Ortelius Evidence Store</a>
      <p>Maintains historical versions of application components, their SBOMs, and deployment locations across time.</p>
    </td>
  </tr>
  </table>
    




