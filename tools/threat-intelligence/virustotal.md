# VirusTotal

**Category:** Threat Intelligence

**Purpose:** Aggregates dozens of antivirus engines and analysis tools to check files, URLs, domains, and IP addresses for known malicious activity.

**Website:** [virustotal.com](https://www.virustotal.com)

**Status:** ✅ Active (Google-owned) | **License:** Free tier + paid API/enterprise

**Installation:**

No installation required for manual lookups. A REST API is available for automation (requires a free or paid API key).

**Basic Usage:**

Submit a file, URL, domain, or IP at [virustotal.com](https://www.virustotal.com) and review the aggregated verdicts.

**What it is useful for:**

- Quickly checking whether a file hash, URL, domain, or IP is flagged as malicious by multiple vendors.
- Historical relationship data (e.g., which domains/IPs a malicious file has communicated with).
- A standard first step in triaging a suspicious indicator during incident response.

**Limitations:**

- Multiple "clean" verdicts do not guarantee safety (zero-day or targeted malware may evade all engines at time of scan).
- Uploading a file makes it available to VirusTotal and its partners — do not upload confidential/proprietary or sensitive files.
- Free-tier API has strict rate limits.

**Operational Safety:**

Prefer submitting a hash or URL over uploading the full file when the file might be sensitive — VirusTotal shares uploaded samples with its partner ecosystem. Keep API keys out of source control.
