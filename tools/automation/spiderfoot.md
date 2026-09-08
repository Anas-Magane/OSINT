# SpiderFoot

**Category:** Automation / All-in-One

**Purpose:** Automated OSINT reconnaissance framework that queries over 200 public data sources to map an organization's attack surface — domains, IPs, emails, usernames, and more — from a single target.

**Official Repository:** [github.com/smicallef/spiderfoot](https://github.com/smicallef/spiderfoot)

**Website:** [spiderfoot.net](https://www.spiderfoot.net)

**Status:** ✅ Active | **License:** MIT

**Installation:**

```bash
git clone https://github.com/smicallef/spiderfoot.git
cd spiderfoot
pip3 install -r requirements.txt
python3 sf.py -l 127.0.0.1:5001
```

**Basic Usage:**

Open the web UI at `http://127.0.0.1:5001`, create a new scan, enter a target (domain, IP, email, etc.), and select a scan profile.

**Example (CLI):**

```bash
python3 sf.py -s example.com -u all -o csv
```

**What it is useful for:**

- Automating the "passive discovery" phase of the [methodology](../../docs/methodology.md) across many modules at once.
- Producing a consolidated, correlated report (entity graph) rather than manually running dozens of separate tools.
- Continuous/scheduled monitoring of an organization's external footprint.

**Limitations:**

- Full-coverage scans ("all" modules) can be noisy and include some active-interaction modules — review module selection before running.
- Many modules benefit significantly from configuring third-party API keys.
- Volume of results requires triage; not every hit is significant.

**Operational Safety:**

Use scan profiles/module selection to stay strictly passive when required. Some modules perform active checks (e.g., port scans) — only enable those within an authorized scope. Review the [Legal & Ethical Use](../../docs/legal-and-ethical-use.md) guide before running broad scans against any target.
