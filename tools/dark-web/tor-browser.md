# Tor Browser

**Category:** Dark Web / Onion Research

**Purpose:** The official, hardened browser for accessing the Tor network, including `.onion` sites, with built-in anti-fingerprinting and traffic-routing protections.

**Official Website:** [torproject.org](https://www.torproject.org)

**Official Repository:** [gitlab.torproject.org/tpo/applications/tor-browser](https://gitlab.torproject.org/tpo/applications/tor-browser)

**Status:** ✅ Active | **License:** Open source (see repository)

**Installation:**

Download only from the official site: [torproject.org/download](https://www.torproject.org/download/). Verify the signature/checksum before running, as fake Tor Browser downloads are a known distribution vector for malware.

**Basic Usage:**

Launch Tor Browser and browse as normal; it automatically routes traffic through the Tor network.

**What it is useful for:**

- Legitimate research into onion-hosted content (research, journalism, threat intelligence) without directly exposing your IP to the destination server.
- Accessing legitimate onion mirrors that some organizations (e.g., news outlets, privacy-focused services) provide for censorship resistance.

**Limitations:**

- Does not anonymize you if you log into personal accounts or reveal identifying information within pages.
- Exit-node traffic for non-onion (clearnet) destinations can, in principle, be observed by exit-node operators for unencrypted traffic — always use HTTPS.
- Performance is slower than a regular browser due to onion routing.

**Operational Safety:**

Do not resize the Tor Browser window (it's fingerprintable), do not install extensions, and do not open downloaded files while still connected. Review the full [OPSEC guide](../../docs/opsec.md#understand-tor-limitations) before conducting onion research. Only access legal content — see [Legal & Ethical Use](../../docs/legal-and-ethical-use.md#a-note-on-dark-web--onion-research).
