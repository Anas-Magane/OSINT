# Maigret

**Category:** Username OSINT

**Purpose:** Collect a detailed profile of a username's presence across a very large number of sites, including extracted bio/page data, and generate a report.

**Official Repository:** [github.com/soxoj/maigret](https://github.com/soxoj/maigret)

**Status:** ✅ Active | **License:** MIT

**Installation:**

```bash
pip3 install maigret
```

**Basic Usage:**

```bash
maigret <username>
```

**Example:**

```bash
maigret johnsmith --html report.html
```

**What it is useful for:**

- Deeper username investigation than a simple existence check — Maigret extracts page content where possible (bio, name, links).
- Generating shareable HTML/PDF/JSON reports for documentation.
- Correlating usernames with additional recovered details (linked profiles, IDs).

**Limitations:**

- Larger site coverage means a higher chance of false positives on any given run.
- Extracted profile data can be outdated or incomplete depending on the target site's structure.
- Still requires manual verification of every meaningful hit.

**Operational Safety:**

Maigret checks hundreds of sites per run, which is more likely to trigger rate-limiting than smaller tools. Space out large runs, use a dedicated research network, and never feed the tool your own personal accounts' usernames unless that is the intended subject.
