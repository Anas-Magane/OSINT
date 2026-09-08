# Wordlists for OSINT & Recon

Wordlists are primarily used alongside domain/infrastructure enumeration tools (e.g., subdomain brute-forcing). Use them only against assets you are authorized to test.

| Wordlist | Source | Use Case |
|---|---|---|
| SecLists | [github.com/danielmiessler/SecLists](https://github.com/danielmiessler/SecLists) | Large, categorized collection (subdomains, usernames, passwords-for-testing, fuzzing payloads). The de facto standard reference collection. |
| commonspeak2 | [github.com/assetnote/commonspeak2-wordlists](https://github.com/assetnote/commonspeak2-wordlists) | Wordlists generated from real-world data (BigQuery-derived), useful for subdomain/content discovery. |
| jhaddix's all.txt | Referenced within SecLists / recon community write-ups | Popular consolidated subdomain wordlist for brute-force enumeration. |

**Operational Safety:** Brute-force enumeration (subdomains, directories, usernames) is an **active** technique that sends a high volume of requests to target infrastructure. Only run it within an authorized scope and at a reasonable rate — see [OPSEC](../docs/opsec.md) and [Legal & Ethical Use](../docs/legal-and-ethical-use.md).

---

See also: [Domain / DNS / Infrastructure tools](../tools/domains/), [Methodology](../docs/methodology.md).
