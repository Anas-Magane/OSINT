# Have I Been Pwned (HIBP)

**Category:** Breach Intelligence

**Purpose:** The canonical, widely trusted service for checking whether an email address or phone number has appeared in a known, publicly-disclosed data breach.

**Website:** [haveibeenpwned.com](https://haveibeenpwned.com)

**Status:** ✅ Active | **License:** Free web lookup; paid API for bulk/automated use

**Installation:**

No installation required for manual lookups. For programmatic use, an API key is required — see the site's API documentation.

**Basic Usage:**

Visit [haveibeenpwned.com](https://haveibeenpwned.com) and enter an email address to see which breaches it appears in.

**What it is useful for:**

- Authoritative, well-maintained breach-exposure checking for an email address.
- A trustworthy baseline that other tools (like [h8mail](h8mail.md)) build on via its API.
- Personal digital-hygiene checks (has *your own* email been breached?).

**Limitations:**

- Only reflects breaches HIBP has ingested and verified — it is not a complete record of every breach that has ever occurred.
- A breach listing shows an email was present in a leaked dataset; it does not by itself reveal passwords or other leaked fields (those require the paid API/domain-verified access, with appropriate safeguards).

**Operational Safety:**

Checking an email is passive from the target's perspective (you're querying HIBP's database, not the email owner). Do not use this service to build lists for credential-stuffing or unauthorized access attempts — that is illegal and outside the scope of this repository.
