# Recon-ng

**Category:** Automation / All-in-One

**Purpose:** Modular, Metasploit-style web reconnaissance framework with a large marketplace of modules for passive and active OSINT collection.

**Official Repository:** [github.com/lanmaster53/recon-ng](https://github.com/lanmaster53/recon-ng)

**Status:** ⚠️ Low activity (no recent releases) — core framework still functional; verify individual module status | **License:** GPL-3.0

**Installation:**

```bash
git clone https://github.com/lanmaster53/recon-ng.git
cd recon-ng
pip3 install -r REQUIREMENTS
./recon-ng
```

**Basic Usage:**

```text
[recon-ng][default] > marketplace install all
[recon-ng][default] > workspaces create example
[recon-ng][example] > modules load recon/domains-hosts/hackertarget
[recon-ng][example][hackertarget] > options set SOURCE example.com
[recon-ng][example][hackertarget] > run
```

**What it is useful for:**

- A structured, database-backed workflow for organizing recon findings (hosts, contacts, credentials-exposure indicators) across a long-running engagement.
- Access to a large module marketplace covering many data sources in one framework.

**Limitations:**

- Some modules rely on third-party APIs that may have changed since the module was last updated.
- Framework itself has seen infrequent core updates — test modules before relying on them for critical work.

**Operational Safety:**

Review each module before running it — some perform active lookups against target infrastructure. Store any required API keys in the framework's key store, never hard-coded in scripts.
