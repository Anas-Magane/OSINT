# Security Policy

## Reporting a Vulnerability

This repository is a documentation and curated-link resource rather than a running application, but security issues can still arise — for example:

- A link pointing to a malicious/typosquatted site rather than the real official source.
- Documentation that inadvertently encourages unsafe or unlawful use.
- Sensitive data (keys, tokens, credentials) accidentally committed to the repository.
- A referenced tool that has become compromised, malicious, or has changed ownership/purpose.

If you discover any of the above, please report it responsibly rather than opening a public issue:

1. Open a [GitHub Security Advisory](https://docs.github.com/en/code-security/security-advisories) on this repository ("Security" tab → "Report a vulnerability"), **or**
2. Contact the Aramon Institute of IT maintainers directly through the organization's [GitHub profile](https://github.com/Anas-Magane).

Please include:

- A clear description of the issue.
- Steps to reproduce or verify it, if applicable.
- The impact you believe it has.

We will acknowledge reports as quickly as possible and work to resolve valid issues promptly, including correcting or removing affected content.

## Our Commitments

- We do not knowingly link to malicious, pirated, or illegal resources.
- We do not store secrets, API keys, or credentials in this repository (see [`.gitignore`](.gitignore)).
- We periodically review tool links for maintenance status and will mark or remove abandoned/compromised entries.

## Please Do Not

- Publicly disclose a serious issue (e.g., a malicious link actively harming users) before it has been addressed.
- Submit pull requests that add secrets, credentials, or tokens — such PRs will be closed and the reporter asked to rotate any exposed credentials.

## Scope

This policy covers the content of this repository. It does **not** cover the security of third-party tools referenced here — vulnerabilities in those tools should be reported to their respective maintainers via their own official channels.
