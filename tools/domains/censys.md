# Censys

**Category:** Domain / DNS / Infrastructure

**Purpose:** Internet-wide scanning and asset search platform, similar in purpose to Shodan, with strong certificate and host-attribution data.

**Website:** [censys.com](https://censys.com)

**CLI / Library:** [github.com/censys/censys-python](https://github.com/censys/censys-python)

**Status:** ✅ Active | **License:** Free tier + paid plans; library is open source (Apache-2.0)

**Installation:**

```bash
pip3 install censys
censys config
```

**Basic Usage:**

```bash
censys search "services.service_name: HTTP"
```

**Example:**

```bash
censys hosts search "example.com" --index-type hosts
```

**What it is useful for:**

- Certificate transparency search and host attribution for attack-surface discovery.
- Cross-referencing Shodan findings with an independent internet-scan dataset.
- Identifying organizational assets via TLS certificate metadata.

**Limitations:**

- Free tier has strict query limits.
- Like Shodan, data reflects Censys' own scan cadence, not real-time state.

**Operational Safety:**

Passive from the target's perspective (Censys performs the scanning, not you). Do not use discovered exposure to attempt unauthorized access. Protect your API credentials.
