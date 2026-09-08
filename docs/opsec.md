# OPSEC for OSINT Research

Operational Security (OPSEC) is about controlling what your own research activity exposes — to the target, to the platforms you use, and to third parties. Good OSINT practice is inseparable from good OPSEC.

> This guide covers safe research hygiene. It does **not** cover evading law enforcement or concealing illegal activity — neither is a legitimate use of this repository. See [Legal & Ethical Use](legal-and-ethical-use.md).

## Separate Research Identities

Use dedicated accounts, browser profiles, and (where appropriate) devices for research that are fully separate from your personal identity:

- Never use personal social media, email, or messaging accounts to view or interact with a subject of research.
- Don't reuse research usernames/handles across your personal life.
- Keep research browser profiles isolated (separate cookies, history, and extensions) from your daily-use profile.

## Avoid Exposing Personal Accounts

Many platforms show "who viewed your profile," suggest mutual connections, or notify users of visits/searches. Assume that any logged-in interaction can be attributed back to your account. Log out or use a research identity before browsing sensitive profiles.

## Understand What Your Browser Leaks

Your browser and network connection reveal more than you might expect:

- IP address (and approximate location) to every site you visit.
- User-Agent, screen resolution, fonts, and other fingerprintable details.
- Referrer headers when following links.
- Cached previews and link unfurling (e.g., messaging apps that fetch a preview of a link you paste) can trigger a request to the target's server before you've even opened the link.

## Use Appropriate Isolation

Depending on sensitivity, consider:

- A separate browser profile or virtual machine dedicated to research.
- Disabling browser extensions that aren't needed for the task (many leak data or fingerprint you).
- Reviewing privacy settings on any research accounts before using them.

## Avoid Interacting with Targets Unnecessarily

Passive collection (viewing public/cached/indexed data) is lower-risk than active interaction (following, messaging, connection requests, liking). Prefer passive methods, and only escalate to active interaction when the objective requires it and you're authorized to do so.

## Understand Tor Limitations

Tor provides network-level anonymity for the *connection*, but it does not anonymize *you* if you log into personal accounts, reveal identifying details in what you type, or misconfigure your browser (e.g., resizing the Tor Browser window, installing extensions, or opening downloaded files while connected). Tor is a tool, not a guarantee.

## Do Not Assume Anonymity

No single tool or technique guarantees anonymity. Combine good practices (separate identities, minimal footprint, awareness of leaks) rather than relying on any one control. Assume your activity could be logged somewhere and act accordingly — legally and ethically.

## Do Not Upload Sensitive Material to Third-Party Services

Free "analysis" tools (image analyzers, metadata strippers, file converters, "check this file" services) often retain what you upload. Before uploading any file or piece of data belonging to a case:

- Confirm the service's data retention and privacy policy.
- Prefer offline/local tools (e.g., [ExifTool](../tools/metadata/exiftool.md) run locally) for sensitive material.
- Never upload confidential, personal, or case-sensitive data to a service you haven't vetted.

## Respect Terms of Service

Automated scraping, bulk queries, or bypassing rate limits can violate a platform's Terms of Service, even when the data itself is public. Excessive automated requests can also get your IP or account blocked, or in some jurisdictions carry legal risk under computer-misuse laws. Use official APIs where available, and respect published rate limits.

## Keep Credentials and Secrets Out of Git

If you build or fork automation around these tools:

- Never commit API keys, tokens, cookies, or session data to a Git repository (see this repository's [`.gitignore`](../.gitignore) and [SECURITY.md](../SECURITY.md)).
- Store credentials in environment variables or a secrets manager, not in scripts.
- Rotate any credential you suspect may have been exposed.

---

Continue to [Legal & Ethical Use](legal-and-ethical-use.md) for the boundaries of acceptable use.
