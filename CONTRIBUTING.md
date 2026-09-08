# Contributing to Aramon OSINT

Thank you for helping improve this resource. Contributions are welcome from beginners and experienced researchers alike — this guide explains how to contribute effectively.

## Ways to Contribute

- **Add a new tool** to an existing category (or propose a new category if none fits).
- **Fix a broken or outdated link.**
- **Improve documentation** — clarity, accuracy, or examples in `docs/` or `resources/`.
- **Report an outdated or abandoned tool** so it can be flagged or removed.
- **Report inaccuracies** in installation steps, usage examples, or tool descriptions.

## Before You Submit: Quality Checklist

Every tool must pass this checklist before being added. Please confirm each point in your pull request description:

- [ ] The **official** repository or website exists and the URL is correct (no mirrors, no reuploads).
- [ ] The project is actively maintained, or its status is clearly marked (e.g., `⚠️ Archived / Unmaintained`).
- [ ] You know the tool's **license** (or have noted "unknown/proprietary").
- [ ] The tool is legal and safe to document (no marketplaces, stolen-data sources, credential dumps, or illegal services).
- [ ] The tool is genuinely OSINT-relevant and useful — not a near-duplicate of an existing entry without added value.
- [ ] The tool is usable without requiring or encouraging unauthorized access.

## Adding a Tool

1. Choose the correct category folder under [`tools/`](tools/).
2. Create a new Markdown file named after the tool (lowercase, hyphenated), e.g. `tools/username/new-tool.md`.
3. Use the **standard tool entry format** (see any existing entry, e.g. [`tools/username/sherlock.md`](tools/username/sherlock.md)):

   ```markdown
   # Tool Name

   **Category:** ...
   **Purpose:** ...
   **Official Repository:** [GitHub](...)
   **Website:** ...
   **Status:** Active / ⚠️ Archived / Unmaintained
   **License:** ...

   **Installation:**
   \`\`\`bash
   ...
   \`\`\`

   **Basic Usage:**
   \`\`\`bash
   ...
   \`\`\`

   **What it is useful for:**
   - ...

   **Limitations:**
   - ...

   **Operational Safety:**
   ...
   ```

4. Add a row to the [tool directory table in the README](README.md#-tool-directory), linking to your new file.
5. If relevant, cross-link the new tool from [`docs/methodology.md`](docs/methodology.md).

## Reporting Broken Links or Outdated Tools

Please open an issue with:

- The affected file/tool.
- What's wrong (broken link, archived project, replaced by a better alternative, etc.).
- A suggested fix or replacement, if you have one.

## Pull Request Guidelines

- Keep PRs focused — one tool or one fix per PR is easier to review than a large batch.
- Use clear commit messages (`docs: add <tool>`, `fix: correct broken link for <tool>`, `docs: mark <tool> as archived`).
- Do not include unrelated changes, large binaries, or personal data in a PR.
- Never include API keys, tokens, or credentials in examples — use placeholders like `YOUR_API_KEY`.

## Code of Conduct

All contributions are expected to follow the [Code of Conduct](CODE_OF_CONDUCT.md) and the [Legal & Ethical Use](docs/legal-and-ethical-use.md) policy.
