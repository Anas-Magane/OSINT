# Shodan

**Category:** Domain / DNS / Infrastructure

**Purpose:** Search engine for internet-connected devices and services — indexes banners, open ports, and metadata from internet-wide scans.

**Website:** [shodan.io](https://www.shodan.io)

**CLI / Library:** [github.com/achillean/shodan-python](https://github.com/achillean/shodan-python)

**Status:** ✅ Active (service) | **License:** Free tier + paid plans; library is open source

**Installation:**

```bash
pip3 install shodan
shodan init YOUR_API_KEY
```

**Basic Usage:**

```bash
shodan search "apache country:MA"
```

**Example:**

```bash
shodan host 8.8.8.8
```

**What it is useful for:**

- Discovering internet-exposed devices/services associated with an organization (as part of authorized attack-surface assessment).
- Identifying exposed, potentially misconfigured services (databases, cameras, industrial control systems) for defensive remediation.
- Historical banner/service data without directly scanning the target yourself.

**Limitations:**

- Data reflects Shodan's own scan schedule and may be out of date at query time.
- Free-tier API access is limited in query volume and result depth.
- Finding an exposed service does not by itself indicate a vulnerability — further authorized verification is required.

**Operational Safety:**

Shodan itself performs the internet-wide scanning, so querying it does not directly touch the target — it is a passive way to see what's already publicly exposed. Do not use findings to attempt access to systems you are not authorized to test. Keep your API key out of source control.
