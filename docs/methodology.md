# OSINT Methodology

A repeatable, professional workflow turns scattered searches into a defensible investigation. This methodology is intentionally tool-agnostic — apply it regardless of which tools from the [directory](../README.md#-tool-directory) you use.

> **Core principle:** every OSINT finding is a hypothesis until it has been independently verified. Treat your output as an assessment with a stated confidence level, not a fact.

## 1. Define Objective

Write down, in one or two sentences, exactly what question you are trying to answer (e.g., "Does this domain belong to a legitimate organization?", "Is this username associated with a known threat actor alias?"). A clear objective prevents scope creep and unnecessary data collection.

## 2. Collect Known Identifiers

List every starting point you already have: name, username, email, domain, IP, phone number, image, company name. These "seeds" drive every subsequent step.

## 3. Passive Discovery

Begin with sources that require no interaction with the target: search engine caches, WHOIS/RDAP records, public breach-notification indexes, archived pages (Wayback Machine), and public records. See [resources/search-engines.md](../resources/search-engines.md).

## 4. Search Engines

Use general-purpose and specialized search engines with advanced operators (site:, filetype:, intitle:, "exact phrase") to surface indexed content that direct browsing would miss. See [tools/search-engines](../tools/search-engines/).

## 5. Username Correlation

Check whether a username appears consistently across platforms using tools such as [Sherlock](../tools/username/sherlock.md), [Maigret](../tools/username/maigret.md), or the [WhatsMyName](../tools/username/whatsmyname.md) database. Treat every hit as unverified until manually confirmed.

## 6. Email Intelligence

Check where an email address is registered ([Holehe](../tools/email/holehe.md), [Epieos](../tools/email/epieos.md)) and whether it appears in known breach datasets ([Have I Been Pwned](../tools/breach-intelligence/haveibeenpwned.md), [h8mail](../tools/breach-intelligence/h8mail.md)).

## 7. Domain / IP Intelligence

Map infrastructure using passive DNS and attack-surface tools ([Amass](../tools/domains/amass.md), [Subfinder](../tools/domains/subfinder.md), [Assetfinder](../tools/domains/assetfinder.md), [dnsx](../tools/domains/dnsx.md)) and internet-wide scan indexes ([Shodan](../tools/domains/shodan.md), [Censys](../tools/domains/censys.md)).

## 8. Image Analysis

Use reverse image search ([TinEye](../tools/images/tineye.md), [Google Lens](../tools/images/google-lens.md), [Yandex Images](../tools/images/yandex-images.md)) to find the origin, prior appearances, or context of an image.

## 9. Metadata Analysis

Extract embedded metadata (camera model, GPS coordinates, timestamps, authorship) from files using [ExifTool](../tools/metadata/exiftool.md) or [MediaInfo](../tools/metadata/mediainfo.md). Note that most social platforms strip metadata on upload — metadata is most useful on files obtained directly, not from social media.

## 10. Cross-Source Correlation

Line up findings from every step above. Look for consistent, independently-sourced overlaps (same alias + same avatar + same email domain, for example) rather than relying on any single source.

## 11. Verification

For each significant finding, ask:

- Can I confirm this through a second, unrelated source?
- Could this be a coincidence (shared name/username), a spoofed account, or stale/cached data?
- Would this finding hold up if someone else tried to reproduce it?

## 12. Documentation

Record the source, timestamp, method, and raw evidence (with screenshots/archives) for every finding that feeds into your conclusion. Undocumented findings are not reproducible and should not be relied upon.

## 13. Confidence Assessment

Grade your overall conclusion honestly, for example:

| Confidence | Meaning |
|---|---|
| **Low** | Single uncorroborated source; plausible but unconfirmed. |
| **Medium** | Multiple independent sources agree; minor gaps remain. |
| **High** | Multiple independent, authoritative sources corroborate; verified directly. |

Present findings with their confidence level attached — never present a low-confidence lead as a confirmed fact.

---

Before starting any investigation, review [OPSEC](opsec.md) and [Legal & Ethical Use](legal-and-ethical-use.md).
