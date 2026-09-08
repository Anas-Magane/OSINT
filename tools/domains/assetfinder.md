# Assetfinder

**Category:** Domain / DNS / Infrastructure

**Purpose:** Simple command-line tool that finds domains and subdomains related to a given domain using public sources.

**Official Repository:** [github.com/tomnomnom/assetfinder](https://github.com/tomnomnom/assetfinder)

**Status:** ⚠️ Stable but infrequently updated | **License:** MIT

**Installation:**

```bash
go install github.com/tomnomnom/assetfinder@latest
```

**Basic Usage:**

```bash
assetfinder example.com
```

**Example:**

```bash
assetfinder --subs-only example.com > subdomains.txt
```

**What it is useful for:**

- A lightweight, scriptable building block in larger recon pipelines (pairs well with Unix-style piping to other tools).
- Quick passive subdomain discovery without extra configuration.

**Limitations:**

- No longer under active feature development — it does one thing well but hasn't changed in some time.
- Passive-only; coverage depends on the public sources it queries.
- Less comprehensive than Amass/Subfinder for large-scale attack surface mapping.

**Operational Safety:**

Purely passive lookups against public data sources — low risk. Combine with authorized, scoped follow-up if you resolve or probe discovered subdomains.
