# T2DM Clinical Trial Landscape Brief

**Source:** ClinicalTrials.gov registry (live queries via the registry API)
**Data as-of:** 2026-10-19 (UTC) — all counts are registry values as returned on this date
**Prepared for:** Strategy review (landscape brief)

---

## 1. Headline numbers

| Metric | Value (as returned) |
|---|---|
| Total T2DM trials in registry | **11,971** |
| Currently recruiting | **870** |
| Top country (by trial sites) | **United States — 49,262** |

---

## 2. Registry-wide picture

All figures below are exact registry counts for the condition search `Type 2 Diabetes Mellitus` (11,971 studies), retrieved 2026-10-19 (UTC). Because the analysis tool caps a single analysis at 5,000 studies, the full set was covered via disjoint partitions that together reconcile exactly to 11,971 (see §6 Methodology).

### 2.1 By overall recruitment status

| Overall status | Count |
|---|---|
| Completed | 7,867 |
| Unknown | 1,531 |
| Recruiting | 870 |
| Not yet recruiting | 419 |
| Active, not recruiting | 339 |
| Terminated | 576 |
| Withdrawn | 242 |
| Enrolling by invitation | 92 |
| Suspended | 32 |
| Expanded-access statuses (AVAILABLE / NO_LONGER_AVAILABLE / TEMPORARILY_NOT_AVAILABLE, combined) | 3 |
| **Total** | **11,971** |

### 2.2 By phase (all T2DM trials)

Aggregated across three disjoint partitions (3,502 + 4,365 + 4,104 = 11,971 studies):

| Phase | Count |
|---|---|
| Phase 3 | 1,644 |
| Phase 4 | 1,406 |
| Phase 2 | 1,309 |
| Phase 1 | 1,243 |
| Early Phase 1 | 86 |
| N/A (no phase assigned) | 4,481 |
| Unknown | 2,112 |

> **Important:** phase buckets sum to 12,281, which exceeds the 11,971 study total. The registry's phase analysis counts a multi-phase trial (e.g., "Phase 1/Phase 2") once in **each** phase bucket, so buckets are not mutually exclusive. `N/A` + `Unknown` together account for 6,593 records (mostly observational studies and records without a phase field).

### 2.3 By sponsor type (lead sponsor class)

| Lead sponsor class | Count |
|---|---|
| Other (academic, hospital, nonprofit, etc.) | 7,165 |
| Industry | 4,349 |
| NIH | 107 |
| Other government (non-U.S. / non-federal) | 244 |
| U.S. federal (non-NIH) | 66 |
| Research network | 27 |
| Individual | 13 |
| **Total** | **11,971** |

> Note: `NIH` reflects the **lead sponsor class only**. NIH-funded trials led by universities or hospitals are counted under `Other`, so this understates total NIH-supported activity.

### 2.4 By country — top 10 (trial-site counts)

| Rank | Country | Trial sites |
|---|---|---|
| 1 | United States | 49,262 |
| 2 | Japan | 6,207 |
| 3 | China | 5,744 |
| 4 | Germany | 5,667 |
| 5 | Canada | 5,439 |
| 6 | United Kingdom | 4,144 |
| 7 | India | 3,906 |
| 8 | Poland | 3,228 |
| 9 | Russia | 3,170 |
| 10 | Spain | 3,060 |

(Next: France 2,992, Italy 2,577, South Korea 2,547.)

> **Important:** the registry's country analysis counts **trial sites/locations**, not unique trials. A single multi-country trial contributes one count per country it runs in. Verified empirically: NCT01608724 alone (one study) returns `China: 37` — its 37 Chinese sites. So these figures measure geographic footprint of study locations, and country counts far exceed the 11,971 trial total by design.

### 2.5 Phase breakdown restricted to currently recruiting trials (active pipeline)

Analysis returned for the 870 recruiting trials, exactly as the registry returned it:

| Phase | Count |
|---|---|
| N/A (no phase assigned) | 410 |
| Unknown | 201 |
| Phase 3 | 74 |
| Phase 4 | 68 |
| Phase 2 | 68 |
| Phase 1 | 58 |
| Early Phase 1 | 13 |

> Buckets sum to 892 vs. 870 recruiting trials — same multi-phase counting behavior as §2.2.

---

## 3. Shortlist: recruiting, industry-sponsored, Phase 3 T2DM trials

Query: condition `Type 2 Diabetes Mellitus`, overall status `RECRUITING`, lead sponsor class `INDUSTRY`, phase `PHASE3`; sorted by target enrollment (descending). The registry returned **54** matching trials; the 8 largest are listed. Machine-readable copy: [`data/shortlist.csv`](../data/shortlist.csv).

