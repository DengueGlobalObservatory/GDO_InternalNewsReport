# GDO Internal News Report — 2026-09-21

*Source: Global Dengue Observatory (accessed 2026-09-21).*

## 1. Header

- **Report date:** 2026-09-21 (Monday routine run)
- **Active snapshot:** `snapshots/2026_09_21/` — **new pull this week**. Source data vintage (`target_render_date`): 2026-09-18. Source commit: `215eb24d` (DENV_global_observatory `Output/2026_09_18/`). Prior snapshot: `snapshots/2026_09_07/` (vintage 2026-09-04).
- **Pull status this week:** **pull week.** `target_render_date` advanced from 2026-09-04 to 2026-09-18, so Step 1's fetch/diff ran in full.
- **Countries covered:** 85.

## 2. This week's snapshot

Global picture across the 85 tracked countries/territories, from `latest_status.csv` only.

**Cumulative severity band** (percentile_cumulative, current position vs. seasonal-to-date expectation):

| Band | Countries |
|---|---|
| Normal | 28 |
| Low | 23 |
| High | 12 |
| Extremely High | 9 |
| Unknown | 7 |
| Extremely Low | 6 |

The 9 at **Extremely High** cumulative severity: Cambodia, Cook Islands, Cuba, Guyana, Kenya, Maldives, Sri Lanka, Sudan, and Timor-Leste.

**Current-season severity band** (current_season_percentile, i.e. how this season is tracking overall):

| Band | Countries |
|---|---|
| Low | 35 |
| Normal | 20 |
| Extremely Low | 17 |
| Unknown | 6 |
| High | 4 |
| Extremely High | 3 |

Current-season **Extremely High**: Cuba (percentile 100.0), Kenya (100.0), Cambodia (99.2). Current-season **High**: Maldives (90.2), Sri Lanka (87.7), United Republic of Tanzania (78.9), Suriname (76.4).

**Notable current-season cooling despite Extremely High cumulative standing:** Guyana's current-season percentile has crashed from 96.7 to 5.9 (Category C, largest single move this snapshot, −90.8) even as its cumulative severity stays Extremely High (98.6) — a season that ran hot early and has since gone quiet, in the same pattern as Cook Islands' 97.8→20.9 fall two pulls ago. Samoa shows the same shape on a smaller scale: cumulative High (79.6) but current-season down to Low (6.3, from 59.8 — Category C, −53.5).

**Caveat — data recency.** Of this week's ten targeted countries (Section 3), nine (Afghanistan, Argentina, Burkina Faso, Côte d'Ivoire, Grenada, Malaysia, Panama, Vietnam, Wallis and Futuna) have a latest observed month of 2026-08-01 (~1.7 months stale, within GDO's 1–2 month nowcast sweet spot, near its upper edge); Timor-Leste sits at 2026-07-01 (~2.7 months stale, beyond the sweet spot — treat its figures as lower-confidence). **Small-sample/large-ratio instability:** Argentina's monthly ratio (0.02×) rests on a single observed case against a ~50-case seasonal baseline — a swing this small in absolute terms should not be read as a confirmed trend on its own. Côte d'Ivoire shows the same shape in reverse: 12 observed cases against a much larger ~1,145-case baseline (ratio 0.01×) — a near-total collapse relative to expectation that is more likely a reporting-lag/data-availability issue than a genuine outbreak resolution (see Section 3).

## 3. News — targeted (10 countries)

**Country selection note:** `movers.csv` flagged 17 Category A (severity-interpretation band changes) and 18 Category B (monthly-ratio-descriptor changes) rows this week — 31 unique countries once de-duplicated, well beyond the 10-country cap. Per the routine's prioritisation rule (A/B over C), all 10 below come from that A/B pool; no Category C-only mover was needed. Within the 31, priority went first to double/triple-category movers (Vietnam and Afghanistan appear in A, B *and* C; Malaysia, Wallis and Futuna, Argentina, Burkina Faso and Côte d'Ivoire each appear in two categories), then to the single-category movers that filled remaining regional gaps and carried the most severe/dramatic single crossing: Timor-Leste (currently the most severe country in the entire dataset, Extremely High cumulative, 99.8th percentile) and Panama and Grenada (filling North & Central America and Caribbean, otherwise unrepresented). This is a judgement call, as in prior weeks — a different, defensible 10 could have been drawn from the same 31.

