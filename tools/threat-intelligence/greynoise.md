# GreyNoise

**Category:** Threat Intelligence

**Purpose:** Identifies internet "background noise" — IPs performing mass scanning/opportunistic activity — helping analysts distinguish targeted attacks from routine internet scanning.

**Website:** [greynoise.io](https://www.greynoise.io)

**Status:** ✅ Active | **License:** Free community tier + paid plans/API

**Installation:**

No installation required for manual lookups via the [GreyNoise Visualizer](https://viz.greynoise.io). A REST API and CLI are available for automation.

**Basic Usage:**

Look up an IP at [viz.greynoise.io](https://viz.greynoise.io) to see whether it's classified as internet-wide scanning noise, a known benign service (e.g., a search engine crawler), or unclassified.

**What it is useful for:**

- Filtering out routine mass-scanning noise when triaging firewall/IDS alerts, so analysts can focus on targeted activity.
- Confirming whether an IP hitting your infrastructure is a known benign crawler/scanner versus unclassified/suspicious.

**Limitations:**

- Classification reflects GreyNoise's own sensor network visibility — an IP can be unclassified simply because it hasn't been observed yet, not because it's safe.
- Free community tier has limited query volume and data depth compared to paid plans.

**Operational Safety:**

Lookups are passive queries against GreyNoise's own dataset — no interaction with the queried IP's owner.
