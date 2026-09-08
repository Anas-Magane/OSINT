# theHarvester

**Category:** Reconnaissance

**Purpose:** Gather emails, subdomains, hosts, employee names, open ports, and banners from public sources (search engines, PGP key servers, certificate transparency, and more) about a target domain or organization.

**Official Repository:** [github.com/laramies/theHarvester](https://github.com/laramies/theHarvester)

**Status:** ✅ Active | **License:** See repository

**Installation:**

```bash
pip3 install theHarvester
# or
git clone https://github.com/laramies/theHarvester.git && cd theHarvester && pip3 install -r requirements.txt
```

**Basic Usage:**

```bash
theHarvester -d example.com -b all
```

**Example:**

```bash
theHarvester -d example.com -b crtsh,duckduckgo,bing -f report.html
```

**What it is useful for:**

- A single first pass that aggregates many passive OSINT sources for a domain.
- Building an initial map of an organization's public footprint (people, infrastructure, emails) before deeper investigation.
- Producing a shareable report for documentation.

**Limitations:**

- Quality depends entirely on the underlying source APIs — some modules require API keys for full results, and some sources rate-limit heavily.
- Results can include stale or decommissioned assets.
- Not a vulnerability scanner — it only gathers information.

**Operational Safety:**

Most modules are passive (querying third-party indexes, not the target directly). A few modules perform direct DNS lookups. Use `-b` to select only the sources you need, and treat all findings as leads requiring manual verification.
