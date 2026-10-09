# Monthly Ransomware Intelligence Briefing - September 2026

## Reporting boundary

- **Reporting period:** 1 September 2026 through 30 September 2026, UTC.
- **Evidence cut-off:** 1 October 2026, 07:09:57 UTC for the quantitative dataset; qualitative sources accessed on 1 October 2026.
- **Audience:** 1LoD operational management and Risk Committee.
- **Unit of analysis:** Distinct public data-leak-site victim claims.

## Executive readout

- September recorded **801 distinct data-leak-site victim claims across 76 groups**, a **23.1% decrease** from 1,042 claims in August using the same source, schema, date treatment, and de-duplication rules.
- The **United States represented 31.7%** of all claims. Country coverage was 88.8%; records without a stated country remained in the percentage denominator.
- **Manufacturing led reported industries with 133 claims**, followed by Professional Services with 93 and Technology with 89. Industry coverage was 79.8%.
- **thegentlemen led group activity with 102 claims**, followed by qilin with 74. The five leading groups represented 34.8% of all claims.
- September research recorded a new UMBRA ransomware assessment, continued evidence of credential and remote-access exposure, and September additions to CISA’s exploited-vulnerability catalogue. These sources do not establish that the vulnerabilities were used in the September victim-claim dataset.

## Slide data

### Top Target Countries

| Rank | Country | Victim claims | Share of all victim claims |
| ---: | --- | ---: | ---: |
| 1 | United States | 254 | 31.7% |
| 2 | Germany | 34 | 4.2% |
| 3 | Canada | 29 | 3.6% |
| 4 | United Kingdom | 28 | 3.5% |
| 5 | Brazil | 26 | 3.2% |
| 6 | Italy | 25 | 3.1% |
| 7 | India | 22 | 2.7% |
| 8 | France | 17 | 2.1% |
| 9 | Spain | 16 | 2.0% |
| 10 | Argentina | 15 | 1.9% |

### Top Target Industries

| Rank | Industry | Victim claims |
| ---: | --- | ---: |
| 1 | Manufacturing | 133 |
| 2 | Professional Services | 93 |
| 3 | Technology | 89 |
| 4 | Healthcare | 71 |
| 5 | Retail & E-Commerce | 52 |
| 6 | Financial Services | 41 |

### Top 5 Ransomware Groups

| Rank | Group | Victim claims |
| ---: | --- | ---: |
| 1 | thegentlemen | 102 |
| 2 | qilin | 74 |
| 3 | Storm | 37 |
| 4 | krybit | 34 |
| 5 | safepay | 32 |

## Analyst's Notes - Ransomware Activity

- September recorded 801 distinct public victim claims across 76 groups, representing a 23.1% decrease from August under the same source and calculation method.
- The United States remained the primary geographic target, accounting for 31.7% of all reported claims; country coverage was 88.8%.
- Manufacturing remained the most targeted reported industry with 133 claims, followed by Professional Services with 93 and Technology with 89.
- thegentlemen led reported group activity with 102 claims, while the five leading groups represented 34.8% of all reported claims.
- CYFIRMA reported UMBRA ransomware on 11 September, including file encryption and data-extortion features; the report does not establish widespread exploitation or attribution beyond the observed sample.
- **2LoD assessment:** Manufacturing concentration and supplier dependency create a concentration-risk pathway across production, logistics, and third-party services; this is an assessment, not a measured September loss.

## Method statement and limitations

> The reported metrics measure distinct public data-leak-site victim claims observed during the reporting period. They understate unpublicised events and can include duplicate, delayed, recycled, misattributed, or uncorroborated claims. They do not measure confirmed intrusions, encryption events, data exfiltration, ransom payments, financial loss, or sector-wide prevalence.

- One organisation can appear more than once where repeat posts, affiliate changes, or duplicate claims cannot be resolved from public fields.
- Country and industry values are source-provided classifications. Missing values are excluded from their respective rankings but remain in the country percentage denominator.
- Historical entries can change after collection. This dated output is the September 2026 reporting-period snapshot.
- External sources use different collection methods and are presented as context only. Their counts are not merged with the Ransomware.live metric base.

## Source register

