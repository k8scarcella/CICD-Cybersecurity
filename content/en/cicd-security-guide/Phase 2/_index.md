
---
title: "Phase 2: Build and Deploy"
linkTitle: "Build and Deploy"
weight: 40
layout: docs
---
## Introduction
As software moves from development to production, the build and deploy stages play a pivotal role in maintaining the integrity and security of your application. These stages are where your application is compiled, packaged, and prepared for its live environment, making them prime targets for potential vulnerabilities or malicious attacks.

Integrating security into these phases ensures that your code is not only functional but also safeguarded against threats. From dynamic analysis during builds to automated scans for container security and misconfigurations, the right tools can help identify risks before deployment. Moreover, secure deployment pipelines prevent unauthorized changes, enforce compliance, and enable safe rollouts.

This page explores the key security tools and best practices for the build and deploy phases, ensuring your applications are delivered securely and maintain resilience in production environments. Learn how to protect your software, infrastructure, and users by embedding security into every step of your delivery process.

## Open Source Tooling

### SBOM Tools and Attestation 
- [Apko](https://github.com/chainguard-dev/apko)
- [Docker BuildX](https://docs.docker.com/reference/cli/docker/buildx/build/#attest)

### Open Source Build Signing Tools 

- [sigstore.dev](https://www.sigstore.dev/)
- [Notary](https://notaryproject.dev/)


