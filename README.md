<div align="center">

<img src="assets/aramon-logo.png" alt="Aramon" width="120" />

# Aramon OSINT Toolkit

### Personal Mirror / Showcase

A curated Open Source Intelligence toolkit and knowledge base for cybersecurity students, researchers, analysts, and authorized investigations.

[![Personal Mirror](https://img.shields.io/badge/status-personal%20mirror-0a0a0a?style=flat-square&labelColor=111)](https://github.com/Aramon-IT/OSINT)
[![Tools](https://img.shields.io/badge/tools-32-0a0a0a?style=flat-square&labelColor=111)](#-tool-directory)
[![Categories](https://img.shields.io/badge/categories-13-0a0a0a?style=flat-square&labelColor=111)](#-tool-directory)
[![License](https://img.shields.io/badge/license-MIT-0a0a0a?style=flat-square&labelColor=111)](LICENSE)
[![Maintained](https://img.shields.io/badge/maintained-yes-0a0a0a?style=flat-square&labelColor=111)](CHANGELOG.md)

</div>

---

> 👤 **This is a personal showcase mirror maintained by [@Anas-Magane](https://github.com/Anas-Magane).** The **official, actively maintained source of truth** is **[Aramon-IT/OSINT](https://github.com/Aramon-IT/OSINT)**, maintained under the Aramon Institute of IT organization — refer there for the latest updates and to contribute.

A curated collection of OSINT tools, resources, methodologies, and practical references maintained by **Aramon Institute of IT**. Built for cybersecurity researchers, students, journalists, and anyone conducting lawful, ethical open-source investigations — from a first search to a full attack-surface assessment.

This is not a dump of links. Every tool listed here has been evaluated for maintenance status, official source, and real-world usefulness — see [how we curate](CONTRIBUTING.md#before-you-submit-quality-checklist).

> ⚖️ **Read this first:** this repository is for education, defensive security, journalism, and authorized investigations only. See [Legal & Ethical Use](docs/legal-and-ethical-use.md).

---

## 📘 Aramon OSINT Guide

**[📥 Download the Aramon OSINT Guide (PDF)](docs/OSINT_Guide_Aramon.pdf)**

A companion guide to this repository — read it alongside the living, continuously updated content here on GitHub.

---

## Table of Contents

- [Quick Start](#-quick-start)
- [Navigation](#navigation)
- [Tool Directory](#-tool-directory)
- [Guides](#-guides)
- [Resources](#%EF%B8%8F-resources)
- [Contributing](#-contributing)
- [Legal & Ethical Use](#%EF%B8%8F-legal--ethical-use)
- [Security](#-security)
- [Roadmap](#%EF%B8%8F-roadmap)

---

## 🚦 Quick Start

New to this repository? Follow this path:

1. **Read first:** [Getting Started](docs/getting-started.md) — what OSINT is, passive vs. active, verification.
2. **Understand the workflow:** [Methodology](docs/methodology.md) — the 13-step process used throughout this repo.
3. **Protect yourself:** [OPSEC](docs/opsec.md) — before you run any tool against a real target.
4. **Know the boundaries:** [Legal & Ethical Use](docs/legal-and-ethical-use.md) — required reading, no exceptions.
5. **Pick a tool:** browse the [Tool Directory](#-tool-directory) below or a [category folder](tools/) directly.
6. **Go deeper:** download the [Aramon OSINT Guide (PDF)](docs/OSINT_Guide_Aramon.pdf).

---

## Navigation

| | | |
|---|---|---|
| 🚀 [Getting Started](docs/getting-started.md) | 🧰 [Tools](#-tool-directory) | 📚 [Guides](docs/) |
| 🔎 [Search Engines](tools/search-engines/) | 🕵️ [Username OSINT](tools/username/) | 📧 [Email OSINT](tools/email/) |
| 🌐 [Domain & Infrastructure](tools/domains/) | 🖼️ [Image OSINT](tools/images/) | 🧬 [Metadata](tools/metadata/) |
| 🛡️ [Threat Intelligence](tools/threat-intelligence/) | 🌑 [Dark Web Research](tools/dark-web/) | ⚙️ [Automation](tools/automation/) |
| 📘 [Aramon OSINT Guide](docs/OSINT_Guide_Aramon.pdf) | 🤝 [Contributing](CONTRIBUTING.md) | ⚖️ [Legal & Ethical Use](docs/legal-and-ethical-use.md) |

---

## 🧰 Tool Directory

A high-signal selection — not an exhaustive list. Full write-up (install, usage, limitations, OPSEC) linked from each tool name.

| Category | Tool | Purpose | Level | Status |
|---|---|---|---|---|
| Username | [Sherlock](tools/username/sherlock.md) | Username enumeration across platforms | Beginner | ✅ Active |
| Username | [Maigret](tools/username/maigret.md) | Deeper username investigation & reporting | Intermediate | ✅ Active |
| Username | [WhatsMyName](tools/username/whatsmyname.md) | Open username-signature dataset | Beginner | ✅ Active |
| Email | [Holehe](tools/email/holehe.md) | Check email registration traces | Intermediate | ⚠️ Low activity |
| Email | [Epieos](tools/email/epieos.md) | Email-to-identity lookup | Beginner | ✅ Active |
| Domains | [Amass](tools/domains/amass.md) | Attack surface / asset discovery | Advanced | ✅ Active |
| Domains | [Subfinder](tools/domains/subfinder.md) | Fast passive subdomain discovery | Intermediate | ✅ Active |
| Domains | [Assetfinder](tools/domains/assetfinder.md) | Lightweight domain/subdomain discovery | Beginner | ⚠️ Stable |
| Domains | [dnsx](tools/domains/dnsx.md) | DNS resolution & probing at scale | Intermediate | ✅ Active |
| Domains | [Shodan](tools/domains/shodan.md) | Internet-connected device search | Beginner | ✅ Active |
| Domains | [Censys](tools/domains/censys.md) | Internet-wide scan & cert search | Intermediate | ✅ Active |
| Reconnaissance | [theHarvester](tools/reconnaissance/theharvester.md) | Emails, subdomains & hosts aggregation | Beginner | ✅ Active |
| Search Engines | [Google Dorking](tools/search-engines/google-dorking.md) | Advanced search operators | Beginner | ✅ Active |
| Images | [TinEye](tools/images/tineye.md) | Reverse image search | Beginner | ✅ Active |
| Images | [Google Lens](tools/images/google-lens.md) | Visual search & object/location ID | Beginner | ✅ Active |
| Images | [Yandex Images](tools/images/yandex-images.md) | Reverse image search (alt. index) | Beginner | ✅ Active |
| Metadata | [ExifTool](tools/metadata/exiftool.md) | Metadata extraction | Beginner | ✅ Active |
| Metadata | [MediaInfo](tools/metadata/mediainfo.md) | Audio/video technical metadata | Beginner | ✅ Active |
| Social Media | [Social-Analyzer](tools/social-media/social-analyzer.md) | Cross-platform presence analysis | Intermediate | ✅ Active |
| Breach Intel | [Have I Been Pwned](tools/breach-intelligence/haveibeenpwned.md) | Email breach-exposure lookup | Beginner | ✅ Active |
| Breach Intel | [h8mail](tools/breach-intelligence/h8mail.md) | Multi-source breach hunting | Intermediate | ⚠️ Low activity |
| Dark Web | [Tor Browser](tools/dark-web/tor-browser.md) | Official onion-network browser | Beginner | ✅ Active |
| Dark Web | [Ahmia](tools/dark-web/ahmia.md) | Filtered legitimate onion search engine | Beginner | ✅ Active |
| Threat Intel | [VirusTotal](tools/threat-intelligence/virustotal.md) | File/domain/IP reputation | Beginner | ✅ Active |
| Threat Intel | [URLScan.io](tools/threat-intelligence/urlscan.md) | Sandboxed URL analysis | Intermediate | ✅ Active |
| Threat Intel | [AbuseIPDB](tools/threat-intelligence/abuseipdb.md) | IP abuse reputation | Beginner | ✅ Active |
| Threat Intel | [AlienVault OTX](tools/threat-intelligence/alienvault-otx.md) | Community threat-intel exchange | Intermediate | ✅ Active |
| Threat Intel | [GreyNoise](tools/threat-intelligence/greynoise.md) | Internet scan-noise classification | Intermediate | ✅ Active |
| Automation | [SpiderFoot](tools/automation/spiderfoot.md) | Automated multi-source OSINT | Intermediate | ✅ Active |
| Automation | [Recon-ng](tools/automation/recon-ng.md) | Modular recon framework | Advanced | ⚠️ Low activity |
| All-in-One | [OSINT Framework](tools/all-in-one/osint-framework.md) | Categorized resource directory | Beginner | ✅ Active |
| All-in-One | [Maltego](tools/all-in-one/maltego.md) | Visual link analysis | Advanced | ✅ Active |

Browse every category folder directly: [username](tools/username/) · [email](tools/email/) · [domains](tools/domains/) · [reconnaissance](tools/reconnaissance/) · [search-engines](tools/search-engines/) · [social-media](tools/social-media/) · [images](tools/images/) · [metadata](tools/metadata/) · [breach-intelligence](tools/breach-intelligence/) · [dark-web](tools/dark-web/) · [threat-intelligence](tools/threat-intelligence/) · [automation](tools/automation/) · [all-in-one](tools/all-in-one/)

**Status legend:** ✅ Active — regularly maintained · ⚠️ Low activity / Stable — functional but infrequently updated, verify before relying on it · ⚠️ Archived / Unmaintained — no longer maintained, use with caution.

---

## 📚 Guides

| Guide | Description |
|---|---|
| [Getting Started](docs/getting-started.md) | What OSINT is, passive vs. active, verification, false positives. |
| [Methodology](docs/methodology.md) | 13-step professional OSINT workflow. |
| [OPSEC](docs/opsec.md) | Safe research identity, browser hygiene, Tor limitations. |
| [Legal & Ethical Use](docs/legal-and-ethical-use.md) | Scope of acceptable use — required reading. |

## 🗂️ Resources

- [Search Engines](resources/search-engines.md) — general-purpose and specialized engines.
- [Useful Websites](resources/useful-websites.md) — WHOIS, certificate transparency, archives.
- [Wordlists](resources/wordlists.md) — for authorized subdomain/content enumeration.
- [Learning Resources](resources/learning-resources.md) — where to go deeper.

---

## 🤝 Contributing

Contributions are welcome — new tools, broken-link fixes, documentation improvements. Every addition goes through a [quality checklist](CONTRIBUTING.md#before-you-submit-quality-checklist) (official source, maintenance status, license, legality). See [CONTRIBUTING.md](CONTRIBUTING.md).

## ⚖️ Legal & Ethical Use

This repository is for education, cybersecurity research, defensive security, journalism, authorized investigations, and CTF/lab environments only. It must never be used for harassment, stalking, doxxing, or unauthorized access. Full policy: [docs/legal-and-ethical-use.md](docs/legal-and-ethical-use.md).

## 🔐 Security

Found a malicious link, an accidentally-committed secret, or a tool that's turned unsafe? See [SECURITY.md](SECURITY.md) for responsible disclosure.

## 🗺️ Roadmap

Modest, honest goals — no exaggerated claims:

- Periodic review of tool maintenance status (quarterly link/status check).
- Expand tool write-ups as new categories prove genuinely useful (quality over quantity — see the [curation checklist](CONTRIBUTING.md#before-you-submit-quality-checklist)).
- Community contributions for broken links and outdated entries via [CONTRIBUTING.md](CONTRIBUTING.md).

---

<div align="center">

Personal mirror by **[@Anas-Magane](https://github.com/Anas-Magane)** · [MIT License](LICENSE) · [Code of Conduct](CODE_OF_CONDUCT.md)

Official project: **[Aramon-IT/OSINT](https://github.com/Aramon-IT/OSINT)** — maintained by Aramon Institute of IT

</div>
