# AbuseIPDB

**Category:** Threat Intelligence

**Purpose:** Community-driven database of reported abusive IP addresses (spam, brute-force, scanning, malware C2), with a confidence score based on report volume/recency.

**Website:** [abuseipdb.com](https://www.abuseipdb.com)

**Status:** ✅ Active | **License:** Free tier + paid API

**Installation:**

No installation required for manual lookups. A REST API is available for automation (free tier included).

**Basic Usage:**

Enter an IP address at [abuseipdb.com](https://www.abuseipdb.com) to view its abuse confidence score and report history.

**What it is useful for:**

- Quickly checking whether an IP has a history of reported abusive behavior.
- Triaging suspicious connection attempts in logs during incident response.
- Contributing your own abuse reports to help the community (optional).

**Limitations:**

- Community-sourced reports can include false positives, misattributions, or stale data (e.g., an IP later reassigned to a different, legitimate user via NAT/DHCP/cloud provider churn).
- A high abuse score is a signal, not proof — always corroborate with other threat-intel sources.

**Operational Safety:**

Lookups are passive (querying AbuseIPDB's database). If you report an IP yourself, avoid including sensitive internal details in the public report comment field.
