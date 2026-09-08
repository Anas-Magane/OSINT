# URLScan.io

**Category:** Threat Intelligence

**Purpose:** Submits a URL to an automated, sandboxed browser that records the full page load — screenshots, network requests, DOM, redirects, and detected technologies — for security analysis.

**Website:** [urlscan.io](https://urlscan.io)

**Status:** ✅ Active | **License:** Free tier + paid API/enterprise

**Installation:**

No installation required for manual scans. An API is available for automation (free tier included).

**Basic Usage:**

Submit a URL at [urlscan.io](https://urlscan.io) and review the resulting scan report (screenshot, requests, indicators).

**What it is useful for:**

- Safely observing what a suspicious URL actually does (redirects, scripts, embedded resources) without visiting it yourself.
- Investigating phishing pages, malicious redirects, or unfamiliar infrastructure.
- Historical search across previously submitted scans for related indicators.

**Limitations:**

- Public scans are, by default, visible to other URLScan users — use "private" or "unlisted" visibility for sensitive submissions.
- The sandbox may not trigger content that requires specific conditions (geolocation, login state, user interaction) to activate.

**Operational Safety:**

Never submit a URL containing sensitive tokens/session identifiers in "public" mode — it becomes visible to others. Use unlisted/private scanning for anything tied to an active, non-public investigation.
