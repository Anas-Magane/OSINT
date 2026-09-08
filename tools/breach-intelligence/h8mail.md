# h8mail

**Category:** Breach Intelligence

**Purpose:** Email OSINT and breach-hunting tool that queries multiple breach/leak data APIs (including Have I Been Pwned) to check exposure for a given email.

**Official Repository:** [github.com/khast3x/h8mail](https://github.com/khast3x/h8mail)

**Status:** ⚠️ Low activity (no recent releases) — verify individual API integrations still work | **License:** See repository

**Installation:**

```bash
pip3 install h8mail
```

**Basic Usage:**

```bash
h8mail -t target@example.com
```

**Example:**

```bash
h8mail -t target@example.com -c config.ini -o results.csv
```

**What it is useful for:**

- Aggregating breach-exposure checks across multiple providers from a single CLI.
- Bulk-checking a list of emails against configured breach APIs (with valid API keys).

**Limitations:**

- Depends on third-party API keys (HIBP, etc.) for most functionality — without them, coverage is minimal.
- Infrequent updates mean some integrations may lag behind API changes.
- Confirms exposure in leaked datasets only — does not confirm current password validity.

**Operational Safety:**

Store all API keys via environment variables or a config file excluded from version control — never commit them (see [`.gitignore`](../../.gitignore) and [SECURITY.md](../../SECURITY.md)). Use exposure findings only for legitimate defensive purposes (e.g., notifying an org of compromised accounts), never to attempt logins.
