<p align="center">
  <img src="https://github.com/merchantprotocol/.github/raw/main/profile/banner.png" alt="Merchant Protocol" width="100%" />
</p>

<h1 align="center">Merchant Protocol</h1>

<p align="center">
  <strong>AI agents and production infrastructure for businesses that move fast.</strong>
  <br />
  We build open-source tools that help teams ship compliant software, automate business workflows, and scale without complexity.
</p>

<p align="center">
  <a href="https://www.merchantprotocol.com"><img src="https://img.shields.io/badge/Website-merchantprotocol.com-0A66C2?style=flat-square" alt="Website" /></a>
  <a href="mailto:jonathon@merchantprotocol.com"><img src="https://img.shields.io/badge/Contact-Email-EA4335?style=flat-square" alt="Email" /></a>
  <a href="https://github.com/merchantprotocol"><img src="https://img.shields.io/github/followers/merchantprotocol?label=Follow&style=flat-square" alt="Followers" /></a>
  <img src="https://img.shields.io/badge/SOC_2-Type_II_Ready-brightgreen?style=flat-square" alt="SOC 2" />
  <img src="https://img.shields.io/badge/License-Open_Source-blue?style=flat-square" alt="Open Source" />
</p>

---

## What We Do

We're a Seattle-based engineering team focused on three things:

1. **AI Agents** — Desktop and server-side agents that handle real business workflows, with a plugin ecosystem anyone can extend.
2. **Production Infrastructure** — SOC 2 compliant Docker images, CI/CD pipelines, and deployment tools built for regulated industries.
3. **Marketing Technology** — Privacy-first tracking, consent management, and audience tooling for modern growth teams.

---

## Flagship Projects

### Sulla — AI Agent Platform

Sulla is our open-source AI agent ecosystem. A desktop app, voice interface, plugin marketplace, and extensible architecture — built for businesses, not demos.

