# GDO Internal News Report — 2026-10-26

*Source: Global Dengue Observatory (accessed 2026-10-26).*

## 1. Header

- **Report date:** 2026-10-26 (Monday routine run).
- **Active snapshot:** `snapshots/2026_10_19/` — **unchanged since 2026-10-19** (news-only week; no new pull this run). Source data vintage (`target_render_date`): 2026-10-18. Source commit `67e82815d1cd625144c4021f338992c0ba6a31ee` (`DENV_global_observatory` `Output/2026_10_18/`, no fallback used). Prior snapshot: `snapshots/2026_10_05/` (vintage 2026-10-04).
- **Pull status this week:** **news-only week.** `target_render_date` for this run computes to 2026-10-18 (most recent of {this month's 4th = 2026-10-04, this month's 18th = 2026-10-18, last month's 18th = 2026-09-18}, all strictly before today, 2026-10-26). That matches the vintage already recorded in `snapshots/2026_10_19/manifest.json` — no new render has happened on the public site since the last pull, so Step 1's fetch/diff was skipped per Step 0.5, and this run reuses `snapshots/2026_10_19/` (including its `movers.csv`, a 2026-10-05 → 2026-10-19 comparison) as the active snapshot.
- **Countries covered:** 85.
- **Environment note:** this session's container had no R runtime pre-installed. Per the routine's Step 0 fallback, `apt-get update && apt-get install -y --no-install-recommends r-base-core r-cran-httr r-cran-jsonlite r-cran-dplyr r-cran-readr r-cran-tibble` was run as a single attempt and succeeded cleanly (R 4.3.3; all five required packages load without error). This wasn't otherwise needed this run, since Step 1 (the R pipeline) is skipped on a news-only week. `gh` CLI is on `PATH` (v2.89.0) but `gh auth status` failed ("the token in GH_TOKEN is invalid"); GitHub operations instead used the `mcp__github__*` tools, confirmed working (`get_me` succeeded, authenticated as `KMSusong`). `git push`/write access is recorded at Step 7 below.
- **Data-integrity note:** last week's report (`reports/2026_10_19_gdo_internal_news_report.md`, Section "News — targeted") quoted Sudan's cumulative percentile as 78.5 and the United States' as 94.5. Re-reading `snapshots/2026_10_19/latest_status.csv` directly this run shows these two figures are **transposed** in that write-up — the correct verbatim values are **Sudan 94.53** (High band, just under the 95-point Extremely High cutoff) and **United States 78.46** (High band). The underlying data file and both countries' `severity` labels ("High") are correct and unaffected; only last week's narrative prose swapped the two numbers between countries. Flagging for the researcher; this report uses the correct verbatim values throughout (see Section 3).

---

## 2. This week's snapshot

Global picture across the 85 tracked countries/territories, from `latest_status.csv` only. These figures are identical to last week's report — the underlying data hasn't changed (see Header) — reproduced here in full per the routine's structure.

**Cumulative severity band** (`percentile_cumulative`, current position vs. seasonal-to-date expectation):

| Band | Countries |
|---|---|
| Normal | 28 |
| Low | 23 |
| High | 14 |
| Extremely High | 9 |
| Unknown | 6 |
| Extremely Low | 5 |

The 9 at **Extremely High** cumulative severity: Cook Islands, Cuba, Guyana, Kenya, Cambodia, Sri Lanka, Maldives, Peru and Timor-Leste.

**Current-season severity band** (`current_season_percentile`, i.e. how this season is tracking overall):

| Band | Countries |
|---|---|
| Low | 36 |
| Normal | 26 |
| Extremely Low | 10 |
| Unknown | 6 |
| High | 4 |
| Extremely High | 3 |

Current-season **Extremely High**: Cuba (100.0), Kenya (100.0), Cambodia (99.8). Current-season **High**: Maldives (91.9), Sri Lanka (89.1), Bangladesh (81.0), United Republic of Tanzania (81.5) — a reminder that cumulative and current-season severity tell different stories and shouldn't be conflated (e.g. Guyana and Timor-Leste are cumulative-Extremely-High but don't appear on the current-season High/Extremely-High lists at all).

Regionally, East & Southeast Asia and South Asia carry the most concentrated High/Extremely-High load (East & SE Asia: 3 High, 2 Extremely High out of 9 countries; South Asia: 2 High, 2 Extremely High out of 8), with the Caribbean and South America each showing smaller but still notable Extremely-High pockets (1 and 2 countries respectively, against otherwise mixed Low/Normal pictures).

**Caveat — data recency.** This snapshot is now a week older than when it was first reported (2026-10-19) without a re-pull. Of this week's ten targeted countries (Section 3), China's `latest_observed_date` is 2026-08-01 (~2.9 months stale as of today, beyond GDO's 1–2 month nowcast sweet spot); the other nine sit at 2026-09-01 (~1.9 months stale, at the outer edge of the sweet spot) except Mauritania, which sits at 2026-07-01 (~3.9 months stale). **Small-baseline/large-ratio instability:** Jamaica's reported case count this period is a single case against a ~263-case seasonal baseline, and French Guiana's is zero cases against a ~119-case baseline — both too small a sample to read the underlying severity-band move as a strong signal on its own.

---

## 3. News — targeted (10 countries)

**Selection note:** this is a news-only week reusing the active snapshot's existing `movers.csv` (a 2026-10-05 → 2026-10-19 comparison): 9 Category A rows and 7 Category B rows, 15 unique countries once de-duplicated (China appears in both categories) — more than the 10-country cap. Per the routine's instructions, Category A/B band-crossings are prioritised over Category C. All 9 Category A countries — China, French Guiana, Honduras, Jamaica, Mexico, Mauritania, Peru, Sudan and the United States — take 9 of the 10 slots; the 10th goes to Brazil (Category B), whose swing from "running well below" to "running well above" is a two-band jump, the single largest Category B move this week and the most newsworthy of the remaining B-only movers (Colombia, Grenada, Guyana, India, Viet Nam). What follows is a **fresh news search** for each (last ~2 weeks, 2026-10-12 to 2026-10-26); the GDO figures themselves are unchanged from last week.

### China (CHN) — category A (also category B)

GDO's severity-interpretation read firmed from **"Cannot determine"** to **"Above average – more cases than typical at this point"** (percentile_cumulative 81.4, High band; cases=836). Interestingly, the monthly-ratio descriptor moved in the *opposite* direction over the same pull — "running well above" → "running slightly below" — meaning the most recent observed month actually eased even as the season-to-date position firmed into "above average." Current-season reading stays Normal (percentile 51.8, "Average"). **Caveat:** `latest_observed_date` here is 2026-08-01, ~2.9 months stale as of this report — beyond GDO's 1–2 month nowcast sweet spot, so treat the August-derived band crossing as the least current of this week's targeted moves. News corroboration is thin and lags further still: a WHO Western Pacific update puts China's July 2026 national count at 1,120 cases (up sharply from 255 in June, and 61.4% above July 2025), and a China CDC seasonality study (2005–2023) finds national case counts typically peak in September–October (around epidemiological week 40) — consistent with, but not confirming, an "above average" autumn. No October-dated figures were found this cycle.
*Source: [WHO Western Pacific dengue situation update](https://cdn.who.int/media/docs/default-source/wpro---documents/emergency/surveillance/dengue/dengue_20260820.pdf); [China CDC Weekly, dengue seasonality 2005–2023](https://weekly.chinacdc.cn/en/article/pdf/preview/10.46234/ccdcw2024.217) (background; no October figure).*

### French Guiana (GUF) — category A

Moved from **"Rare good event – unusually low cases to date"** to **"Below average – fewer cases than typical at this point"** — still a quiet dengue picture, just marginally less extreme (percentile_cumulative 5.6, Low band). **Small-baseline caveat:** this move is from a reported case count of 0 against a ~119-case seasonal baseline — there is essentially no case signal underlying the shift, so read the band change as a statistical normalisation rather than a real uptick. News confirms dengue is a non-story locally right now: Santé publique France's most recent regional bulletin (16 October 2026) reports dengue activity staying low, with chikungunya the active local concern instead — 2,096 cumulative lab-confirmed chikungunya cases since late January, with the West Coast sector post-epidemic since week 38 but the Savanes sector still in active epidemic phase. An earlier bulletin (21 August) recorded only 12 lab-confirmed dengue cases for the whole of 2026 to that point.
*Source: [Santé publique France, French Guiana bulletin, 16 October 2026](https://www.santepubliquefrance.fr/en/regions-and-territories/french-guiana/regional-bulletin/chikungunya-and-dengue-french-guiana-bulletin-dated-october-16-2026); [Santé publique France, French Guiana bulletin, 21 August 2026](https://www.santepubliquefrance.fr/en/regions-and-territories/french-guiana/regional-bulletin/chikungunya-and-dengue-french-guiana-bulletin-dated-august-21-2026).*

### Honduras (HND) — category A

Moved from **"Average – typical case load at this point"** to **"Below average – fewer cases than typical at this point"** (percentile_cumulative 24.6, Low band — just under the Normal cutoff). **Caveat:** `latest_observed_date` is 2026-09-01, ~1.9 months stale — at the outer edge of GDO's nowcast sweet spot. The most current news found is La Tribuna's 13 October report: five deaths from severe dengue confirmed in 2026 with a sixth under investigation, and a national cumulative count of 10,749 cases for the year. That builds on a mid-August figure of 9,643 cases through epidemiological week 31 — already described then as a roughly 40% reduction on the same period in 2025 — with Distrito Central, San Pedro Sula, Olancho, Choluteca and Yoro running above the national incidence average. **Caveat:** case totals aren't perfectly consistent across outlets and cutoff dates; treat the easing direction, not an exact figure, as the reliable read, broadly consistent with GDO's own "Average → Below average" move.
*Source: [La Tribuna, 13 October 2026](https://www.latribuna.hn/2026/10/13/honduras-reporta-cinco-muertes-por-dengue-grave-en-2026-e-investiga-otro-fallecimiento/); [La Tribuna, 18 August 2026](https://www.latribuna.hn/2026/08/18/honduras-reporta-9643-casos-de-dengue-13-de-sarampion-y-228-de-tosferina/); [La Prensa, Honduras dengue figures](https://www.laprensa.hn/honduras/dengue-cifras-salud-casos-estadisticas-prevencion-ME30075108).*

### Jamaica (JAM) — category A

Moved from **"Average – typical case load at this point"** to **"Below average – fewer cases than typical at this point"** (percentile_cumulative 19.8, Low band). **Small-baseline caveat:** the underlying reported case count is 1, against a seasonal baseline of ~263 — a single observed case driving a band crossing is not a trend in itself, however the classification reads. No 2026-dated, Jamaica-specific news was found this cycle: PAHO's regional bulletin records over 1.2 million suspected dengue cases across the Americas so far in 2026 (down sharply on the same period of 2025) but doesn't break out Jamaica, and the most recent Jamaica-specific figure available dates to January–April 2025. Jamaica's last well-documented outbreak remains 2023. This is a genuine, unresolved news gap rather than a settled "quiet" story — worth a direct Ministry of Health and Wellness or PAHO country-dashboard check before using in a social post.
*Source: no current (2026) Jamaica-specific news corroboration found; [PAHO, Dengue Epidemiological Situation, Region of the Americas](https://www.paho.org/en/documents/situation-report-no-20-dengue-epidemiological-situation-region-americas-epidemiological); [Statista, Jamaica dengue incidence](https://www.statista.com/statistics/1463264/dengue-cases-incidence-rate-jamaica).*

### Mexico (MEX) — category A

Moved from **"Below average – fewer cases than typical at this point"** to **"Average – typical case load at this point"** (percentile_cumulative 28.8, Normal band). **Caveat:** `latest_observed_date` is 2026-09-01, ~1.9 months stale. No October-dated national figure was found this cycle; the most recent confirmed national cut remains epidemiological week 32 (to 17 August): 4,152 confirmed cases and 7 deaths, with Sonora, Veracruz, Tabasco, Sinaloa and Quintana Roo together accounting for 72% of cases. State-level reporting for the State of México through the same week describes a declining 2026 trend, broadly consistent with GDO's own figures sitting in "typical" territory rather than an escalation. Separately, Mexico's health authorities added a tetravalent dengue vaccine to the national compendium of health supplies — a formulary listing, not yet a national vaccination campaign.
*Source: [Excélsior, 17 August 2026](https://www.excelsior.com.mx/nacional/dengue-mexico-2026); [Posta, Edomex dengue cases declining](https://www.posta.com.mx/edomex/dengue-en-edomex-2026-bajan-contagios/vl2249684).*

### Mauritania (MRT) — category A

GDO: cumulative severity interpretation moved **"Below average – fewer cases than typical at this point"** to **"Average – typical case load at this point"** (Normal band, percentile_cumulative 29.3). Cases=36, `latest_observed_date` 2026-07-01 — ~3.9 months stale, well beyond GDO's 1–2 month nowcast sweet spot, so treat this move cautiously. Current-season percentile sits higher, at 72.5 ("Average"), a reminder the current-season read is less lagged than the cumulative one. No 2026-dated figures turned up this cycle — the freshest confirmed numbers remain a 3 December 2025 bulletin: 7,280 suspected cases (4,050 confirmed) and one death since a May-2025-onset outbreak spanning 13 of 15 regions. An undated feature describes a severe, under-reported outbreak in Nouakchott's Teyarett suburb, but carries no dateline tying it to 2026. **Caveat:** given the ~4-month data gap and no corroborating current reporting, this week's "Average" read is the only live signal — not independently confirmed either way.
*Source: [TravelHealthPro, Mauritania outbreak update, 3 December 2025](https://travelhealthpro.org.uk/updates.php?base=4999); [The New Arab, Dengue fever devastates Mauritania's capital](https://newarab.com/analysis/dengue-fever-devastates-mauritanias-capital) (undated, not confirmed current).*

### Peru (PER) — category A (also category C)

GDO: cumulative severity moved "Above average" → **"Rare bad event – unusually high cases to date"** (percentile_cumulative 97.9, Extremely High); current-season percentile also jumped 19.9 → 49.1, the largest Category C move in this snapshot (+29.2 pts). Cases=7,685, `latest_observed_date` 2026-09-01 (~1.9 months stale). No October-dated figures surfaced this cycle — the latest confirmed official data remains MINSA's week-33 bulletin (to ~22 August 2026): 46,669 cumulative cases and 57 deaths (46 confirmed, 11 under investigation) — already exceeding all of 2025's death toll, against 30,587 cases over the same period in 2025. Piura remains hardest-hit. Peru's CDC director has said the ministry is modelling scenarios up to a 2023/2024-scale severe season and warned high temperatures could push cases further; the vaccination strategy has been extended to ages 10–16. **Caveat:** nothing newer than late August was found, so GDO's own jump to Extremely High is the most current signal available — the direction matches MINSA's own warnings, but the precise scale of any September/October rise is unconfirmed.
*Source: [Canal N, casos de dengue aumentan en Perú (MINSA)](https://canaln.pe/actualidad/casos-dengue-aumentan-79-peru-minsa-advierte-que-podrian-incrementarse-altas-temperaturas-n495247); [MINSA/DGE, Sala de Situación Dengue, Semana Epidemiológica 33, 2026](https://www.dge.gob.pe/portal/docs/vigilancia/sala/2026/SE33/dengue.pdf).*

### Sudan (SDN) — category A (also category C)

GDO: cumulative severity moved "Rare bad event – unusually high cases to date" → **"Above average – more cases than typical at this point"** — an improvement in relative terms, though the country remains High severity overall (percentile_cumulative **94.5**, just under the 95-point Extremely High cutoff — see Header for a correction to last week's transposed figure). Current-season percentile eased 83.9 → 72.6 (−11.3 pts). Cases=2,636, `latest_observed_date` 2026-09-01 (~1.9 months stale). The live story has shifted location since last week: Blue Nile's late-July outbreak is no longer the most current item. A displaced-persons coordination group reported over 500 dengue cases in Tawila, North Darfur, on 12 October 2026, revised to 927 cases (September–16 October) in a 16–17 October update, warning of a severe medicine shortage and suspended services at several health centres — Tawila hosts a large, rapidly growing displaced population fleeing conflict across Darfur. **Caveat:** these figures come from a displaced-persons advocacy group, not an official health ministry or WHO count, and conflict-disrupted surveillance means small-baseline/large-swing instability is a live risk — read the direction (worsening in Darfur specifically, easing nationally per GDO) with caution, not the precise numbers.
*Source: [Sudan Tribune, 12 October 2026](https://sudantribune.com/?p=319868); [Sudan Tribune, 17 October 2026](https://sudantribune.com/?p=320054).*

### United States (USA) — category A (also category C)

GDO: cumulative severity moved "Average" → **"Above average – more cases than typical at this point"** (percentile_cumulative **78.5**, High band — see Header for a correction to last week's transposed figure). Current-season percentile also rose 52.4 → 58.5. Cases=339, `latest_observed_date` 2026-09-01 (~1.9 months stale). Florida's outbreak keeps climbing: the Florida Department of Health's week-40 arbovirus report (4–10 October 2026) counts 368 locally-acquired dengue cases for the year across eight counties, up from 296 at week 39, with 72 new cases in week 40 alone, alongside a separate travel-associated tally of 262 cases. One death has been confirmed (an 80-year-old Tampa resident). Coverage continues to call this the most cases in a single US state in a calendar year since at least the 1940s, surpassing Florida's own 2023 record. **Caveat, carried from prior reports:** this is a sharply Florida-concentrated story — the national resident count doesn't resolve cleanly against the state local-transmission figures, so frame any post around Florida specifically, not a US-wide trend.
*Source: [Florida Department of Health, Arbovirus Surveillance Report, Week 40 2026](https://www.floridahealth.gov/wp-content/uploads/2026/10/fl-arbovirus-report-w40-2026.pdf); [WGCU, dengue fever cases on the rise in Florida, 9 October 2026](https://www.wgcu.org/health/2026-10-09/dengue-fever-cases-on-the-rise-in-florida).*

### Brazil (BRA) — category B

GDO: monthly ratio descriptor swung "running well below" → **"running well above"** — a two-band jump, the single largest Category B move in this snapshot. Cases=63,952 (`latest_observed_date` 2026-09-01). Cumulative severity remains Normal (percentile_cumulative 52.6) — not Extremely High; current-season severity is Extremely Low (percentile ≈0, "Rare good event – unusually low cases to date"), so "running well above" is a relative-to-seasonal-baseline read for an otherwise quiet season, not evidence of a return to a major outbreak. PAHO's 20–21 October update calls on countries across the Americas to strengthen surveillance ahead of South America's peak season and an anticipated El Niño intensification, citing rising dengue in the Andean, Central American and Caribbean subregions plus renewed chikungunya transmission; PAHO's own regional figures (to mid-September) put the Americas at 1.69 million suspected cases and 571 deaths — a 58% decrease on the same period in 2025. **Caveat:** no Brazil-specific case count newer than a week-20 third-party figure was found — this week's GDO signal is corroborated in direction (PAHO flags a genuine regional uptick) but not independently confirmed for Brazil specifically at a comparable, current cutoff.
*Source: [PAHO, calls for strengthened surveillance and preparedness amid increases in dengue and chikungunya in the Americas, 21 October 2026](https://www.paho.org/en/news/21-10-2026-paho-calls-strengthened-surveillance-and-preparedness-amid-increases-dengue-and); [PAHO, Epidemiological Update: Dengue and Chikungunya in the Americas Region, 20 October 2026](https://www.paho.org/en/documents/epidemiological-update-dengue-and-chikungunya-americas-region-20-october-2026); [mappr.co, Dengue Outbreak 2026: Cases by Country](https://www.mappr.co/dengue-outbreak-map/).*

---

## 4. News — general scan (5 items)

Independent broad scan, capped at 5, for the last ~2 weeks (2026-10-12 to 2026-10-26); includes GDO-tracked countries outside this week's 10-country target list and non-endemic settings per the routine's instruction. Chosen to avoid repeating stories already well-covered in the past two reports (Cuba, Sri Lanka, Maldives-linked imported EU cases, Marshall Islands).

1. **Region-wide, Americas — PAHO's week-38 update (20 October 2026).** PAHO's latest regional situation report puts the cumulative 2026 dengue total at 1,782,016 suspected cases across 45 reporting countries/territories (273 per 100,000 population), with 552,904 laboratory-confirmed, 3,736 severe cases and 604 deaths — down 55% on the same point in 2025 and 62% below the five-year average. All four serotypes are circulating regionally, with Colombia, Brazil, Venezuela, Mexico and Panama confirmed co-circulating all four. The accompanying epidemiological update flags rising dengue in parts of the Andean, Central American/Mexico and Caribbean subregions ahead of an approaching El Niño-linked peak season. *[PAHO, Epidemiological Update, 20 October 2026](https://www.paho.org/en/documents/epidemiological-update-dengue-and-chikungunya-americas-region-20-october-2026); [week 38 situation report](https://www.paho.org/sites/default/files/2026/10/2026-cde-dengue-sitrep-americas-epi-week-38-oct.pdf).*
2. **Khyber Pakhtunkhwa, Pakistan — single-day record.** Provincial health officials reported 99 new dengue cases in 24 hours on 20 October, the highest single-day tally of 2026, bringing KP's cumulative total to 4,091. Kohat district remains worst-affected with 2,567 cases to date; officials warned current mosquito-breeding conditions could push numbers higher in the coming weeks. Pakistan is GDO-tracked but wasn't among this week's 10 targeted countries — a reminder that national-level nowcasts can mask sharp sub-national spikes like this one. *[ProPakistani, 20 October 2026](https://propakistani.pk/2026/10/20/kp-reports-highest-single-day-dengue-cases-of-2026/).*
3. **Europe — locally-acquired cases, a different angle from the usual imported-case story.** As of 2 September 2026, ECDC data recorded five dengue cases acquired locally within France and three in Italy — the Italian cases the first autochthonous transmission of the season there, across two separate clusters. Distinct from the Maldives-linked imported-case story covered in recent reports: these are mosquito-borne infections within Europe itself, not travel-associated, though ECDC continues to assess onward local-transmission risk as low given currently unfavourable *Aedes* conditions. *[Quotidiano Sanità, ECDC: 8 casi autoctoni in Europa nel 2026](https://www.quotidianosanita.it/scienza-e-farmaci/dengue-ecdc-8-casi-autoctoni-in-europa-nel-2026-segnalazioni-in-francia-e-italia/).*
4. **Americas — chikungunya co-circulation, compounding pressure.** Alongside the dengue totals above, PAHO's week-38 reporting cycle recorded 213,919 suspected chikungunya cases across 20 countries in 2026 (78,481 laboratory-confirmed, 88 deaths) — a second *Aedes*-borne virus straining the same surveillance and vector-control systems as dengue, in several of the same hard-hit countries (Brazil, Colombia). Useful context for why regional health authorities are emphasising combined vector control rather than disease-specific responses. *[PAHO, week 38 situation report](https://www.paho.org/sites/default/files/2026/10/2026-cde-dengue-sitrep-americas-epi-week-38-oct.pdf).*
5. **Nashik and Delhi, India — early-October city-level counts.** Nashik recorded 82 new dengue cases in the first 20 days of October 2026, bringing its 2026 total to 264. Delhi logged 98 new cases in the first week of October, taking its cumulative tally to 695, with no dengue deaths reported in the capital so far this year. India is GDO-tracked but wasn't among this week's 10 targeted countries; these city-level figures are too granular to compare directly against GDO's national-level nowcast, but both point to continued transmission into the back half of the season. *[Free Press Journal, Nashik](https://www.freepressjournal.in/pune/nashik-82-new-dengue-cases-reported-in-october-total-count-reaches-264); [The Hans India, Delhi](https://www.thehansindia.com/news/cities/new-delhi/delhi-98-dengue-cases-in-1st-week-of-oct-tally-touches-695-1129800).*

---

## 5. Trend since last update

No new GDO data this week — `latest_status.csv` and `movers.csv` are unchanged from the 2026-10-19 report (news-only week; see Header). For completeness, the active `movers.csv` (a 2026-10-05 → 2026-10-19 comparison) breaks down as:

**Category A — severity-band crossings (9 countries)**

| Country | Prior | Current |
|---|---|---|
| China | Cannot determine | Above average |
| French Guiana | Rare good event (unusually low) | Below average |
| Honduras | Average | Below average |
| Jamaica | Average | Below average |
| Mexico | Below average | Average |
| Mauritania | Below average | Average |
| Peru | Above average | Rare bad event (unusually high) |
| Sudan | Rare bad event (unusually high) | Above average |
| United States | Average | Above average |

**Category B — monthly-ratio-descriptor crossings (7 countries)**

| Country | Prior | Current |
|---|---|---|
| Brazil | running well below | running well above |
| China | running well above | running slightly below |
| Colombia | running well below | tracking near |
| Grenada | running well below | tracking near |
| Guyana | running well below | running slightly above |
| India | tracking near | running slightly above |
| Viet Nam | running well above | running slightly above |

**Category C — current-season percentile movers:** 10 countries flagged (largest absolute moves: Peru +29.2 pts, Australia −46.3 pts, Sudan −11.3 pts). Full list in Appendix.

---

## 6. Social-media candidate flags

Ranked short-list, for the researcher drafting Tuesday's posts.

1. **Peru — the cleanest, strongest signal this week.** A category A *and* C crossing in the same direction (cumulative now Extremely High, current-season percentile up nearly 30 points), corroborated by MINSA's own case/death figures and explicit ministry warnings of further rises. *Caveat: cite the direction of change, not a single precise growth percentage — MINSA's own figures and press summaries of them vary by cutoff date.*
2. **Florida, United States — outbreak keeps climbing, now with an updated county/week count.** 368 locally-acquired cases through week 40, up from 296 two weeks prior, one confirmed death — still described as the largest single-state outbreak since at least the 1940s. *Caveat: frame as a Florida/subnational story, not a US-wide trend — the national resident count doesn't move in step with Florida's local-transmission figures.*
3. **Sudan — the story has moved to Darfur.** A displaced-persons dengue outbreak in Tawila, North Darfur (500+ cases reported 12 October, revised to 927 by 17 October) amid a severe medicine shortage is a compelling humanitarian angle, distinct from the Blue Nile story flagged in recent weeks. *Caveat: figures come from a displaced-persons advocacy group, not an official count, and conflict-disrupted surveillance makes exact numbers unstable — lead with the humanitarian/access angle rather than precise case counts.*
4. **Americas region-wide — the "quiet regional average, loud local exceptions" post.** PAHO's week-38 data shows the region overall running well below both 2025 and the five-year average, even as Peru, Sudan and Florida (all above) post sharp local escalations — good material for a post about regional aggregates masking country-level divergence, with Brazil's own category-B "running well above" move as a live example. *No major caveat — PAHO is an independent, authoritative regional source.*
5. **Khyber Pakhtunkhwa, Pakistan — a vivid single-day record.** 99 new cases in 24 hours, the highest single-day tally of 2026 for the province, concentrated in Kohat district. *Caveat: Pakistan isn't among this week's GDO-targeted countries and this is a provincial, not national, figure — frame as a local spike, not a national trend shift.*

---

## 7. Scientific literature findings

Lighter-effort pass; a handful of recent items across forecasting, climate, surveillance and vaccine policy.

- **Forecasting (multi-country):** A new peer-reviewed framework automates dengue forecasting by combining surveillance, climate, environmental and demographic data into an ensemble model; temperature, precipitation variability and urban-environment indicators emerged as the dominant predictive drivers, with the ensemble outperforming any single constituent model. [PNNL, 1 October 2026](https://www.pnnl.gov/publications/environmental-and-epidemiological-drivers-dengue-forecasting-across-heterogeneous)
- **Climate drivers (systematic review):** A PRISMA-based systematic review confirms temperature and rainfall as the most commonly studied dengue climate drivers in the literature, but flags considerable heterogeneity in lag structures and modelling choices between studies — a caution against treating any single model's thresholds as universal. [Vacunas, Jul–Sep 2026](https://www.elsevier.es/es-revista-vacunas-72-articulo-predicting-dengue-in-changing-climate-S1576988726000233)
- **Vaccine policy (Singapore):** Singapore's Ministry of Health confirmed in September 2026 that Dengvaxia's manufacturer has discontinued the vaccine globally due to weak demand, not a safety signal; MOH will keep monitoring newer-generation dengue vaccines, with no further action needed for those who already completed dosing. [MOH Singapore](https://www.moh.gov.sg/newsroom/discontinuation-of-dengvaxia-and-ongoing-monitoring-of-dengue-vaccines/)
- **Vaccine policy (Brazil) — an update on a previously open question:** prior reports flagged that Brazil's Butantan-DV single-dose vaccine had no confirmed national-programme rollout date. Government sources now report it is confirmed for inclusion in the national health system (SUS) programme within 2026, though an exact start date remains unclear. [tnh1.com.br](https://www.tnh1.com.br/noticia/nid/vacina-brasileira-contra-dengue-estara-no-sus-em-2026-diz-governo/)

---

## 8. Appendix

### 8.1 `movers.csv` (active snapshot, full table — unchanged from the 2026-10-19 report)

| iso3 | country | region | category | field | prior_value | current_value | delta |
|---|---|---|---|---|---|---|---|
| CHN | China | East & Southeast Asia | A | severity_interpretation | Cannot determine | Above average – more cases than typical at this point | NA |
| GUF | French Guiana | South America | A | severity_interpretation | Rare good event – unusually low cases to date | Below average – fewer cases than typical at this point | NA |
| HND | Honduras | North & Central America | A | severity_interpretation | Average – typical case load at this point | Below average – fewer cases than typical at this point | NA |
| JAM | Jamaica | Caribbean | A | severity_interpretation | Average – typical case load at this point | Below average – fewer cases than typical at this point | NA |
| MEX | Mexico | North & Central America | A | severity_interpretation | Below average – fewer cases than typical at this point | Average – typical case load at this point | NA |
| MRT | Mauritania | Sub-Saharan Africa | A | severity_interpretation | Below average – fewer cases than typical at this point | Average – typical case load at this point | NA |
| PER | Peru | South America | A | severity_interpretation | Above average – more cases than typical at this point | Rare bad event – unusually high cases to date | NA |
| SDN | Sudan | Europe, Middle East & North Africa | A | severity_interpretation | Rare bad event – unusually high cases to date | Above average – more cases than typical at this point | NA |
| USA | United States Of America | North & Central America | A | severity_interpretation | Average – typical case load at this point | Above average – more cases than typical at this point | NA |
| BRA | Brazil | South America | B | monthly_ratio_descriptor | running well below | running well above | NA |
| CHN | China | East & Southeast Asia | B | monthly_ratio_descriptor | running well above | running slightly below | NA |
| COL | Colombia | South America | B | monthly_ratio_descriptor | running well below | tracking near | NA |
| GRD | Grenada | Caribbean | B | monthly_ratio_descriptor | running well below | tracking near | NA |
| GUY | Guyana | South America | B | monthly_ratio_descriptor | running well below | running slightly above | NA |
| IND | India | South Asia | B | monthly_ratio_descriptor | tracking near | running slightly above | NA |
| VNM | Viet Nam | East & Southeast Asia | B | monthly_ratio_descriptor | running well above | running slightly above | NA |
| AUS | Australia | Pacific Islands | C | current_season_percentile | 46.3 | 0 | −46.32 |
| PER | Peru | South America | C | current_season_percentile | 19.9 | 49.1 | +29.22 |
| SDN | Sudan | Europe, Middle East & North Africa | C | current_season_percentile | 83.9 | 72.6 | −11.34 |
| PAK | Pakistan | South Asia | C | current_season_percentile | 31 | 22.8 | −8.20 |
| SUR | Suriname | South America | C | current_season_percentile | 62.9 | 55 | −7.88 |
| ARG | Argentina | South America | C | current_season_percentile | 21 | 13.4 | −7.67 |
| USA | United States Of America | North & Central America | C | current_season_percentile | 52.4 | 58.5 | +6.07 |
| BGD | Bangladesh | South Asia | C | current_season_percentile | 75.1 | 81 | +5.86 |
| GRD | Grenada | Caribbean | C | current_season_percentile | 43 | 48.7 | +5.64 |
| VEN | Venezuela | South America | C | current_season_percentile | 26.3 | 21.7 | −4.70 |

### 8.2 Consolidated citation list

1. WHO Western Pacific, dengue situation update (China) — https://cdn.who.int/media/docs/default-source/wpro---documents/emergency/surveillance/dengue/dengue_20260820.pdf
2. China CDC Weekly, dengue seasonality 2005–2023 — https://weekly.chinacdc.cn/en/article/pdf/preview/10.46234/ccdcw2024.217
3. Santé publique France, French Guiana bulletin, 16 October 2026 — https://www.santepubliquefrance.fr/en/regions-and-territories/french-guiana/regional-bulletin/chikungunya-and-dengue-french-guiana-bulletin-dated-october-16-2026
4. Santé publique France, French Guiana bulletin, 21 August 2026 — https://www.santepubliquefrance.fr/en/regions-and-territories/french-guiana/regional-bulletin/chikungunya-and-dengue-french-guiana-bulletin-dated-august-21-2026
5. La Tribuna (Honduras), 13 October 2026 — https://www.latribuna.hn/2026/10/13/honduras-reporta-cinco-muertes-por-dengue-grave-en-2026-e-investiga-otro-fallecimiento/
6. La Tribuna (Honduras), 18 August 2026 — https://www.latribuna.hn/2026/08/18/honduras-reporta-9643-casos-de-dengue-13-de-sarampion-y-228-de-tosferina/
7. La Prensa (Honduras), dengue figures — https://www.laprensa.hn/honduras/dengue-cifras-salud-casos-estadisticas-prevencion-ME30075108
8. PAHO, Dengue Epidemiological Situation, Region of the Americas — https://www.paho.org/en/documents/situation-report-no-20-dengue-epidemiological-situation-region-americas-epidemiological
9. Statista, Jamaica dengue incidence — https://www.statista.com/statistics/1463264/dengue-cases-incidence-rate-jamaica
10. Excélsior (Mexico), 17 August 2026 — https://www.excelsior.com.mx/nacional/dengue-mexico-2026
11. Posta (Mexico, Edomex) — https://www.posta.com.mx/edomex/dengue-en-edomex-2026-bajan-contagios/vl2249684
12. TravelHealthPro, Mauritania outbreak update, 3 December 2025 — https://travelhealthpro.org.uk/updates.php?base=4999
13. The New Arab, dengue fever devastates Mauritania's capital — https://newarab.com/analysis/dengue-fever-devastates-mauritanias-capital
14. Canal N (Peru) — https://canaln.pe/actualidad/casos-dengue-aumentan-79-peru-minsa-advierte-que-podrian-incrementarse-altas-temperaturas-n495247
15. MINSA/DGE (Peru), Sala de Situación Dengue, week 33 2026 — https://www.dge.gob.pe/portal/docs/vigilancia/sala/2026/SE33/dengue.pdf
16. Sudan Tribune, 12 October 2026 — https://sudantribune.com/?p=319868
17. Sudan Tribune, 17 October 2026 — https://sudantribune.com/?p=320054
18. Florida Department of Health, Arbovirus Surveillance Report, Week 40 2026 — https://www.floridahealth.gov/wp-content/uploads/2026/10/fl-arbovirus-report-w40-2026.pdf
19. WGCU, dengue fever cases on the rise in Florida, 9 October 2026 — https://www.wgcu.org/health/2026-10-09/dengue-fever-cases-on-the-rise-in-florida
20. PAHO, calls for strengthened surveillance and preparedness amid increases in dengue and chikungunya in the Americas, 21 October 2026 — https://www.paho.org/en/news/21-10-2026-paho-calls-strengthened-surveillance-and-preparedness-amid-increases-dengue-and
21. PAHO, Epidemiological Update: Dengue and Chikungunya in the Americas Region, 20 October 2026 — https://www.paho.org/en/documents/epidemiological-update-dengue-and-chikungunya-americas-region-20-october-2026
22. mappr.co, Dengue Outbreak 2026: Cases by Country — https://www.mappr.co/dengue-outbreak-map/
23. PAHO, week 38 situation report — https://www.paho.org/sites/default/files/2026/10/2026-cde-dengue-sitrep-americas-epi-week-38-oct.pdf
24. ProPakistani, KP highest single-day dengue cases, 20 October 2026 — https://propakistani.pk/2026/10/20/kp-reports-highest-single-day-dengue-cases-of-2026/
25. Quotidiano Sanità, ECDC autochthonous cases in Europe 2026 — https://www.quotidianosanita.it/scienza-e-farmaci/dengue-ecdc-8-casi-autoctoni-in-europa-nel-2026-segnalazioni-in-francia-e-italia/
26. Free Press Journal, Nashik dengue cases — https://www.freepressjournal.in/pune/nashik-82-new-dengue-cases-reported-in-october-total-count-reaches-264
27. The Hans India, Delhi dengue cases — https://www.thehansindia.com/news/cities/new-delhi/delhi-98-dengue-cases-in-1st-week-of-oct-tally-touches-695-1129800
28. PNNL, environmental and epidemiological drivers of dengue forecasting — https://www.pnnl.gov/publications/environmental-and-epidemiological-drivers-dengue-forecasting-across-heterogeneous
29. Vacunas, predicting dengue in a changing climate (systematic review) — https://www.elsevier.es/es-revista-vacunas-72-articulo-predicting-dengue-in-changing-climate-S1576988726000233
30. MOH Singapore, discontinuation of Dengvaxia — https://www.moh.gov.sg/newsroom/discontinuation-of-dengvaxia-and-ongoing-monitoring-of-dengue-vaccines/
31. tnh1.com.br, Butantan-DV vaccine SUS inclusion — https://www.tnh1.com.br/noticia/nid/vacina-brasileira-contra-dengue-estara-no-sus-em-2026-diz-governo/
