# Amass

**Category:** Domain / DNS / Infrastructure

**Purpose:** In-depth attack surface mapping and asset discovery through DNS enumeration, scraping, certificate transparency logs, and multiple OSINT data sources.

**Official Repository:** [github.com/owasp-amass/amass](https://github.com/owasp-amass/amass) (OWASP project)

**Status:** ✅ Active | **License:** See repository (Apache-2.0 family / OWASP terms)

**Installation:**

```bash
# via Go
go install -v github.com/owasp-amass/amass/v4/...@master

# or download a release binary from the GitHub Releases page
```

**Basic Usage:**

```bash
amass enum -d example.com
```

**Example:**

```bash
amass enum -passive -d example.com -o subdomains.txt
```

**What it is useful for:**

- Comprehensive passive and active subdomain/asset enumeration for attack-surface mapping.
- Aggregating data from many public sources (certificate transparency, DNS, web archives) in one workflow.
- Building a visual/graph model of an organization's external footprint.

**Limitations:**

- Active enumeration mode performs direct DNS/network requests against the target's infrastructure — it is not purely passive.
- Large scans can take significant time and produce a high volume of data that still needs triage.
- Some data sources require API keys for full coverage.

**Operational Safety:**

Use `-passive` mode when you need zero direct interaction with the target's infrastructure. Active enumeration (brute-forcing, resolution, port checks) should only be run against assets you are authorized to test — see [Legal & Ethical Use](../../docs/legal-and-ethical-use.md).