| Repository | What It Does |
|:-----------|:-------------|
| [**sulla-desktop**](https://github.com/merchantprotocol/sulla-desktop) | Business-ready AI agent for desktop. Easy to install, free to run. `Apache-2.0` |
| [**sulla-recipes**](https://github.com/merchantprotocol/sulla-recipes) | Plugin registry — browse, install, and contribute extensions. |
| [**sulla-voice-ai**](https://github.com/merchantprotocol/sulla-voice-ai) | Voice interface for hands-free agent interaction. |
| [**sulla-commercial-plugins**](https://github.com/merchantprotocol/sulla-commercial-plugins) | Premium plugins for advanced business workflows. |
| [**sulla-upgrade-responder**](https://github.com/merchantprotocol/sulla-upgrade-responder) | Telemetry and update service for the Sulla ecosystem. |
| [**agents**](https://github.com/merchantprotocol/agents) | Reusable agent definitions and templates. |
| [**skills**](https://github.com/merchantprotocol/skills) | Modular skill packs that extend agent capabilities. |
| [**workflows**](https://github.com/merchantprotocol/workflows) | Pre-built automation workflows for common business tasks. |
| [**integrations**](https://github.com/merchantprotocol/integrations) | Connectors for third-party services and APIs. |

---

### Infrastructure & DevOps

Production-grade images and deployment tools designed for SOC 2, HIPAA, and PCI compliance from day one.

| Repository | What It Does |
|:-----------|:-------------|
| [**docker-nginx-php8.2-fpm**](https://github.com/merchantprotocol/docker-nginx-php8.2-fpm) | Ubuntu 24.04 + Nginx + PHP 8.2 FPM + ModSecurity WAF + Wazuh SIEM. `MIT` |
| [**docker-nginx-php8.1-fpm**](https://github.com/merchantprotocol/docker-nginx-php8.1-fpm) | Production Docker image for PHP 8.1 applications. |
| [**docker-nginx-php8.2-ffmpeg**](https://github.com/merchantprotocol/docker-nginx-php8.2-ffmpeg) | PHP 8.2 image with FFmpeg for media processing workloads. |
| [**protocol**](https://github.com/merchantprotocol/protocol) | Push a tag, set one variable, every node deploys. Encrypted secrets, instant rollback, full audit trail. `MIT` |
| [**launchpad**](https://github.com/merchantprotocol/launchpad) | Orchestration and provisioning for new environments. |
| [**aws-cloudformation-templates**](https://github.com/merchantprotocol/aws-cloudformation-templates) | Reusable CloudFormation templates for AWS infrastructure. |
| [**runpod-installation-scripts**](https://github.com/merchantprotocol/runpod-installation-scripts) | Setup scripts for GPU compute on RunPod. |

---

### Marketing Technology

Privacy-first tools for consent, tracking, and audience management.

| Repository | What It Does |
|:-----------|:-------------|
| [**ConsentGuard**](https://github.com/merchantprotocol/ConsentGuard) | Lightweight, plug-and-play cookie consent banner. GDPR & CCPA compliant. |
| [**hero-pixel**](https://github.com/merchantprotocol/hero-pixel) | First-party tracking pixel for privacy-respecting analytics. |
| [**heropixel-wordpress-plugin**](https://github.com/merchantprotocol/heropixel-wordpress-plugin) | HeroPixel integration for WordPress sites. |
| [**inbound**](https://github.com/merchantprotocol/inbound) | Inbound lead capture and routing engine. |
| [**outbound**](https://github.com/merchantprotocol/outbound) | Outbound campaign management platform. |
| [**content-planner**](https://github.com/merchantprotocol/content-planner) | Content calendar and publishing workflow tool. |

---

## Architecture & Principles

```
┌─────────────────────────────────────────────────────────────┐
│                      SULLA DESKTOP                          │
│              AI Agent + Voice + Plugin System               │
├──────────┬──────────┬───────────┬───────────┬───────────────┤
│  Agents  │  Skills  │ Workflows │ Integr.   │    Recipes    │
├──────────┴──────────┴───────────┴───────────┴───────────────┤
│                   INFRASTRUCTURE                            │
│     Docker Images  ·  Protocol CI/CD  ·  Launchpad          │
├─────────────────────────────────────────────────────────────┤
│                   MARTECH LAYER                             │
│  ConsentGuard  ·  HeroPixel  ·  Inbound  ·  Outbound       │
└─────────────────────────────────────────────────────────────┘
```

**Our engineering principles:**

- **Open source first** — Our core tools are open source under MIT and Apache-2.0 licenses.
- **Compliance by default** — SOC 2 Type II, GDPR, CCPA, and HIPAA considerations built in, not bolted on.
- **Zero-complexity deployment** — If it takes more than one command to deploy, we haven't finished building it.
- **Plugin over platform** — Extend, don't fork. Our agent ecosystem is designed for contribution.

---

## Getting Started

**Try Sulla Desktop** — our AI agent:
```bash
# Clone and run
git clone https://github.com/merchantprotocol/sulla-desktop.git
cd sulla-desktop && npm install && npm start
```

**Deploy a compliant PHP app** in seconds:
```bash
docker pull ghcr.io/merchantprotocol/docker-nginx-php8.2-fpm:latest
docker run -p 80:80 -v ./app:/var/www/html ghcr.io/merchantprotocol/docker-nginx-php8.2-fpm:latest
```

**Add cookie consent** to any site:
```html
<script src="https://cdn.jsdelivr.net/gh/merchantprotocol/ConsentGuard/consentguard.min.js"></script>
```

---

## Contributing

We welcome contributions across all our projects. Here's how to get involved:

1. **Browse open issues** across our repos — look for `good first issue` labels.
2. **Submit a Sulla plugin** — create a recipe and submit a PR to [sulla-recipes](https://github.com/merchantprotocol/sulla-recipes).
3. **Report bugs or request features** — open an issue in the relevant repository.
4. **Join the conversation** — reach out at [jonathon@merchantprotocol.com](mailto:jonathon@merchantprotocol.com).

---

<p align="center">
  <strong>Seattle, WA</strong> · <a href="https://www.merchantprotocol.com">merchantprotocol.com</a> · <a href="mailto:jonathon@merchantprotocol.com">jonathon@merchantprotocol.com</a>
</p>

<p align="center">
  <sub>Building tools we wish existed. Open source since 2016.</sub>
</p>
