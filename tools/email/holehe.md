# Holehe

**Category:** Email OSINT

**Purpose:** Check whether an email address is registered on various online services, by abusing "forgot password" / registration endpoints that leak account existence.

**Official Repository:** [github.com/megadose/holehe](https://github.com/megadose/holehe)

**Status:** ⚠️ Low activity (no recent releases) — still functional as of last verification | **License:** GPL-3.0

**Installation:**

```bash
pip3 install holehe
```

**Basic Usage:**

```bash
holehe target@example.com
```

**Example:**

```bash
holehe target@example.com --only-used
```

**What it is useful for:**

- Quickly determining which platforms an email address is associated with.
- Supporting email-based identity correlation as part of a wider investigation.

**Limitations:**

- Relies on third-party endpoint behavior that can change or be patched without notice, breaking individual modules.
- A "registered" result confirms an account exists for that email, not who controls it.
- Project shows infrequent updates — verify individual module results manually.

**Operational Safety:**

Holehe queries live third-party services directly using the target email. This is a form of active reconnaissance — it can, in principle, trigger security notifications on some platforms (e.g., "someone tried to reset your password"). Use judiciously and only within an authorized scope.
