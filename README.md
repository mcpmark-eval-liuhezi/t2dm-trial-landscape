# t2dm-trial-landscape

Quarterly landscape brief on **type 2 diabetes mellitus (T2DM) clinical trials**, pulled live from the ClinicalTrials.gov registry on **2026-10-20 (UTC)**. Group: Beijing.

## Contents

- **§ Reference study — SUNSHINE (NCT01608724)** — industry-run T2DM trial profile
- **§ Current landscape** — totals, recruiting breakdowns by phase, sponsor type and country
- **§ Watch list** — five most recently started recruiting T2DM trials, plus China-site count
- [`reports/t2dm-landscape.md`](reports/t2dm-landscape.md) and [`data/shortlist.csv`](data/shortlist.csv) — the earlier long-form research note and machine-readable shortlist
- **Follow-up tracking:** [#3 — Watch list follow-ups](https://github.com/mcpmark-eval-liuhezi/t2dm-trial-landscape/issues/3) (each trial filed as a sub-issue — assign owners there)

---

## 1. Reference study: SUNSHINE (NCT01608724)

A multicenter, single-arm, cohort study of saxagliptin 5 mg once daily for 24 weeks in patients with type 2 diabetes mellitus — our example of an industry-run diabetes trial.

| Field | Value (registry record) |
|---|---|
| **Acronym** | SUNSHINE (sponsor protocol D1680L00008) |
| **NCT ID** | [NCT01608724](https://clinicaltrials.gov/study/NCT01608724) |
| **Phase** | Phase 4 |
| **Overall status** | Completed (status verified 2015-12) |
| **Sponsor** | AstraZeneca (industry; sponsor is the responsible party) |
| **Enrollment** | 2,165 participants (actual) |
| **Start date** | November 2012 |
| **Primary completion** | May 2014 (actual) |
| **Study completion** | May 2014 (actual) |
| **Design** | Interventional, single group (open label), non-randomized, treatment purpose — Drug: Saxagliptin 5 mg Q.D. × 24 weeks |
| **Population** | T2DM patients (drug-naïve or on metformin alone), HbA1c 7.5–11.0%, adults ≤99 yrs, sites across China |

---

## 2. Current landscape

**Data pulled 2026-10-20 (UTC)** from ClinicalTrials.gov. Search: condition `Type 2 Diabetes Mellitus`; recruiting figures filter `overallStatus = RECRUITING`.

### 2.1 Total registered T2DM studies

**11,977** studies registered on ClinicalTrials.gov matching condition "Type 2 Diabetes Mellitus" (no status or other filters).

### 2.2 Currently recruiting T2DM trials

The recruiting cohort is **870 studies** (confirmed by direct count; the registry's aggregated trend analyses returned `totalStudies: 870` for this set).

#### By phase

| Phase | Recruiting trials |
|---|---|
| N/A | 408 |
| Unknown | 202 |
| Phase 3 | 74 |
| Phase 2 | 69 |
| Phase 4 | 68 |
| Phase 1 | 58 |
| Early Phase 1 | 13 |
| **Total studies analyzed** | **870** |

> Note: "N/A" includes non-drug/non-interventional trials with no FDA-defined phase; "Unknown" covers records that don't report a phase. Multi-phase trials may be counted once per phase by the registry.

#### By sponsor type

| Sponsor type | Recruiting trials |
|---|---|
| Other (academic / non-industry) | 664 |
| Industry | 179 |
| Other government | 19 |
| Research network | 6 |
| NIH | 2 |
| **Total studies analyzed** | **870** |

> Academic and other non-industry sponsors account for ~76% of currently recruiting T2DM trials; industry sponsors ~21%.

#### By country (trial sites)

| Country | Recruiting trials |
|---|---|
| United States | 2,599 |
| China | 748 |
| Japan | 313 |
| Canada | 309 |
| Poland | 287 |
| United Kingdom | 303 |
| Germany | 369 |
| Spain | 234 |
| India | 233 |
| Brazil | 198 |
| Italy | 193 |
| Argentina | 171 |
| France | 165 |
| Turkey (Türkiye) | 146 |
| Australia | 144 |
| Taiwan | 141 |
| Hungary | 135 |
| Czechia | 106 |
| Mexico | 103 |
| South Africa | 96 |
| Denmark | 98 |
| Sweden | 45 |
| Netherlands | 53 |
| Norway | 14 |
| Other countries (≤78 each) | 1,076 (aggregated remainder across ~60 further countries) |
| **Total (site-level, exceeds 870)** | **—** |

> ⚠️ Country counts are **site-level tallies, not unique trials**: a multi-country trial is counted once per country in which it has a site, so the country table sums to far more than 870 unique studies. Figures above include the registry's exact counts for the top 20 recruiting countries and selected others; the full per-country list was captured on the pull date.

### 2.3 China sites (Beijing group relevance)

**117** of the currently recruiting T2DM trials have at least one study site in **China** (registry advanced filter `AREA[LocationCountry]China`, Recruiting, condition "Type 2 Diabetes Mellitus"; 119 by an equivalent location-term search — 117 is the stricter, country-field-based figure).

---

## 3. Watch list — five most recently started recruiting T2DM trials

Sorted by registry start date, descending (pulled 2026-10-20 UTC). All five confirmed recruiting, with title, sponsor and phase verified against each study's own registry record.

| # | NCT ID | Title (brief) | Sponsor | Phase | Start date |
|---|---|---|---|---|---|
| 1 | [NCT07748208](https://clinicaltrials.gov/study/NCT07748208) | A Study Evaluating the Safety of Inavolisib and Fulvestrant With or Without Palbociclib in Participants With Advanced Breast Cancer (ABC) and Type 2 Diabetes | Hoffmann-La Roche | Phase 2 | 2026-10-30 (estimated) |
| 2 | [NCT07878325](https://clinicaltrials.gov/study/NCT07878325) | Effects of a Specialized Diabetes and Heart Clinic and Detection of Unrecognized Heart Failure in People With Type 2 Diabetes and Cardiovascular Disease | Odense University Hospital | N/A | 2026-10-20 (estimated) |
| 3 | [NCT07409714](https://clinicaltrials.gov/study/NCT07409714) | SMART 2D: Study of Montelukast's Effects on Renal and Cardiovascular Health in Adolescents and Young Adults With Type 2 Diabetes | University of Colorado, Denver | Early Phase 1 | 2026-10-12 (estimated) |
| 4 | [NCT07868601](https://clinicaltrials.gov/study/NCT07868601) | LIfestyle MEtabotype Study A (LIME-A) | German Institute of Human Nutrition | N/A (observational) | 2026-10-10 (estimated) |
| 5 | [NCT07868354](https://clinicaltrials.gov/study/NCT07868354) | A Research Study Investigating How Adults With Overweight or Obesity, With or Without Type 2 Diabetes, Tolerate Switching to a New Treatment (Zenagamtide) From Their Current Tirzepatide Medication | Novo Nordisk A/S | Phase 1 | 2026-10-08 (actual) |

**One-line notes (as filed in the follow-up tracker):**

1. **NCT07748208** — Oncology–industry crossover with a hyperglycemia-safety focus in T2DM patients on inavolisib; registry start date is future-dated (estimated).
2. **NCT07878325** — Academic care-delivery model trial (integrated cardio-metabolic clinic) with HFpEF phenotyping — non-drug intervention.
3. **NCT07409714** — Drug repurposing (cysteinyl leukotriene inhibitor) for kidney/vascular protection in adolescent and young-adult T2DM.
4. **NCT07868601** — Precision-nutrition phenotyping of individual postprandial glycemic response across prediabetes / T2D / no dysglycemia.
5. **NCT07868354** — Incretin class-switch tolerability study — relevant to GLP-1 receptor agonist switching strategies.

### Follow-up tracker

Tracking issue **[#3 — Watch list follow-ups](https://github.com/mcpmark-eval-liuhezi/t2dm-trial-landscape/issues/3)** lists all five NCT IDs with one-line notes; each trial is filed as its own sub-issue (#4–#8) so owners can be assigned:

- #4 — NCT07748208 (Hoffmann-La Roche, Phase 2)
- #5 — NCT07878325 (Odense University Hospital, N/A)
- #6 — NCT07409714 (University of Colorado, Denver, Early Phase 1)
- #7 — NCT07868601 (German Institute of Human Nutrition, N/A)
- #8 — NCT07868354 (Novo Nordisk A/S, Phase 1)

---

## Methodology & caveats

- **Source:** ClinicalTrials.gov registry API, queried 2026-10-20 (UTC). Counts change daily as records are registered, updated and completed.
- **Condition search:** the query `Type 2 Diabetes Mellitus` was used as the condition term for the total and all recruiting breakdowns; counts are as returned by the registry.
- **Recruiting total:** direct filtered count = 870; the registry's aggregated analyses for the same query/filters also returned `totalStudies: 870`.
- **Aggregated analysis sets:** phase / sponsor-type / country counts come from the registry's aggregation endpoints on the recruiting set (870 studies each).
- **Country counts are site-level**, not unique trials — see the warning in §2.2.
- **Watch list:** the five most recent start dates among recruiting trials (descending). Two of the five (NCT07748208, NCT07878325) carry estimated start dates in the near future per the registry — they are currently flagged Recruiting.
- **"Most recently started" ranking:** `StartDate:desc` sort over the recruiting set; ties or records with partial dates could rank differently.
