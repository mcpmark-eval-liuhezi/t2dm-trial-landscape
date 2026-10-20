# Type 2 Diabetes Trial Landscape

A public research note on the type 2 diabetes mellitus (T2DM) clinical trial landscape: why the field is moving now, how the registered trial portfolio breaks down, which industry-sponsored trials are currently recruiting, and a registry reference trial.

- **Registry data source:** ClinicalTrials.gov, queried via the registry API on 2026-10-20 (UTC).
- **Web coverage:** recent public reporting, September–October 2026.
- **Tracking issue:** [#1](https://github.com/mcpmark-eval-liuhezi/t2dm-trial-landscape/issues/1)

**Scope of the registry analyses.** The registry's analysis tool caps a single analysis at 5,000 studies, and an unrestricted condition search for `Type 2 Diabetes Mellitus` returns 11,973 records across all study types (9,863 interventional; 5,282 interventional drug trials). The portfolio analyzed below is therefore scoped to **interventional drug trials with a start date on or after 2015-01-01** — the current-era T2DM drug-trial portfolio — which is **2,344 studies**. Every count in the "Registry breakdown" section is reported exactly as the corresponding analysis returned it, and each of the four analyses covered 2,344 studies (`totalStudies: 2344`).

## Why now

- **Once-weekly basal insulin has arrived in T2DM.** The U.S. FDA approved Eli Lilly's Onswik (insulin efsitora), a once-weekly basal insulin injection for adults living with type 2 diabetes — its fourth global approval, following regulatory actions from the European Medicines Agency, Mexico and others. *(Source: PR Newswire, "U.S. Food and Drug Administration (FDA) approves Lilly's Onswik…", Sep 24, 2026)*
- **Roche reported positive Phase II results for the dual GLP-1/GIP receptor agonist enicepatide in people living with type 2 diabetes**, with weight loss of 15.5% at 48 weeks; trade coverage adds that the highest titrated dose (24 mg) achieved an HbA1c reduction of 2.65%, with 90% of that cohort reaching HbA1c ≤ 6.5%. *(Sources: Roche media release, Sep 22, 2026; Clinical Trials Arena, Sep 23, 2026)*
- **Triple-agonist data is resetting expectations for how metabolic trials are designed.** Eli Lilly announced positive Phase III topline results for retatrutide, an investigational GIP/GLP-1/glucagon triple hormone receptor agonist, and an independent deep-dive on the retatrutide TRIUMPH-2 data argues it "forces a reckoning with how we design metabolic trials." *(Sources: Yahoo Finance, Oct 13, 2026; Clinical Trial Vanguard, Oct 12, 2026; SciTechDaily, Oct 19, 2026)*
- **Care guidelines are formalizing the post-GLP-1 pipeline.** The 2026 consensus report on the management of type 2 diabetes notes that many nutrient-stimulated hormone-based medications and combinations are currently in development beyond GLP-1 receptor agonists, with the dual GLP-1/GIP class the first of these. *(Source: Davies et al., "Management of type 2 diabetes, 2026. A consensus report", Diabetologia / Springer, 2026)*
- **GLP-1 benefits keep extending beyond glucose control, widening the outcome set that T2DM trials must power for.** New analyses report semaglutide lowered albuminuria by ~40% versus placebo in type 2 diabetes kidney disease while maintaining eGFR, and EASD 2026 congress coverage continues to feature next-generation candidates such as Tzeild alongside experimental weight-loss drugs. *(Sources: Tuttle et al., Nature Medicine, 2026; diaTribe, EASD 2026 coverage)*

## Registry breakdown

All four analyses below were run on the same query — condition `Type 2 Diabetes Mellitus`, study type interventional, intervention type drug, start date on or after 2015-01-01 — and each analysis covered **2,344 studies**.

### By phase

| Phase | Count (as returned) |
| --- | --- |
| PHASE4 | 588 |
| PHASE3 | 559 |
| PHASE1 | 531 |
| PHASE2 | 480 |
| NA | 236 |
| EARLY_PHASE1 | 39 |

> Note: the phase buckets sum to 2,433, which exceeds the 2,344-study total. The registry counts a multi-phase trial (e.g., Phase 1/Phase 2) once in each phase bucket, so the buckets are not mutually exclusive.

### By overall status

| Overall status | Count (as returned) |
| --- | --- |
| COMPLETED | 1,341 |
| UNKNOWN | 338 |
| RECRUITING | 250 |
| NOT_YET_RECRUITING | 111 |
| ACTIVE_NOT_RECRUITING | 109 |
| TERMINATED | 99 |
| WITHDRAWN | 75 |
| ENROLLING_BY_INVITATION | 15 |
| SUSPENDED | 6 |

### By sponsor type (lead sponsor class)

| Sponsor type | Count (as returned) |
| --- | --- |
| INDUSTRY | 1,276 |
| OTHER | 1,021 |
| OTHER_GOV | 36 |
| NIH | 5 |
| FED | 3 |
| NETWORK | 2 |
| INDIV | 1 |

### By country

The registry's country analysis counts **trial sites/locations**, not unique studies: a multi-country trial contributes one count to every country in which it runs, so the counts sum far beyond the 2,344-study portfolio. Full results as returned (92 countries/territories), sorted by count:

| Country | Count (as returned) |
| --- | --- |
| United States | 14,655 |
| China | 3,030 |
| Japan | 2,403 |
| Canada | 1,622 |
| Germany | 1,563 |
| Poland | 1,322 |
| India | 1,257 |
| United Kingdom | 1,014 |
| Spain | 982 |
| South Korea | 938 |
| Argentina | 907 |
| Russia | 805 |
| Hungary | 774 |
| Mexico | 742 |
| Italy | 734 |
| Czechia | 659 |
| Brazil | 622 |
| Romania | 599 |
| France | 573 |
| Slovakia | 530 |
| Australia | 508 |
| Bulgaria | 459 |
| Turkey (Türkiye) | 454 |
| Israel | 445 |
| Greece | 437 |
| South Africa | 380 |
| Taiwan | 373 |
| Denmark | 273 |
| Netherlands | 273 |
| Ukraine | 258 |
| Austria | 223 |
| Belgium | 220 |
| Puerto Rico | 215 |
| Malaysia | 202 |
| Sweden | 179 |
| Portugal | 169 |
| Thailand | 160 |
| Serbia | 159 |
| Chile | 128 |
| Finland | 124 |
| Croatia | 124 |
| New Zealand | 116 |
| Switzerland | 95 |
| Norway | 94 |
| Colombia | 92 |
| Latvia | 65 |
| Lithuania | 64 |
| Egypt | 58 |
| Saudi Arabia | 56 |
| United Arab Emirates | 53 |
| Pakistan | 46 |
| Hong Kong | 44 |
| Slovenia | 43 |
| Georgia | 42 |
| Philippines | 37 |
| Ireland | 35 |
| Peru | 35 |
| Vietnam | 33 |
| Algeria | 29 |
| Singapore | 28 |
| Estonia | 26 |
| Indonesia | 16 |
| Lebanon | 16 |
| Nigeria | 13 |
| Guatemala | 12 |
| Iran | 11 |
| Iraq | 10 |
| Kuwait | 8 |
| Sri Lanka | 7 |
| North Macedonia | 7 |
| Qatar | 6 |
| Tunisia | 6 |
| Bosnia and Herzegovina | 6 |
| Jordan | 6 |
| Bangladesh | 4 |
| Burkina Faso | 3 |
| Cameroon | 3 |
| Moldova | 3 |
| Mauritius | 3 |
| Syria | 2 |
| Kazakhstan | 2 |
| Kosovo | 1 |
| Guadeloupe | 1 |
| Reunion | 1 |
| Tanzania | 1 |
| Afghanistan | 1 |
| Kenya | 1 |
| Morocco | 1 |
| Paraguay | 1 |
| Uzbekistan | 1 |
| Costa Rica | 1 |
| Dominican Republic | 1 |

## Recruiting trials to watch

Query: condition `Type 2 Diabetes Mellitus`, overall status `RECRUITING`, lead sponsor class `INDUSTRY`, study type interventional, intervention type drug — the registry returns **116** matching studies. Three T2DM trials from that result set:

| NCT ID | Sponsor | Title |
| --- | --- | --- |
| NCT06671587 | Sanofi | iGlarLixi CGM Study in Chinese T2D Individuals After OADs |
| NCT06739122 | Eli Lilly and Company | A Study of Dulaglutide (LY2189265) 3.0 mg and 4.5 mg in Pediatric Participants With Type 2 Diabetes Mellitus (AWARD-PEDS PLUS) |
| NCT05268237 | Biolingus | Safety, Tolerability and Preliminary Efficacy of Sublingual Liraglutide in Patients With Type 2 Diabetes Mellitus |

> Note: the top-ranked registry match under this query (NCT06451757, Khondrion BV — sonlicromanol in primary mitochondrial diseases) is not a T2DM trial per se; it enrolls people with T2DM only within a chronic kidney disease subgroup, so it is not included in the table above.

## Reference trial: NCT01608724

All fields below are taken directly from the ClinicalTrials.gov registry record for NCT01608724, as they appear there.

| Field | Registry value |
| --- | --- |
| NCT ID | NCT01608724 (org study ID: D1680L00008; acronym: SUNSHINE) |
| Official title | A Multicenter, Single Arm, Cohort Study to Evaluate the Efficacy and Safety of Saxagliptin 5mg, Once Daily for 24 Weeks, in Patients With Type 2 Diabetes Mellitus |
| Sponsor | AstraZeneca (lead sponsor, class INDUSTRY; responsible party: sponsor) |
| Study design | Interventional, Phase 4, multicenter single-arm cohort study — non-randomized, single-group assignment, open label (no masking). Drug: **saxagliptin** (other name: Onglyza), oral **5 mg once daily (Q.D.)**, for **24 weeks**. Enrollment: 2,165 (actual). |
| Overall status | COMPLETED (status verified 2015-12) |
| Start date | 2012-11 |
| Primary completion date | 2014-05 (actual) |

Additional registry details: condition "Diabetes Mellitus, Non-Insulin-Dependent" (keyword: Type 2 DM); primary outcome measure is the absolute change from baseline in HbA1c at weeks 6, 12 and 24; the study was conducted at research sites in China; study completion date 2014-05 (actual).

---

*Prepared as the lab's public research note on the T2DM clinical trial landscape. Registry figures are as returned on 2026-10-20 (UTC) and will drift as the registry updates.*
