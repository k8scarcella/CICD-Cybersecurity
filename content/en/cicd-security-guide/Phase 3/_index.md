---
title: "Phase 3: Post Deploy"
linkTitle: "Post Deploy"
weight: 40
layout: docs
---
## Introduction

The post-deploy stage of your software delivery pipeline is where your application is live and actively serving users. While much of the focus in DevSecOps is on securing code, builds, and deployments, ensuring robust security doesn’t end there. The post-deploy phase is critical for monitoring, maintaining, and adapting to new threats in real time.

This phase includes tools and practices for continuous monitoring, vulnerability management, and incident response. From runtime application self-protection (RASP) to real-time threat detection and log analysis, post-deploy security ensures your application remains secure, compliant, and reliable in production.

## Open Source Tools

### Post Build Software Bill of Material Tools
- [Anchore Syft](https://github.com/anchore/syft)
- [Microsoft SBOM Tool](https://github.com/microsoft/sbom-tool)
- [OpenSSF SPDX](https://github.com/opensbom-generator/spdx-sbom-generator)
- [bomctl](https://openssf.org/projects/bomctl/)

### DAST

- [OWASP Zap](https://github.com/OWASP/www-project-zap)
- [W3AF](https://github.com/andresriancho/w3af)
- [Arachni](https://github.com/Arachni/arachni)
- [Nikto](https://github.com/sullo/nikto)

### Vulnerability Databases
- [OSV.dev](https://osv.dev/)

### Continuous Vulnerability Management
- [Ortelius](https://www.ortelius.io)

### Application Security Compliance Reporting
- [OpenSSF Scorecard](https://openssf.org/projects/scorecard/)