| ID | Source | URL | Publisher | Published / retrieved date | Reporting period | Tier | Used for | Methodology / limitation |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| S-01 | Ransomware.live public victims CSV | https://data.ransomware.live/victims.csv | Ransomware.live | Retrieved 1 Oct 2026 | September 2026 | Tier 2 | Country, industry, group, and volume rankings | Passive public leak-site monitoring; victim posts are uncorroborated claims. |
| S-02 | Ransomware.live public victims CSV, prior-month rerun | https://data.ransomware.live/victims.csv | Ransomware.live | Retrieved 1 Oct 2026 | August 2026 | Tier 2 | Comparable month-over-month baseline | Same source and schema as S-01; historical records can change. |
| S-03 | Ransomware roundup: August 2026 | https://www.comparitech.com/news/ransomware-roundup-august-2026/ | Comparitech | Updated 8 Sep 2026 | August 2026 | Tier 2 | External benchmark and group context | 997 recorded claims, of which 77 were confirmed by the entity involved; different collection method from S-01. |
| S-04 | Weekly Intelligence Report - 11 Sep 2026 | https://www.cyfirma.com/?post_type=news&p=62033 | CYFIRMA | Published 11 Sep 2026 | September 2026 | Tier 2 | UMBRA development | Threat-discovery report based on public and underground monitoring; sample evidence does not establish prevalence or attribution. |
| S-05 | Known Exploited Vulnerabilities Catalog | https://www.cisa.gov/known-exploited-vulnerabilities-catalog | CISA | Accessed 1 Oct 2026 | September 2026 additions | Tier 1 | Operational vulnerability context | September entries show exploitation status as unknown for the cited examples; catalogue inclusion does not establish ransomware use. |
| S-06 | BOD 26-04: Prioritizing Security Updates Based on Risk | https://www.cisa.gov/news-events/directives/bod-26-04-prioritizing-security-updates-based-risk | CISA | Published 10 Jun 2026 | Current guidance | Tier 1 | Risk translation for exposed assets | Binding guidance applies to U.S. federal agencies; enterprise implications are an assessment, not a direct regulatory obligation for all firms. |
| S-07 | 2026 Manufacturing & Distribution Ransomware Report | https://blackkite.com/reports/2026-manufacturing-distribution | Black Kite Research Group | Report period Jan 2023-Jul 2026; accessed 1 Oct 2026 | Jan 2023-Jul 2026 | Tier 2 | Manufacturing and supplier-concentration context | Publicly disclosed incidents and external exposure indicators; not a September-only dataset. |

## Claim ledger

| Claim ID | Claim text | Classification | Source IDs | Locator / calculation | Confidence rationale | Limitation |
| --- | --- | --- | --- | --- | --- | --- |
| C-01 | September recorded 801 distinct public victim claims across 76 groups. | Observed activity | S-01 | `metrics_2026_09.json` totals | Direct calculation from retained September extract. | Leak-site claims do not confirm incident outcomes. |
| C-02 | September claims decreased 23.1% from August. | Observed activity | S-01, S-02 | `(801 / 1042) - 1` | Same source, schema, timestamp treatment, and de-duplication rules. | Historical source records may be backfilled or amended. |
| C-03 | The United States represented 31.7% of all claims. | Observed activity | S-01 | 254 / 801 | Direct source-field calculation. | 11.2% of claims had no stated country and remained in the denominator. |
| C-04 | Manufacturing led reported industries with 133 claims. | Observed activity | S-01 | Ranked `activity` field | Direct source-field count. | Industry coverage was 79.8%; labels are source-provided. |
| C-05 | thegentlemen led group activity with 102 claims; the top five represented 34.8%. | Observed activity | S-01 | Ranked `group_name` field | Direct source-field count and concentration calculation. | Group names and aliases are not independently normalised. |
| C-06 | CYFIRMA reported UMBRA ransomware on 11 September with encryption and data-extortion features. | Observed activity | S-04 | Report section “Ransomware In Focus” | Source-supported report of observed malware characteristics. | The report does not establish widespread exploitation or attribution beyond its sample. |
| C-07 | September additions to CISA’s catalogue included unauthenticated or remote-access-relevant vulnerabilities, while the catalogue marked ransomware use as unknown for cited examples. | Observed activity | S-05 | September catalogue entries | Direct reading of catalogue fields. | Catalogue status does not establish ransomware exploitation. |
| C-08 | Manufacturing and supplier dependencies create a concentration-risk pathway. | Assessed exposure | S-01, S-07 | September manufacturing ranking plus Black Kite supplier analysis | Explicit 2LoD translation of observed concentration and contextual evidence. | This is not a measured September loss or confirmed third-party impact. |

## Quality gate

- **Period control:** PASS - `2026-09`, 1 September through 30 September 2026 UTC.
- **Metric source:** PASS - retained September extract, JSON, and slide-data Markdown.
- **Comparable baseline:** PASS - August rerun with the same source and schema.
- **Traceability:** PASS - all slide metrics and material bullets link to S-01 through S-07 and the claim ledger.
- **Language control:** PASS - no prohibited governance descriptors or em dash characters detected in this briefing.
- **Scope limitation:** PASS - external sources are contextual and not merged with S-01 counts.
- **Final status:** COMPLETE WITH LIMITATIONS.
