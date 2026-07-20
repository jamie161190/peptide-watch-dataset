# The Peptide Watch — UK research-peptide vendor audit (open dataset)

Independent audit of every identifiable UK research-peptide website, recording whether each publishes its **own verifiable Janoshik certificate of analysis (COA)** — a report from the independent laboratory Janoshik Analytical that names the vendor itself as the client and can be checked on Janoshik's own website.

**Headline finding:** Just **9%** of active UK research-peptide sellers (29 of 325 audited) publish their own verifiable independent lab certificate. The other 91% show none, a borrowed one, a self-made one, or one that cannot be verified. (427 domains audited in total, including sites now dead or off-scope.)

- **Source of record:** https://thepeptidewatch.com
- **Live dataset (always current):** https://thepeptidewatch.com/data/vendors.json
- **Methodology:** https://thepeptidewatch.com/methodology
- **Licence:** CC BY 4.0 — free to use with attribution to *The Peptide Watch* (https://thepeptidewatch.com)

## What's in `vendors.json`

A JSON object with a `headline_finding`, summary counts, and a `vendors` array. Each vendor record:

| field | meaning |
|---|---|
| `domain` | vendor website |
| `company` | brand/company name |
| `verdict` | `verified` (own verifiable Janoshik COA) or `watch` (not) |
| `lab` | testing lab named on the COA, if any |
| `coa_date` | date on the certificate shown |
| `coa_type` | `janoshik-genuine` / `borrowed` / `self-made` / `analiza` / etc. |
| `coa_client` | the company named as the client on the certificate |
| `trustpilot_score`, `trustpilot_reviews` | Trustpilot data where found |
| `advertising_on_google` | boolean, if confirmed |
| `bpc157_gbp_per_mg` | BPC-157 price benchmark (£/mg) where available |
| `audit_url` | full per-vendor audit page |

## Independence

The Peptide Watch sells no peptides, takes no payment from any vendor to appear or be removed, and links to no vendor's shop. Every field states an observable fact from the vendor's own website, the certificate it published, or the public record.

**Important scope note:** this evaluates the *credibility of a seller's evidence*, not the product. No dataset or document can prove what is in a specific vial you receive — only independently testing that exact unit can. It reduces uncertainty; it does not eliminate risk.

## Citation

> The Peptide Watch (2026). *UK research-peptide vendor audit.* https://thepeptidewatch.com/data/vendors.json (CC BY 4.0)
