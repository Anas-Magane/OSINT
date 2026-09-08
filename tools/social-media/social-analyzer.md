# Social-Analyzer

**Category:** Social Media OSINT

**Purpose:** Analyze and find a person's presence across social media and websites using username, name, or other identifiers, with a web UI, API, and CLI.

**Official Repository:** [github.com/qeeqbox/social-analyzer](https://github.com/qeeqbox/social-analyzer)

**Status:** ✅ Active | **License:** AGPL-3.0

**Installation:**

```bash
pip3 install social-analyzer
```

**Basic Usage:**

```bash
social-analyzer --username "johnsmith" --output web_html
```

**Example:**

```bash
social-analyzer --username "johnsmith" --top 25 --output json
```

**What it is useful for:**

- Broad social-media presence discovery, complementing username-only tools like [Sherlock](../username/sherlock.md) with additional analysis modes (name-based, web-page detection modules).
- Generating structured reports for documentation.

**Limitations:**

- Large detection surface means more false positives to manually filter.
- Some detection modules rely on page-content heuristics that can break when a platform changes its layout.

**Operational Safety:**

Runs many requests against many platforms — expect possible rate-limiting. Use a research identity/network and avoid running it against your own or others' accounts without authorization.

---

> **Note on historical tools:** Several once-popular platform-specific scrapers for X/Twitter (e.g., Twint) have stopped working and are archived due to platform API/policy changes, and are intentionally not listed here. Always check a tool's maintenance status before relying on it — see the [tool directory](../../README.md#-tool-directory) for current status flags.
