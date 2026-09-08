# Google Dorking (Advanced Search Operators)

**Category:** Search Engines

**Purpose:** Use advanced search operators to surface specific, often unindexed-by-default content — exposed documents, login portals, specific file types, or site-restricted results.

**Website:** [google.com](https://www.google.com) (technique applies to most major search engines)

**Status:** ✅ Always current (it's a technique, not software) | **License:** N/A

**Basic Usage:**

Common operators:

```text
site:example.com               # restrict results to a domain
filetype:pdf                   # restrict to a file type
intitle:"index of"             # find pages with a specific title
inurl:admin                    # find URLs containing a keyword
"exact phrase"                 # exact phrase match
-excludeword                   # exclude a term
```

**Example:**

```text
site:example.com filetype:pdf confidential
```

**What it is useful for:**

- Finding publicly indexed but hard-to-browse-to documents, configuration files, or portals belonging to a target domain.
- Narrowing broad searches to a specific site, file type, or phrase during any OSINT phase.
- A zero-cost, zero-installation starting technique for almost any investigation.

**Limitations:**

- Only surfaces content the search engine has actually indexed — recently published or `robots.txt`-blocked content won't appear.
- Operator support and syntax vary slightly between search engines (Google, Bing, DuckDuckGo, Brave).
- Aggressive automated dorking against a single search engine can trigger CAPTCHA challenges or temporary blocks.

**Operational Safety:**

This is a fully passive technique — it queries the search engine's index, not the target. However, clicking through to a discovered result *is* an interaction with the target's server; review cached/snippet previews first when possible. See the general [search engines resource list](../../resources/search-engines.md) for more engines and their dork syntax differences.
