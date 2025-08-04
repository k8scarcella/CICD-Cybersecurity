---
title: "Produce Well-Secured Software (PW)"
linkTitle: "Produce Well-Secured Software (PW)"
weight: 7
description: >
 Produce Well-Secured Software (PW) CI/CD Steps
---

### Produce Well-Secured Software (PW)

### SBOM Tools and Attestation
A Software Bill of Materials (SBOM) provides visibility into software components, dependencies, and security risks**. When combined with attestation mechanisms, SBOMs enhance trust and traceability across the software supply chain.

- [Apko](https://github.com/chainguard-dev/apko)
- [Docker BuildX](https://docs.docker.com/reference/cli/docker/buildx/build/#attest)
- [Syft](https://github.com/anchore/syft)
- [Trivy](https://github.com/aquasecurity/trivy)

### Open Source Build Signing and Verification
Ensuring software artifacts remain authentic and unmodified**is essential for a trusted software supply chain**. The following tools provide cryptographic verification**to protect against supply chain attacks**.

- [sigstore.dev](https://www.sigstore.dev/)
- [Notary](https://notaryproject.dev/)
- [in-toto](https://in-toto.io/)
- [GitHub Artifact Attestations](https://github.blog/changelog/2024-06-25-artifact-attestations-is-generally-available/)
- [The Update Framework (TUF)](https://theupdateframework.io/)

### Security-Enhanced Build and Deployment Tooling

Beyond open-source tools, a secure build and deploy pipeline relies on trusted execution environments, deterministic build systems, cryptographic verification, and policy-enforced deployment mechanisms. These technologies provide tamper-proof guarantees, verifiable attestations, and automated security policies to strengthen the software supply chain.

#### 1. Reproducible and Deterministic Build Systems
Ensuring that software builds are reproducible enhances security by allowing independent verification of artifacts. These systems minimize non-determinism and ensure that a given input always produces the same output.

- [Nix](https://nixos.org/)
- [Guix](https://guix.gnu.org/)
- [Bazel](https://bazel.build/)
- [Reproducible Builds](https://reproducible-builds.org/)

#### 2. Trusted Execution Environments (TEEs) and Confidential Computing
Trusted Execution Environments (TEEs) provide hardware-backed isolation to secure the build process, key management, and code execution. These environments ensure confidentiality and integrity in the build and deploy process and can be found in major cloud providers.

- [Intel TDX](https://www.intel.com/content/www/us/en/developer/tools/trust-domain-extensions/overview.html)
- [AMD SEV](https://www.amd.com/en/developer/sev.html)
- [Microsoft CCF (Confidential Consortium Framework)](https://github.com/microsoft/CCF)
- [AWS Nitro Enclaves](https://aws.amazon.com/ec2/nitro/nitro-enclaves/)
- [Confidential Containers](https://github.com/confidential-containers/confidential-containers/)

#### 3. Cryptographic Signing and Verification  ensures authenticity, integrity, and provenance in the software supply chain

- [OpenSSL](https://www.openssl.org/)
- [GnuPG (GPG)](https://gnupg.org/)
- [Bouncy Castle](https://www.bouncycastle.org/)
- [Keylime](https://keylime.dev/)
- [Ethereum Attestation Service (EAS)](https://attest.org/)

#### 4. Secure Build and Deployment Policies
Automated security policy enforcement in CI/CD pipelines ensures only verifiably secure software is built and deployed.

- [Kyverno](https://kyverno.io/)
- [OPA (Open Policy Agent)](https://www.openpolicyagent.org/)
- [SPIFFE/SPIRE](https://spiffe.io/)

.
