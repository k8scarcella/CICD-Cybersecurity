---
title: "Protect the Software (PS)"
linkTitle: "Protect the Software (PS)"
weight: 6
description: >
 Protect the Software (PS) CI/CD Steps
---

## Protect the Software (PS)

Organizations should protect all components of their software from tampering and unauthorized access.

<br>

### PS.1: Protect All Forms of Code from Unauthorized Access and Tampering.

<br>
Help prevent unauthorized changes to code, both inadvertent and intentional, which could circumvent or negate the intended security characteristics of the software.
For code that is not intended to be publicly accessible, this helps prevent theft of the software and may make it more difficult or time-consuming for attackers to find vulnerabilities in the software.

<br>


<strong>PS.1.1:</strong> Store all forms of code
Store all forms of code – including source code, executable code, and configuration-as-code – based on the principle of least privilege so that only authorized personnel, tools, services, etc. have access.

<br>


_Store all source code and configuration-as-code in a code repository, and restrict access to it based on the nature of the code. For example,  open source code intended for public access may need its integrity and availability protected; other code may also need its confidentiality protected._

<br>

<u>Open-Source or Free Tools to Achieve:</u>

<br>

- [GitHub](https://github.com/)
- [GitLab](https://gitlab.com/)
- [Bitbucket](https://bitbucket.org/)
- [SourceForge](https://sourceforge.net/)

<br>


_Use version control features of the repository to track all changes made to the code with accountability to the individual account._

<br>


<u>Open-Source or Free Tools to Achieve:</u>

<br>

- [Git](https://git-scm.com/)


_Use commit signing for code repositories to sign code._

<br>

<u>Open-Source or Free Tools to Achieve:</u>

<br>

- [GitHub Signing Commits](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits)
- [About commit signature verification](https://docs.github.com/en/authentication/managing-commit-signature-verification/about-commit-signature-verification)
- [GitLab Signed Commits](https://docs.gitlab.com/user/project/repository/signed_commits/)
- [Bitbucket Sign Commits and Tags with SSH keys](https://confluence.atlassian.com/bitbucketserver/sign-commits-and-tags-with-ssh-keys-1305971205.html)
- [Bitbucket Sign Commits and Tags with X.509 certificatesG](https://confluence.atlassian.com/bitbucketserver/sign-commits-and-tags-with-x-509-certificates-1305971206.html)
- [Bitbucket Using GPG Keys](https://confluence.atlassian.com/bitbucketserver/using-gpg-keys-913477014.html)


_Have the code owner review and approve all changes made to the code by others._

<br>

<u>Open-Source or Free Tools to Achieve:</u>

<br>

- [Github CODEOWNERS](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners)
- [GitHub Code Review](https://github.com/features/code-review)
- [Gitlab CODEOWNERS](https://docs.gitlab.com/user/project/codeowners/)
- [Gitlab Code Review Guidelines](https://docs.gitlab.com/development/code_review/)
- [Bitbucket Set Up and Use Code Owners](https://support.atlassian.com/bitbucket-cloud/docs/set-up-and-use-code-owners/)
- [Bitbucket Code Review](https://www.atlassian.com/software/bitbucket/features/code-review)


_Use cryptography (e.g., cryptographic hashes) to help protect file integrity_

<br>


<u>Open-Source or Free Tools to Achieve:</u>

<br>

- [GitHub About Commits](https://docs.github.com/en/pull-requests/committing-changes-to-your-project/creating-and-editing-commits/about-commits)

<br>

### PS.2 Provide a Mechanism for Verifying Software Release Integrity:

Help software acquirers ensure that the software they acquire is legitimate and has not been tampered with. 

<br>

<strong>PS.2.1: </strong> Make software integrity verification information available to software acquirers. 

<br>

_Post cryptographic hashes for release files on a well-secured website._

<br>


<u>Open-Source or Free Tools to Achieve:</u>

<br>

- [Apache Infrastructure Signing Releases](https://infra.apache.org/release-signing.html)
- [OpenPGP](https://www.openpgp.org/)
- [The GNU Privacy Guard](https://www.gnupg.org/)

<br>

_Use an established certificate authority for code signing so that consumers’ operating systems or other tools and services can confirm the validity of signatures before use. Periodically review the code signing processes, including certificate renewal, rotation, revocation, and protection._

<br>

<u>Open-Source or Free Tools to Achieve:</u>

<br>

- [Let's Encrypt](https://letsencrypt.org/)
- [EJBCA Community](https://www.ejbca.org/)
- [Dogtag Certificate System](https://www.dogtagpki.org/)
- [OpenXPKI](https://www.openxpki.org/)
- [Step-CA](https://smallstep.com/product/team/devops/index.html)


### PS.3 Archive and Protect Each Software Release:

Preserve software releases in order to help identify, analyze, and eliminate vulnerabilities discovered in the software after release.

<br>

<strong>PS.3.1: </strong> Securely archive the necessary files and supporting data (e.g., integrity verification information, provenance data) to be retained for each software release. 

<br>

_Store the release files, associated images, etc. in repositories following the organization’s established policy. Allow read-only access to them by necessary personnel and no access by anyone else._

<br>

_Store and protect release integrity verification information and provenance data, such as by keeping it in a separate location from the release files or by signing the data._

<br>

<u>Open-Source or Free Tools to Achieve:</u>

<br>

- [GitHub Repository Roles for an Organization](https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/repository-roles-for-an-organization)
- [GitLab Roles and Permissions](https://docs.gitlab.com/user/permissions/)
- [Bitbucket Grant Access to a Workspace](https://support.atlassian.com/bitbucket-cloud/docs/grant-access-to-a-workspace/)

<br>

<strong>PS.3.2:</strong> Collect, safeguard, maintain, and share provenance data for all components of each software release (e.g., in a Software Bill of Materials (SBOM)). 

<br>

_Make the provenance data available to software acquirers in accordance with the organization’s policies, preferably using standards-based formats._

<br>

<u>Open-Source or Free Tools to Achieve:</u>

<br>

- [CycloneDX](https://cyclonedx.org/)
- [SPDX](https://spdx.dev/)
- [Software Identification (SWID) Tagging Tools and Utilities](https://github.com/usnistgov/swid-tools)

<br>

 _Make the provenance data available to the organization’s operations and response teams to aid them in mitigating software vulnerabilities._

<br>

<u>Open-Source or Free Tools to Achieve:</u>

<br>

- [Dependency-Check](https://owasp.org/www-project-dependency-check/)
- [Dependency-Track](https://dependencytrack.org/)
- [Syft](https://github.com/anchore/syft)
- [Grype](https://github.com/anchore/grype)
- [Trivy](https://trivy.dev/latest/)
- [Clair](https://clairproject.org/)
- [Tern](https://github.com/tern-tools/tern)

_Protect the integrity of provenance data, and provide a way for recipients to verify provenance data integrity._

<br>

<u>Open-Source or Free Tools to Achieve:</u>

<br>

- [aoss-verifier](https://github.com/google/aoss-verifier)
- [Sigstore](https://sigstore.dev/)
- [TLSNotary Protocol](https://docs.tlsnotary.org/)

<br>

_Update the provenance data every time any of the software’s components are updated._

<br>
<u>Open-Source or Free Tools to Achieve:</u>

<br>

- [GitHub Actions](https://docs.github.com/en/actions)
- [GitLab CI/CD](https://docs.gitlab.com/ci/)
- [Bitbucket Pipelines](https://www.atlassian.com/software/bitbucket/features/pipelines)
- [CircleCI](https://circleci.com/)
- [Travis CI](https://travis-ci.org/)
- [Updatecli](https://www.updatecli.io/)
- [Renovate](https://www.mend.io/renovate/)
