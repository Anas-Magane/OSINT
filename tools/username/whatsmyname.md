# WhatsMyName

**Category:** Username OSINT

**Purpose:** A community-maintained, open dataset (and web tool) of website username-check signatures, used to determine whether a username is registered on a given site.

**Official Repository:** [github.com/WebBreacher/WhatsMyName](https://github.com/WebBreacher/WhatsMyName)

**Website:** [whatsmyname.app](https://whatsmyname.app)

**Status:** ✅ Active | **License:** See repository

**Installation:**

The web version requires no installation. To use the underlying dataset with other tools or your own scripts:

```bash
git clone https://github.com/WebBreacher/WhatsMyName.git
```

**Basic Usage:**

Visit [whatsmyname.app](https://whatsmyname.app) and enter a username, or point a compatible OSINT tool at the project's `wmn-data.json` signature file.

**What it is useful for:**

- A well-vetted, actively curated signature dataset that many other username tools rely on.
- Manually spot-checking a username on specific sites of interest.
- Understanding exactly how a "match" is detected for a given site (transparent, open methodology).

**Limitations:**

- Coverage is limited to sites included in the dataset.
- Same false-positive caveats as any username-existence checker — a match is not proof of ownership.

**Operational Safety:**

The hosted web tool sends your query to whatsmyname.app's infrastructure; avoid entering usernames tied to sensitive, non-public investigations if that's a concern — consider running the dataset locally against a self-hosted checker instead.