| # | NCT | Short title | Sponsor | Target enrollment |
|---|---|---|---|---|
| 1 | NCT07064473 | EASi-PROTKT™ — vicadrostat (BI 690517) + empagliflozin in T2DM, hypertension & CVD | Boehringer Ingelheim | 11,800 |
| 2 | NCT07667803 | Master protocol: efficacy and safety of elecoglipron in obesity/overweight ± T2DM | AstraZeneca | 4,500 |
| 3 | NCT07481747 | SURMOUNT-1: tirzepatide once weekly vs placebo in obese/overweight with comorbidities | Hudson Biotech | 2,539 |
| 4 | NCT07784725 | AZD6234 in obesity/overweight with weight-related comorbidity (without T2DM) | AstraZeneca | 2,500 |
| 5 | NCT07564414 | CagriSema (two doses) vs semaglutide for weight loss in obesity ± T2DM | Novo Nordisk A/S | 2,500 |
| 6 | NCT07662109 | Eluminate-5: elecoglipron + dapagliflozin combination in adults with T2DM | AstraZeneca | 2,000 |
| 7 | NCT07351045 | Enicepatide (RO7795068) in obesity/overweight without T2DM | Hoffmann-La Roche | 2,000 |
| 8 | NCT07321886 | Eloralintide (LY3841136) in obesity/overweight without T2DM | Eli Lilly and Company | 1,980 |

> Caveat on composition: the registry's condition search for "Type 2 Diabetes Mellitus" also returns cardio-metabolic trials that enroll T2DM-adjacent populations (e.g., obesity trials that permit or exclude T2DM). Trials #3, #4, #7 and #8 are obesity/overweight trials surfaced by that match; #1, #2, #5 and #6 are T2DM-core or explicitly T2DM-inclusive. Enrollment figures are the registry's current target (mostly `ESTIMATED`, not actual).

---

## 4. Deep dives

### 4.1 NCT01608724 — SUNSHINE (cited in our draft)

**AstraZeneca, saxagliptin 5 mg once daily for 24 weeks in T2DM.** Full record pulled 2026-10-19.

| Field | Registry value |
|---|---|
| Overall status | **COMPLETED** (status verified 2015-12) |
| Phase | **Phase 4** |
| Enrollment | **2,165 (ACTUAL)** |
| Lead sponsor | **AstraZeneca (INDUSTRY)** — also the responsible party (sponsor) |
| Study type / design | Interventional; single-arm, non-randomized, open-label (single group) |
| Condition | Diabetes Mellitus, Non-Insulin-Dependent (Type 2 DM) |
| Interventions | Drug: Saxagliptin (oral 5 mg Q.D.; other name: Onglyza) |
| Start date | 2012-11 |
| Primary completion | 2014-05 (ACTUAL) |
| Study completion | 2014-05 (ACTUAL) |
| Last update posted | 2016-02-02 (estimated) |
| Locations | China (site-level count: 37), e.g., Baotou, Beijing, Chengdu, Chongqing, Dalian… |
| Primary outcome | Absolute change from baseline in HbA1c (weeks 6, 12, 24) |

**Verdict vs. our draft:** the registry record **matches** the draft's claim of a completed, industry-sponsored saxagliptin trial. Two refinements for the brief: the registry classifies it as **Phase 4** (post-marketing), not Phase 3, and the single-arm open-label design means it is an efficacy/safety cohort study rather than a randomized comparative trial.

### 4.2 NCT07064473 — EASi-PROTKT™ (shortlist #1)

**Boehringer Ingelheim — vicadrostat (BI 690517) + empagliflozin in T2DM, hypertension and established CVD.** Largest recruiting industry Phase 3 trial in the shortlist.

| Field | Registry value |
|---|---|
| Overall status | RECRUITING (status verified 2026-10) |
| Phase | Phase 3 |
| Enrollment | 11,800 (ESTIMATED) |
| Lead sponsor | Boehringer Ingelheim (INDUSTRY) |
| Design | Randomized, parallel-group, quadruple-masked (participant, care provider, investigator, outcomes assessor); superiority |
| Conditions | Diabetes Mellitus, Type 2; Hypertension; Cardiovascular Diseases |
| Start / completion | Started 2025-07-22 (ACTUAL); primary completion 2029-12-14 and completion 2029-12-21 (ESTIMATED) |
| Last update posted | 2026-10-14 (ACTUAL) |
| Oversight | Data monitoring committee: yes; FDA-regulated drug: yes |
| Primary outcome | Time to first event of cardiovascular death or heart failure event (up to 51 months) |
| Arms | Vicadrostat + empagliflozin (experimental) vs vicadrostat-matched placebo + empagliflozin (active comparator) |

