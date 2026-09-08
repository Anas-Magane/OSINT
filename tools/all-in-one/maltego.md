# Maltego

**Category:** All-in-One

**Purpose:** Link-analysis platform that visually maps relationships between people, domains, infrastructure, and other entities using "transforms" that query data sources automatically.

**Website:** [maltego.com](https://www.maltego.com)

**Status:** ✅ Active | **License:** Proprietary — free Community Edition (CE) available; paid tiers for full transform access

**Installation:**

Download the Community Edition installer from [maltego.com/downloads](https://www.maltego.com/downloads/) (registration required).

**Basic Usage:**

Create a new graph, add a starting entity (domain, email, person, etc.), right-click to run a transform, and visually explore the resulting relationship graph.

**What it is useful for:**

- Visually correlating findings across many entities and data sources — especially valuable in the "cross-source correlation" step of the [methodology](../../docs/methodology.md).
- Presenting complex relationship findings to non-technical stakeholders via the graph view.

**Limitations:**

- The free Community Edition has usage and transform limits; full data-source access typically requires a commercial license or separate paid transform providers.
- Transform results depend on the underlying data provider's accuracy — verify key findings independently.

**Operational Safety:**

Some transforms send target data to third-party transform providers — review which providers you've enabled before running transforms on sensitive data. Keep any transform/API credentials out of shared or committed configuration files.
