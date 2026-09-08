# Subfinder

**Category:** Domain / DNS / Infrastructure

**Purpose:** Fast, passive subdomain discovery tool that aggregates results from many public sources.

**Official Repository:** [github.com/projectdiscovery/subfinder](https://github.com/projectdiscovery/subfinder)

**Status:** ✅ Active (ProjectDiscovery) | **License:** MIT

**Installation:**

```bash
go install -v github.com/projectdiscovery/subfinder/v2/cmd/subfinder@latest
```

**Basic Usage:**

```bash
subfinder -d example.com
```

**Example:**

```bash
subfinder -d example.com -all -o subdomains.txt
```

**What it is useful for:**

- Quick, purely passive subdomain enumeration as a first step in infrastructure mapping.
- Feeding subdomain lists into further tooling (e.g., [dnsx](dnsx.md)) for resolution and liveness checks.
- Integrating into automated recon pipelines alongside other ProjectDiscovery tools.

**Limitations:**

- Passive-only by design — it will not find subdomains that aren't indexed anywhere publicly.
- Full source coverage (`-all`) benefits significantly from configuring free API keys for third-party sources.
- Results still require validation (a discovered subdomain may be inactive or decommissioned).

**Operational Safety:**

Subfinder is passive by default (queries public data sources, not the target directly), making it low-risk for reconnaissance. Still, only act on discovered assets within an authorized scope.