### Vietnam (Category A — severity interpretation: Average → Above average; Category B — monthly ratio: running well below → running well above; Category C — current-season percentile 2.4 → 32.6, one of the largest swings this snapshot)
- GDO figures: 24,069 reported cases (latest observed month 2026-08-01, ~1.7 months stale). Cumulative percentile 85.5 (High); current-season percentile 32.6 (Normal), up sharply from 2.4 (Extremely Low). Estimated total seasonal cases: 237,572. Monthly ratio: running well above (1.31×, off an ~18,422-case baseline — a large, stable baseline, so this reading isn't small-sample noise).
- News: **fresh and directionally consistent.** Ho Chi Minh City has recorded 32,626 cases since the start of 2026 (1,544 in the most recent week, as of 21 Sept); Hanoi reported over 2,000 cases in the week to 18 Sept, roughly double the weeks before it, concentrated in Phu Xuyen, Hoang Mai, Cau Giay, Ha Dong, Dong Da, Dan Phuong, Thanh Oai and Thanh Tri districts. Nationally, over 78,000 cases and 13 deaths had been recorded by mid-August — 20% up on 2025 — with case counts typically peaking in October. [PressReader/Viet Nam News, 21 Sep](https://www.pressreader.com/vietnam/viet-nam-news/20260921/281548002800575) · [TechTimes, 3 Aug](https://www.techtimes.com/articles/322818/20260803/dengue-cases-vietnam-have-doubled-adults-now-face-greater-risk-children.htm) · [Dengue Visual Atlas](https://denguevisualatlas.com/en/78000-cases-of-dengue-in-vietnam-in-2026-20-more-than-the-previous-year/)

### Afghanistan (Category A — severity interpretation: Rare bad event → Above average; Category B — monthly ratio: running well above → tracking near; Category C — current-season percentile 51.0 → 33.2)
- GDO figures: 279 reported cases (latest observed month 2026-08-01, ~1.7 months stale). Cumulative percentile 82.2 (High) — eased from a "Rare bad event" reading but still in the High band. Current-season percentile 33.2 (Normal), down from 51.0. Estimated total seasonal cases: 6,717. Monthly ratio: tracking near baseline (1.05×, vs ~265 expected) — no longer running well above.
- News: no dated September 2026 update could be confirmed within the ~2-week window. Available coverage is background/historical (WHO-confirmed outbreak reporting and academic epidemiology from Nangarhar province in earlier years) rather than a live 2026 situation report — flag to the researcher as a genuine news gap rather than a sign of continued easing. [VOA, WHO dengue outbreak confirmation (background)](https://www.voanews.com/a/dengue-fever-outbreak-confirmed-in-afghanistan-who-says-/6688911.html)

### Malaysia (Category A — severity interpretation: Average → Above average; Category C — current-season percentile 24.7 → 56.7, the largest current-season increase this snapshot)
- GDO figures: 11,629 reported cases (latest observed month 2026-08-01, ~1.7 months stale). Cumulative percentile 83.6 (High). Current-season percentile 56.7 (Normal), up sharply from 24.7 (Low). Estimated total seasonal cases: 121,276. Monthly ratio: running well above (1.82×, off a ~6,399-case baseline).
- News: **fresh, and a further escalation on last fortnight's figures.** Nationwide cases up 66% to 65,979 as of epidemiological week 35 (vs. 39,616 over the same period in 2025); deaths up 93.8% to 62 (vs. 32 last year) — this is a bigger jump than the 56% year-on-year rise reported in mid-August (58,079 cases, 55 deaths). [Malay Mail, 9 Sep](https://www.malaymail.com/news/malaysia/2026/09/09/dengue-cases-soar-66pc-deaths-hit-62-in-malaysia-almost-double-2025-toll/234576) · [PressReader/Straits Times, 22 Aug](https://www.pressreader.com/singapore/the-straits-times/20260822/281659671884700)

### Wallis and Futuna (Category A — severity interpretation: Rare bad event → Average, an easing; Category B — monthly ratio: running well above → running well below, a reversal)
- GDO figures: 12 reported cases (latest observed month 2026-08-01, ~1.7 months stale). Cumulative percentile 71.7 (Normal band). Current-season percentile 44.8 (Normal). Estimated total seasonal cases: 487. Monthly ratio: running well below (0.17×, vs ~72.6 expected) — a sharp reversal from the "running well above" reading tied to earlier in the year's outbreak.
- News: no item confirmed within the last ~2 weeks, in either English or French. Background found is all several months old: local transmission was first confirmed in Futuna in April 2026, and by mid-July the epidemic was reported to be slowing in Futuna while progressing in Wallis, with 225 cumulative cases cited without a firm date. Directionally consistent with GDO's own easing read, but not independently confirmed for September. [La 1ère, 17 Jul](https://la1ere.franceinfo.fr/wallisfutuna/dengue-l-epidemie-ralentit-a-futuna-mais-progresse-a-wallis-1711747.html)

### Argentina (Category A — severity interpretation: Average → Below average; Category C — current-season percentile 22.3 → 10.7)
- GDO figures: 1 reported case (latest observed month 2026-08-01, ~1.7 months stale). Cumulative percentile 15.9 (Low). Current-season percentile 10.7 (Low), down from 22.3. Estimated total seasonal cases: 79. **Caveat:** the monthly ratio (0.02×) rests on a single case against a ~50-case seasonal baseline — treat it as noisy in isolation, though the percentile-band easing is a separate, independently meaningful reading.
- News: no September-specific figure confirmed. National picture as of mid-2026: 122,090 suspected cases, 22,409 confirmed, 242 severe cases, 6 deaths — lower than the same period in 2025, with authorities maintaining surveillance and Salta province coordinating with Bolivia on cross-border monitoring. Overall notably less severe than the 2024 epidemic. [Argentina.gob.ar, Boletines Epidemiológicos 2026](https://www.argentina.gob.ar/salud/boletin-epidemiologico-nacional/boletines-2026) · [LA NACION, claves detrás de la baja de casos](https://www.lanacion.com.ar/sociedad/las-claves-detras-de-la-baja-de-casos-de-dengue-y-las-alertas-de-los-especialistas-nid03022026/)

### Burkina Faso (Category A — severity interpretation: Above average → Cannot determine; Category B — monthly ratio: running well above → running well below)
- GDO figures: 1,142 reported cases (latest observed month 2026-08-01, ~1.7 months stale). Cumulative severity is now **"Cannot determine"** (percentile unavailable this pull, versus a defined "Above average" two pulls ago) — a data-availability caveat about GDO's own pipeline, not an epidemiological claim about Burkina Faso. Current-season percentile 42.1 (Normal). Estimated total seasonal cases: 93,174. Monthly ratio: running well below (0.41×, vs ~2,768 baseline).
- News: the Oubritenga regional governor's 10 September alert over an "unusual and rapid increase" in Ziniaré and Zorgho — flagged in last fortnight's report — remains the only live 2026 situation update found, now over a week old. Worth flagging the mismatch to the researcher: ground reporting suggests continued/worsening transmission even as GDO's own classification reverted to "Cannot determine" this pull — a data gap, not evidence of improvement. [Wakat Séra, 10 Sep](https://www.wakatsera.com/burkina-une-augmentation-inhabituelle-et-rapide-de-cas-de-dengue-a-ziniare-et-zorgho/)

### Timor-Leste (Category B — monthly ratio: running well above → running well below; currently the most severe country in this snapshot — Extremely High cumulative, 99.8th percentile)
- GDO figures: 18 reported cases (latest observed month 2026-07-01, ~2.7 months stale — beyond GDO's nowcast sweet spot; treat as lower-confidence). Cumulative percentile 99.8 (Extremely High). Current-season severity "Unknown" (percentile 16.5, interpretation "Cannot determine"). Estimated total seasonal cases: 5,230. Monthly ratio: running well below (0.47×, vs ~38.1 baseline) — a reversal, though on a moderate baseline so treat as indicative rather than definitive.
- News: no item within the strict ~2-week window; the freshest available figures are several months old. Timor-Leste recorded an estimated 4,824 cases year-to-date (4.4× an average year), one of the sharpest early-year risers, but has declined month-on-month since April — directionally consistent with this pull's ratio reversal, though the specific reporting found (hospitals overwhelmed, Jan–Feb surge) predates the current easing by many months. [World Mosquito Program, Timor-Leste](https://www.worldmosquitoprogram.org/global-progress/timor-leste) · [WHO, Dengue – Timor-Leste](https://www.who.int/emergencies/disease-outbreak-news/item/dengue---timor-leste)

### Panama (Category B — monthly ratio: running slightly below → running well above)
- GDO figures: 1,688 reported cases (latest observed month 2026-08-01, ~1.7 months stale). Cumulative percentile 84.2 (High). Current-season percentile 53.8 (Normal). Estimated total seasonal cases: 18,528. Monthly ratio: running well above (1.40×, vs ~1,209 baseline).
- News: **fresh, but a genuinely mixed picture — flag both figures, don't pick one.** Panama's Ministry of Health (MINSA) reports the 2026 season running well *below* 2025 nationally: 7,565 accumulated cases as of the week of 23–29 Aug, down 30.9% on the 10,664 recorded in the same week of 2025, with hospitalisations down 14.5% and the incidence rate roughly halved. A separate 10 September item reports a 7.1% week-on-week rise. **Caveat:** GDO's monthly ratio compares this month's cases against Panama's own seasonally-expected baseline for the same calendar month, not against the same period last year — so "running well above" (vs. seasonal baseline) and "down 30.9% year-on-year" (vs. 2025) are not actually contradictory, but presenting them side-by-side without this context would read as one. [Infobae, 16 Sep](https://www.infobae.com/panama/2026/09/16/panama-registra-7565-casos-acumulados-de-dengue-y-baja-las-hospitalizaciones-en-145/) · [Infobae, 10 Sep](https://www.infobae.com/panama/2026/09/10/los-casos-de-dengue-aumentaron-71-en-una-semana-en-panama/)

### Côte d'Ivoire (Category A — severity interpretation: Average → Below average; Category C — current-season percentile 35.8 → 10.0)
- GDO figures: 12 reported cases (latest observed month 2026-08-01, ~1.7 months stale). Cumulative percentile 11.8 (Low). Current-season severity "Unknown" (percentile 10.0, interpretation "Cannot determine" — copied verbatim from `latest_status.csv` despite the apparent internal inconsistency between a present percentile value and an "Unknown" band; likely an upstream data-pipeline quirk, not a claim made here). Estimated total seasonal cases: 509. **Caveat:** the monthly ratio (0.01×, 12 cases against a ~1,145-case baseline) is a near-total collapse relative to expectation — more likely a reporting-lag/data-availability issue than a genuine, confirmed improvement, especially given the news below.
- News: **directly contradicts GDO's easing read this pull — flag to the researcher rather than picking a side.** Côte d'Ivoire's Ministry of Health describes an active, ongoing "6th dengue epidemic": 380 suspected cases and 3 deaths recorded by late September 2026, with an emergency planning meeting convened (Ministry of Health, WHO Côte d'Ivoire office) to organise an awareness campaign. GDO's own case count (12, for the 2026-08-01 month) is far below the ministry's cumulative epidemic total (380), which most likely reflects a reporting-lag or scope difference (monthly nowcast vs. cumulative epidemic count) rather than a real-world improvement. [Ministère de la Santé de Côte d'Ivoire, 6è épidémie de dengue](https://sante.gouv.ci/actualite/1559)

### Grenada (Category B — monthly ratio: running well below → running well above)
- GDO figures: 63 reported cases (latest observed month 2026-08-01, ~1.7 months stale). Cumulative percentile 55.1 (Normal). Current-season percentile 30.2 (Normal). Estimated total seasonal cases: 255. Monthly ratio: running well above (1.60×, vs ~39.5 baseline).
- News: fresh and directionally consistent. Grenada's Ministry of Health "urges vigilance amid increase in dengue cases" after a rise from 6 cases (epi week 32) to 23 cases (epi week 33, 16–22 Aug) — adults aged 25–44 the most affected group. Sits within PAHO's broader Grade-3 regional outbreak response across the Americas (Section 4). [NOW Grenada, Aug 2026](https://nowgrenada.com/2026/08/ministry-of-health-urges-vigilance-amid-increase-in-dengue-cases/)

## 4. News — general scan (5 items)

Independent broad scan, capped at 5; includes GDO-tracked countries with dramatic recent news outside this week's 10-country target list, and non-endemic/no-GDO-data settings per the routine's instruction.

1. **Bangladesh, 2026-09-21 (ongoing, record-breaking)** — 87 dengue deaths recorded so far in September alone, the highest monthly toll of the year, bringing the 2026 cumulative death toll to 184; 61,972 confirmed cases since January, with 26,126 of those in just the first 20 days of September. GDO-tracked (High cumulative severity, running well above ratio) but not among this week's 10 targeted countries; its own latest observed month is well behind this surge. [Social News XYZ, 21 Sep](https://www.socialnews.xyz/2026/09/21/bangladesh-reports-87-dengue-deaths-in-september-highest-monthly-toll-this-year) · [Xinhua, 21 Sep](https://english.news.cn/20260921/600a67d1e27b42479ce6da5ead7cf6cf/c.html)
2. **Florida, United States, as of 2026-09-16/19** — Florida has confirmed its first dengue death of 2026 amid an outbreak now at 152–153 locally-acquired cases (its second-highest on record), concentrated in Hillsborough County, with additional locally-transmitted cases confirmed in Orange County (18 Sep) and alerts in Pasco and Miami-Dade. A further 186 travel-associated cases have been reported nationally in 2026. Non-endemic in GDO terms; continues the "dengue's US range is expanding" thread from prior weeks. [Weather.com, 19 Sep](https://weather.com/2026/09/19/health/florida-confirms-death-dengue-amid-outbreak) · [Florida DOH, Arbovirus Surveillance Week 36](https://www.floridahealth.gov/wp-content/uploads/2026/09/fl-arbovirus-report-w36-2026.pdf)
3. **Philippines, through 2026-09-05 — a genuinely mixed national/local picture** — Nationally, the DOH reported 138,538 cases, a 36% *decrease* on 217,693 over the same period in 2025. But Cebu Province bucked the national trend: 3,759 cases and 21 deaths, up from ~2,000 in 2025 (Cebu City alone: 2,456 cases, +65.5% year-on-year). Not GDO-tracked; a useful reminder that a national improvement can mask a sharply worsening sub-region. [Outbreak News Today, Cebu](https://outbreaknewstoday.substack.com/p/cebu-reports-rise-in-dengue-in-2026)
4. **Americas region-wide, epi week 33 (through 2026-09-11)** — PAHO's Grade-3 (highest level) multi-country outbreak response now covers 1,599,333 suspected cases, 3,176 severe cases and 507 deaths region-wide — still 58% below the same period in 2025, even as several individual countries (Grenada, Section 3; Cebu, above) show local upticks. Useful counter-narrative to this week's individual escalation stories. [PAHO/WHO, Epi Week 33](https://www.paho.org/en/topics/dengue/dengue-multi-country-grade-3-outbreak)
5. **France, as of 2026-07-27 — non-endemic autochthonous transmission, continuing theme** — Two unrelated locally-acquired (autochthonous) dengue cases identified in the Tarn and Hérault departments (Occitanie). The most recent dated figure found this week is from late July; no fresher September count could be confirmed (ECDC's own site was unreachable from this session — see note below). Continues the recurring "dengue's reach is expanding into Europe" thread from prior weeks' reports. [Connexion France, France's first native dengue cases of 2026](https://www.connexionfrance.com/news/first-native-dengue-fever-cases-recorded-in-france-in-2026/803099)

*Note: this session's network access could not reach ecdc.europa.eu directly this run (egress blocked), so item 5 relies on press coverage rather than ECDC's own weekly threat report as in some prior weeks — flagged for the researcher, not a claim that ECDC's figures have changed.*

## 5. Trend since last update

35 unique mover countries flagged this week (17 Category A rows, 18 Category B rows, 10 Category C rows; some countries appear in more than one category — see Section 3's selection note and the full table in Section 8.1).

**Category A — severity-band interpretation changes (17), worsening first, then easing, then indeterminate:**
- Afghanistan: Rare bad event → Above average (easing, still High)
- Malaysia: Average → Above average (worsening, now High)
- Nepal: Average → Above average (worsening, now High)
- Vietnam: Average → Above average (worsening, now High)
- Burkina Faso: Above average → **Cannot determine** (data-availability caveat, see Section 3)
- Seychelles: Cannot determine → Below average (newly defined)
- Saint Kitts and Nevis: Above average → **Cannot determine** (data-availability caveat)
- Argentina, Bhutan, Côte d'Ivoire, Mauritania, Reunion, Tuvalu: Average → Below average (improving)
- Wallis and Futuna: Rare bad event → Average (improving)
- Saint Martin, French Polynesia: Below average → Rare good event (improving further)
- Uruguay: Below average → Average (improving)

**Category B — monthly-ratio descriptor changes (18):**
- Malaysia, Grenada, Colombia, Panama, United States, Brazil: below-band → **running well above** (worsening)
- Afghanistan: running well above → tracking near (easing)
- Burkina Faso, New Caledonia, Senegal, Timor-Leste, Vanuatu, Wallis and Futuna: running well above → running well below/slightly below (easing/reversal)
- Australia, Bolivia, Ethiopia, Fiji: below-band shifts further down (well below → slightly below, or slightly below → tracking near) — minor
- Vietnam: running well below → running well above (worsening — see Section 3)

**Category C — current-season percentile shifts (10, largest first):**

| Country | Prior | Current | Δ |
|---|---|---|---|
| Guyana | 96.7 | 5.9 | −90.8 |
| Samoa | 59.8 | 6.3 | −53.5 |
| Sudan | 81.2 | 61.2 | −20.0 |
| Côte d'Ivoire | 35.8 | 10.0 | −25.8 |
| Kiribati | 40.7 | 22.8 | −17.8 |
| Afghanistan | 51.0 | 33.2 | −17.8 |
| Malaysia | 24.7 | 56.7 | +32.0 |
| Vietnam | 2.4 | 32.6 | +30.3 |
| Reunion | 10.1 | 21.3 | +11.2 |
| Argentina | 22.3 | 10.7 | −11.5 |

## 6. Social-media candidate flags

Ranked short-list, for the researcher drafting Tuesday's posts.

1. **Vietnam — GDO's biggest mover this week, and strongly corroborated.** The only triple-category (A+B+C) mover, with a current-season percentile jump from 2.4 to 32.6, now backed by fresh, dated news: Hanoi cases doubling week-on-week (to 18 Sep), Ho Chi Minh City at 32,626 cases since January, national count up 20% on 2025 with the usual October peak still ahead. *No major caveat — GDO's read and the news line up cleanly, though the season hasn't peaked yet.*
2. **Malaysia — still escalating, and the gap keeps widening.** Ministry of Health figures rose from 58,079 cases/55 deaths (15 Aug) to 65,979 cases/62 deaths (week 35, 9 Sep) — a 66% year-on-year rise, deaths nearly doubled. GDO's own current-season percentile jumped further than any other country this pull (+32.0). *Caveat: GDO's raw case figure (11,629) reflects the August month only — don't conflate it with the ministry's cumulative year-to-date total (65,979).*
3. **Bangladesh — the most dramatic single figure this week, and it's a new record.** 87 deaths in September alone is the highest monthly toll of the year, pushing 2026's cumulative death toll to 184. GDO-tracked (High severity, running well above) but outside this week's 10-country selection. *Caveat: as in prior weeks, don't attribute the September press figures to GDO directly — its own nowcast vintage sits well behind this surge.*
4. **Panama or Côte d'Ivoire — a "read GDO's ratio carefully" story, if the researcher wants one.** Both countries this pull show GDO nowcast readings that look like they're moving one way (Panama "running well above"; Côte d'Ivoire's cases collapsing to near-zero against baseline) while ground reporting says something different (Panama's ministry reports cases down 30.9% year-on-year; Côte d'Ivoire's ministry describes an active "6th epidemic"). Good material for a post about *why* GDO's seasonal-baseline ratio isn't the same thing as a year-on-year press figure. *Caveat: this is an explainer angle, not a "worsening/improving" claim — frame it as methodology, not alarm.*
5. **Grenada / wider Caribbean — smaller number, but sits inside a Grade-3 regional response.** Grenada's cases nearly quadrupled week-on-week in mid-August (6→23), and GDO's own ratio flipped fully from "running well below" to "running well above" this pull. Ties into PAHO's ongoing Grade-3 (highest-level) outbreak response across the Americas (Section 4). *Caveat: Grenada's absolute case count (63 for the month) is small — treat the ratio flip as directionally real but not (yet) a large-scale event on its own.*

## 7. Scientific literature findings

Lighter-effort pass; a handful of recent items across forecasting, climate, vaccine policy and surveillance methods.

- **Forecasting/climate:** A climate-driven machine-learning model for Bangladesh (14 years of monthly incidence plus temperature/precipitation/humidity data) projects the probability of exceeding 20,000 monthly cases rising from 37% (2025) to 64% (2026) to ≥90% (2027 onward) — directly relevant given Bangladesh's own record September death toll this week (Section 4). *Health Science Reports*, 2026. [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC13087637/)
- **Climate drivers:** A review frames dengue as a "sentinel signal" for climate-driven vector-borne disease transmission in Europe, tying into this week's France autochthonous-case item (Section 4) and the broader "dengue's reach is expanding" theme running through recent reports. *PMC*, 2026. [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC13418699/)
- **Vaccine policy:** India's drug regulator (DCGI) approved Qdenga (TAK-003) in July 2026 — the country's first licensed dengue vaccine, for ages 4–60, two doses three months apart — with a mandated post-marketing safety and effectiveness study within six months of rollout. A concrete, dated policy development rather than a modelling exercise. [Happiest Health](https://www.happiesthealth.com/articles/infectious-diseases/india-approves-dengue-vaccine-qdenga)
- **Surveillance methods:** A systematic review (accepted 30 Jun 2026) assesses wastewater-based epidemiology as an early-warning complement to clinical/entomological dengue surveillance, noting it can detect cryptic transmission before clinical identification — though evidence for a consistent early-warning advantage over existing methods remains limited. *Pathogens*, 2026. [DOI](https://doi.org/10.3390/pathogens15070690)
- **Surveillance methods (real-world case):** Dengue virus was detected in a wastewater sample from Hawai'i Island (reported 3 Sep 2026) — a live, dated illustration of the wastewater-surveillance approach above being used operationally in a non-endemic-adjacent US setting. [Maui Now, 3 Sep](https://mauinow.com/2026/09/03/dengue-virus-detected-in-wastewater-sample-from-hawai%CA%BBi-island/)

## 8. Appendix

### 8.1 `movers.csv` (active snapshot, full table)

| iso3 | country | region | category | field | prior_value | current_value | delta |
|---|---|---|---|---|---|---|---|
| AFG | Afghanistan | South Asia | A | severity_interpretation | Rare bad event - unusually high cases to date | Above average - more cases than typical at this point | NA |
| ARG | Argentina | South America | A | severity_interpretation | Average - typical case load at this point | Below average - fewer cases than typical at this point | NA |
| BFA | Burkina Faso | Sub-Saharan Africa | A | severity_interpretation | Above average - more cases than typical at this point | Cannot determine | NA |
| BTN | Bhutan | South Asia | A | severity_interpretation | Average - typical case load at this point | Below average - fewer cases than typical at this point | NA |
| CIV | Cote D'ivoire | Sub-Saharan Africa | A | severity_interpretation | Average - typical case load at this point | Below average - fewer cases than typical at this point | NA |
| KNA | Saint Kitts And Nevis | Caribbean | A | severity_interpretation | Above average - more cases than typical at this point | Cannot determine | NA |
| MAF | Saint Martin | Caribbean | A | severity_interpretation | Below average - fewer cases than typical at this point | Rare good event - unusually low cases to date | NA |
| MRT | Mauritania | Sub-Saharan Africa | A | severity_interpretation | Average - typical case load at this point | Below average - fewer cases than typical at this point | NA |
| MYS | Malaysia | East & Southeast Asia | A | severity_interpretation | Average - typical case load at this point | Above average - more cases than typical at this point | NA |
| NPL | Nepal | South Asia | A | severity_interpretation | Average - typical case load at this point | Above average - more cases than typical at this point | NA |
| PYF | French Polynesia | Pacific Islands | A | severity_interpretation | Below average - fewer cases than typical at this point | Rare good event - unusually low cases to date | NA |
| REU | Reunion | Sub-Saharan Africa | A | severity_interpretation | Average - typical case load at this point | Below average - fewer cases than typical at this point | NA |
| SYC | Seychelles | Sub-Saharan Africa | A | severity_interpretation | Cannot determine | Below average - fewer cases than typical at this point | NA |
| TUV | Tuvalu | Pacific Islands | A | severity_interpretation | Average - typical case load at this point | Below average - fewer cases than typical at this point | NA |
| URY | Uruguay | South America | A | severity_interpretation | Below average - fewer cases than typical at this point | Average - typical case load at this point | NA |
| VNM | Viet Nam | East & Southeast Asia | A | severity_interpretation | Average - typical case load at this point | Above average - more cases than typical at this point | NA |
| WLF | Wallis And Futuna | Pacific Islands | A | severity_interpretation | Rare bad event - unusually high cases to date | Average - typical case load at this point | NA |
| AFG | Afghanistan | South Asia | B | monthly_ratio_descriptor | running well above | tracking near | NA |
| AUS | Australia | Pacific Islands | B | monthly_ratio_descriptor | running slightly below | running well below | NA |
| BFA | Burkina Faso | Sub-Saharan Africa | B | monthly_ratio_descriptor | running well above | running well below | NA |
| BOL | Bolivia | South America | B | monthly_ratio_descriptor | running slightly below | tracking near | NA |
| BRA | Brazil | South America | B | monthly_ratio_descriptor | running slightly above | running well above | NA |
| COL | Colombia | South America | B | monthly_ratio_descriptor | running well below | running slightly above | NA |
| ETH | Ethiopia | Sub-Saharan Africa | B | monthly_ratio_descriptor | running slightly below | running well below | NA |
| FJI | Fiji | Pacific Islands | B | monthly_ratio_descriptor | running slightly below | running well below | NA |
| GRD | Grenada | Caribbean | B | monthly_ratio_descriptor | running well below | running well above | NA |
| MHL | Marshall Islands | Pacific Islands | B | monthly_ratio_descriptor | running well below | running slightly above | NA |
| NCL | New Caledonia | Pacific Islands | B | monthly_ratio_descriptor | running well above | running well below | NA |
| PAN | Panama | North & Central America | B | monthly_ratio_descriptor | running slightly below | running well above | NA |
| SEN | Senegal | Sub-Saharan Africa | B | monthly_ratio_descriptor | running well above | running slightly below | NA |
| TLS | Timor-Leste | East & Southeast Asia | B | monthly_ratio_descriptor | running well above | running well below | NA |
| USA | United States Of America | North & Central America | B | monthly_ratio_descriptor | running slightly below | running well above | NA |
| VNM | Viet Nam | East & Southeast Asia | B | monthly_ratio_descriptor | running well below | running well above | NA |
| VUT | Vanuatu | Pacific Islands | B | monthly_ratio_descriptor | running well above | running well below | NA |
| WLF | Wallis And Futuna | Pacific Islands | B | monthly_ratio_descriptor | running well above | running well below | NA |
| GUY | Guyana | South America | C | current_season_percentile | 96.7 | 5.9 | −90.78 |
| WSM | Samoa | Pacific Islands | C | current_season_percentile | 59.8 | 6.3 | −53.48 |
| CIV | Cote D'ivoire | Sub-Saharan Africa | C | current_season_percentile | 35.8 | 10.0 | −25.81 |
| MYS | Malaysia | East & Southeast Asia | C | current_season_percentile | 24.7 | 56.7 | +31.98 |
| VNM | Viet Nam | East & Southeast Asia | C | current_season_percentile | 2.4 | 32.6 | +30.27 |
| SDN | Sudan | Europe, Middle East & North Africa | C | current_season_percentile | 81.2 | 61.2 | −19.97 |
| KIR | Kiribati | Pacific Islands | C | current_season_percentile | 40.7 | 22.8 | −17.82 |
| AFG | Afghanistan | South Asia | C | current_season_percentile | 51.0 | 33.2 | −17.75 |
| ARG | Argentina | South America | C | current_season_percentile | 22.3 | 10.7 | −11.55 |
| REU | Reunion | Sub-Saharan Africa | C | current_season_percentile | 10.1 | 21.3 | +11.20 |

### 8.2 Consolidated citation list

1. PressReader/Viet Nam News, dengue fever cases surge with more than 1,000 new infections (21 Sep) — https://www.pressreader.com/vietnam/viet-nam-news/20260921/281548002800575
2. TechTimes, dengue cases in Vietnam have doubled: adults now face greater risk than children (3 Aug) — https://www.techtimes.com/articles/322818/20260803/dengue-cases-vietnam-have-doubled-adults-now-face-greater-risk-children.htm
3. Dengue Visual Atlas, 78,000 cases of dengue in Vietnam in 2026, 20% more than the previous year — https://denguevisualatlas.com/en/78000-cases-of-dengue-in-vietnam-in-2026-20-more-than-the-previous-year/
4. VOA News, dengue fever outbreak confirmed in Afghanistan, WHO says (background) — https://www.voanews.com/a/dengue-fever-outbreak-confirmed-in-afghanistan-who-says-/6688911.html
5. Malay Mail, dengue cases soar 66pc, deaths hit 62 in Malaysia (9 Sep) — https://www.malaymail.com/news/malaysia/2026/09/09/dengue-cases-soar-66pc-deaths-hit-62-in-malaysia-almost-double-2025-toll/234576
6. PressReader/The Straits Times, dengue cases spike in Malaysia, with 55 deaths so far in 2026 (22 Aug) — https://www.pressreader.com/singapore/the-straits-times/20260822/281659671884700
7. La 1ère, dengue: l'épidémie ralentit à Futuna mais progresse à Wallis (17 Jul) — https://la1ere.franceinfo.fr/wallisfutuna/dengue-l-epidemie-ralentit-a-futuna-mais-progresse-a-wallis-1711747.html
8. Argentina.gob.ar, Boletines Epidemiológicos Nacionales 2026 — https://www.argentina.gob.ar/salud/boletin-epidemiologico-nacional/boletines-2026
9. LA NACION, las claves detrás de la baja de casos de dengue y las alertas de los especialistas — https://www.lanacion.com.ar/sociedad/las-claves-detras-de-la-baja-de-casos-de-dengue-y-las-alertas-de-los-especialistas-nid03022026/
10. Wakat Séra, Burkina: une augmentation inhabituelle et rapide de cas de dengue à Ziniaré et Zorgho (10 Sep) — https://www.wakatsera.com/burkina-une-augmentation-inhabituelle-et-rapide-de-cas-de-dengue-a-ziniare-et-zorgho/
11. World Mosquito Program, Timor-Leste — https://www.worldmosquitoprogram.org/global-progress/timor-leste
12. WHO, Disease Outbreak News: Dengue – Timor-Leste — https://www.who.int/emergencies/disease-outbreak-news/item/dengue---timor-leste
13. Infobae, Panamá registra 7,565 casos acumulados de dengue y baja las hospitalizaciones en 14.5% (16 Sep) — https://www.infobae.com/panama/2026/09/16/panama-registra-7565-casos-acumulados-de-dengue-y-baja-las-hospitalizaciones-en-145/
14. Infobae, los casos de dengue aumentaron 7,1% en una semana en Panamá (10 Sep) — https://www.infobae.com/panama/2026/09/10/los-casos-de-dengue-aumentaron-71-en-una-semana-en-panama/
15. Ministère de la Santé de Côte d'Ivoire, 6è épidémie de dengue en Côte d'Ivoire — https://sante.gouv.ci/actualite/1559
16. NOW Grenada, Ministry of Health urges vigilance amid increase in dengue cases (Aug 2026) — https://nowgrenada.com/2026/08/ministry-of-health-urges-vigilance-amid-increase-in-dengue-cases/
17. Social News XYZ, Bangladesh reports 87 dengue deaths in September, highest monthly toll this year (21 Sep) — https://www.socialnews.xyz/2026/09/21/bangladesh-reports-87-dengue-deaths-in-september-highest-monthly-toll-this-year
18. Xinhua, Bangladesh reports 87 dengue deaths in September, highest monthly toll this year (21 Sep) — https://english.news.cn/20260921/600a67d1e27b42479ce6da5ead7cf6cf/c.html
19. Weather.com, Florida confirms a death from dengue fever amid outbreak (19 Sep) — https://weather.com/2026/09/19/health/florida-confirms-death-dengue-amid-outbreak
20. Florida Department of Health, Arbovirus Surveillance Week 36: September 6–12, 2026 — https://www.floridahealth.gov/wp-content/uploads/2026/09/fl-arbovirus-report-w36-2026.pdf
21. Outbreak News Today, Cebu reports rise in dengue in 2026 — https://outbreaknewstoday.substack.com/p/cebu-reports-rise-in-dengue-in-2026
22. PAHO/WHO, Dengue Multi-Country Grade 3 Outbreak — https://www.paho.org/en/topics/dengue/dengue-multi-country-grade-3-outbreak
23. Connexion France, first native dengue fever cases recorded in France in 2026 — https://www.connexionfrance.com/news/first-native-dengue-fever-cases-recorded-in-france-in-2026/803099
24. PMC, climate-driven advanced machine learning approach for dengue incidence forecasting in Bangladesh — https://pmc.ncbi.nlm.nih.gov/articles/PMC13087637/
25. PMC, climate change and autochthonous vector-borne disease transmission in Europe: dengue as a sentinel signal — https://pmc.ncbi.nlm.nih.gov/articles/PMC13418699/
26. Happiest Health, India approves Qdenga, its first dengue vaccine — https://www.happiesthealth.com/articles/infectious-diseases/india-approves-dengue-vaccine-qdenga
27. Pathogens (MDPI), wastewater surveillance for early warning of infectious disease outbreaks: a systematic review — https://doi.org/10.3390/pathogens15070690
28. Maui Now, dengue virus detected in wastewater sample from Hawai'i Island (3 Sep) — https://mauinow.com/2026/09/03/dengue-virus-detected-in-wastewater-sample-from-hawai%CA%BBi-island/