### 4.3 NCT07662109 — Eluminate-5 (shortlist #6)

**AstraZeneca — elecoglipron + dapagliflozin combination vs each agent alone in adults with T2DM.**

| Field | Registry value |
|---|---|
| Overall status | RECRUITING (status verified 2026-08) |
| Phase | Phase 3 |
| Enrollment | 2,000 (ESTIMATED) |
| Lead sponsor | AstraZeneca (INDUSTRY) |
| Design | Randomized, double-blind, parallel-group, quadruple-masked; 5 arms (2 elecoglipron dose levels × dapagliflozin or matched placebo, plus dapagliflozin-alone comparator) |
| Conditions | Type 2 Diabetes Mellitus |
| Start / completion | Started 2026-07-06 (ACTUAL); primary completion and completion 2028-07-05 (ESTIMATED) |
| Last update posted | 2026-08-31 (ACTUAL) |
| Oversight | Data monitoring committee: no; FDA-regulated drug: yes |
| Primary outcome | Change from baseline in HbA1c (baseline to Week 40) |
| Secondary outcomes (selected) | HbA1c < 7% achievement, percent change in body weight, fasting plasma glucose |

---

## 5. Caveats

1. **As-of date.** All counts in this brief are registry values retrieved on **2026-10-19 (UTC)** from the live ClinicalTrials.gov registry. The registry changes daily; re-run the queries before any number is quoted externally.
2. **Multi-phase counting.** The registry's phase analyses count a multi-phase trial once per phase bucket, so phase buckets sum to more than the study total (12,281 vs 11,971 overall; 892 vs 870 for recruiting). Treat phase buckets as non-exclusive.
3. **Country figures are site-level, not trial-level.** The country analysis counts trial locations; a multi-country trial contributes to every country it runs in (verified: NCT01608724 → `China: 37`). Country counts therefore exceed the number of unique trials by design.
4. **Sponsor class is lead-sponsor only.** `NIH` (107) counts NIH as lead sponsor; NIH-funded studies led by academic centers fall under `Other` (7,165).
5. **Condition-search breadth.** "Type 2 Diabetes Mellitus" as a condition search returns T2DM-core trials plus adjacent cardio-metabolic trials (obesity/overweight programs) that match the condition indexing; see the shortlist caveat in §3.
6. **Enrollment figures.** Shortlist enrollment counts are targets (mostly `ESTIMATED`); NCT01608724's 2,165 is `ACTUAL`.
7. **Status reconciliation.** The status table sums exactly to 11,971 (including 3 expanded-access-status records). Phase and sponsor partitions also reconcile exactly (3,502 + 4,365 + 4,104 = 11,971; 4,349 + 107 + 7,165 + 350 = 11,971).

---

## 6. Methodology (reproducibility)

- **Query base:** condition search `Type 2 Diabetes Mellitus` → 11,971 studies (2026-10-19).
- **Analysis cap:** the trends-analysis tool processes at most 5,000 studies per run; a single whole-registry T2DM analysis was rejected (11,971 > 5,000). The full set was therefore covered with **disjoint partitions** whose totals reconcile exactly to 11,971:
  - Phase & country, partition A: `COMPLETED` **and** (lead sponsor class `INDUSTRY` or `NIH`) → 3,502 studies
  - Phase & country, partition B: `COMPLETED` **and not** (`INDUSTRY` or `NIH`) → 4,365 studies
  - Phase & country, partition C: **not** `COMPLETED` → 4,104 studies
- **Status counts:** exact `totalCount` values from status-filtered registry searches (each status is a disjoint bucket).
- **Sponsor counts:** exact `totalCount` values from lead-sponsor-class-filtered searches; the 350 records outside `INDUSTRY`/`NIH`/`OTHER` were sub-analyzed (`OTHER_GOV` 244, `FED` 66, `NETWORK` 27, `INDIVID` 13).
- **Recruiting-only phase breakdown:** single trends analysis on the `RECRUITING` filter (870 studies, under the cap).
- **Shortlist:** `RECRUITING` + `INDUSTRY` lead sponsor + `PHASE3`, sorted by `EnrollmentCount` descending (54 matching trials; top 8 shown).
- **Deep dives:** full study records pulled by NCT ID.
- **Verification of the country metric:** a control analysis on NCT01608724 alone returned `China: 37` for a single study, confirming site-level counting.
