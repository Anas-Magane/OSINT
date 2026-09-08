# Sherlock

**Category:** Username OSINT

**Purpose:** Search for a username across hundreds of public platforms to find where an account with that handle exists.

**Official Repository:** [github.com/sherlock-project/sherlock](https://github.com/sherlock-project/sherlock)

**Status:** ✅ Active | **License:** MIT

**Installation:**

```bash
pip3 install sherlock-project
```

**Basic Usage:**

```bash
sherlock <username>
```

**Example:**

```bash
sherlock johnsmith --timeout 10 --print-found
```

**What it is useful for:**

- Discovering which platforms have an account under a given username.
- Building an initial list of candidate accounts for further manual verification.
- Fast, broad, passive first pass in a username-based investigation.

**Limitations:**

- False positives are possible (some sites return "found" for placeholder/default pages).
- A positive result does not prove account ownership by a specific person — usernames are often reused by unrelated people.
- Site layout changes can break individual site checks until the project updates its detection rules.
- Results must be manually verified by visiting the profile directly.

**Operational Safety:**

Sherlock's checks are largely passive HTTP requests to each platform, but running it repeatedly and rapidly against many sites can trigger rate-limiting or temporary IP blocks. Use a research network/identity separate from your personal one (see [OPSEC](../../docs/opsec.md)), and avoid unnecessary repeat runs against the same targets.
