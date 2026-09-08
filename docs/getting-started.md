# Getting Started with OSINT

This guide is the entry point for anyone new to Open Source Intelligence (OSINT). It assumes no prior background and builds toward the practical workflow used throughout this repository. For a deeper, structured walkthrough, see the [Aramon OSINT Guide](OSINT_Guide_Aramon.pdf).

## What is OSINT?

**Open Source Intelligence (OSINT)** is the practice of collecting and analyzing information from publicly available sources — websites, search engines, social media, public records, DNS data, code repositories, images, and more — to answer a specific question or support an investigation.

"Open source" here does not mean open-source software. It means the source of information is legally and publicly accessible, without hacking, social engineering, or unauthorized access.

OSINT is used across many fields:

- Cybersecurity (attack surface mapping, threat intelligence, incident response)
- Journalism and fact-checking
- Due diligence and fraud investigation
- Law enforcement (within legal authorization)
- Personal digital footprint audits

## Passive vs. Active OSINT

| Type | Description | Risk of Detection | Examples |
|---|---|---|---|
| **Passive** | Information is gathered without any direct interaction with the target (no requests sent to their systems/accounts). | Very low | Search engine queries, WHOIS lookups, cached pages, public records |
| **Active** | Information gathering involves direct interaction with target-owned systems (visiting a site, sending a request, following an account). | Present | Visiting a target's website, port scanning, sending a connection request |

For most reconnaissance work, **default to passive techniques first**. Escalate to active techniques only when authorized and necessary, and understand that active steps can be logged and can alert the target.

## Basic Methodology (Overview)

A professional OSINT investigation typically follows a structured loop rather than random searching:

1. Define what you are trying to find out.
2. Gather known starting points (a name, email, domain, username, image).
3. Expand passively across multiple independent sources.
4. Correlate findings across sources.
5. Verify before trusting.
6. Document as you go.

The full workflow is detailed in [methodology.md](methodology.md).

## Verification

A single data point is not evidence — it's a lead. Before treating any finding as reliable:

- Confirm it independently through at least one other, unrelated source.
- Check whether the information could be outdated, spoofed, or coincidental (e.g., a common name/username shared by unrelated people).
- Distinguish between what a source *states* and what is *independently confirmed*.

## Source Evaluation

Not all sources are equally trustworthy. When evaluating a source, consider:

- **Authoritativeness** — Is this the platform/organization itself, or a third-party mirror/aggregator?
- **Freshness** — When was this data last updated? Cached or archived data can be stale.
- **Bias/motive** — Does the source have an incentive to mislead (marketing pages, unmoderated forums)?
- **Corroboration** — Do independent sources agree?

## False Positives

Many OSINT tools (especially username enumeration tools) report matches based on HTTP status codes or page heuristics, not confirmed identity. Expect:

- Placeholder or default pages being misidentified as "account exists."
- Common usernames matching unrelated people.
- Rate-limiting or blocking producing misleading results.

**A tool result is a hypothesis, not a conclusion.** Always manually verify important findings by visiting the source directly.

## Documentation

Keep a research log as you work:

- What you searched for and when.
- Which tool/source produced each finding.
- Screenshots or archived copies of key evidence (with timestamps).
- Your confidence level for each finding (see [methodology.md](methodology.md#13-confidence-assessment)).

Good documentation is what turns raw search results into a defensible, reproducible investigation.

## OPSEC Basics

Before you start searching, understand what your own activity exposes. At minimum:

- Use a research browser profile separate from your personal accounts.
- Understand that visiting a target's site or profile can leave a trace (visible in analytics, "viewed your profile" notifications, etc.).
- Never upload sensitive material to unfamiliar third-party tools.

The full guide is in [opsec.md](opsec.md).

## Next Steps

- Read the [Methodology](methodology.md) for a full step-by-step workflow.
- Read [OPSEC](opsec.md) before doing any active lookups.
- Read [Legal & Ethical Use](legal-and-ethical-use.md) — required reading before using anything in this repository.
- Browse the [tool categories](../README.md#-tool-directory) to find the right tool for your task.
- Download the companion [Aramon OSINT Guide (PDF)](OSINT_Guide_Aramon.pdf).
