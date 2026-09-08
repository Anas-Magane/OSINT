# dnsx

**Category:** Domain / DNS / Infrastructure

**Purpose:** Fast and multi-purpose DNS toolkit for resolving hosts, checking liveness, and retrieving multiple DNS record types at scale.

**Official Repository:** [github.com/projectdiscovery/dnsx](https://github.com/projectdiscovery/dnsx)

**Status:** ✅ Active (ProjectDiscovery) | **License:** MIT

**Installation:**

```bash
go install -v github.com/projectdiscovery/dnsx/cmd/dnsx@latest
```

**Basic Usage:**

```bash
echo example.com | dnsx
```

**Example:**

```bash
cat subdomains.txt | dnsx -a -resp -o resolved.txt
```

**What it is useful for:**

- Resolving large subdomain lists (from Subfinder/Amass/Assetfinder) to confirm which are actually live.
- Retrieving specific DNS record types (A, AAAA, CNAME, MX, TXT, etc.) at scale.
- A standard pipeline step between subdomain discovery and further probing.

**Limitations:**

- Requires an input list (it's a resolver/prober, not a discovery tool by itself).
- DNS resolution is a direct query to DNS infrastructure — technically active, though extremely lightweight and standard internet behavior.

**Operational Safety:**

DNS resolution itself is normal, low-impact internet activity, but running very large, rapid batches can look like scanning traffic to some monitoring systems. Rate-limit large jobs and stay within your authorized scope.
