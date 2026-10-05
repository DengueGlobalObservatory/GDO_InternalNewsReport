# GDO Internal News Report — 2026-10-05

*Source: Global Dengue Observatory (accessed 2026-10-05).*

## 1. Header

- **Report date:** 2026-10-05 (Monday routine run)
- **Active snapshot:** `snapshots/2026_10_05/` — **new pull this week**. Source data vintage (`target_render_date`): 2026-10-04. Source commit: `eed9c6d7` (DENV_global_observatory `Output/2026_10_04/`). Prior snapshot: `snapshots/2026_09_21/` (vintage 2026-09-18).
- **Pull status this week:** **pull week.** `target_render_date` advanced from 2026-09-18 to 2026-10-04 (this month's 4th, as expected), so Step 1's fetch/diff ran in full. No fallback was needed — `Output/2026_10_04/` existed exactly on the target date.
- **Countries covered:** 85.

## 2. This week's snapshot

Global picture across the 85 tracked countries/territories, from `latest_status.csv` only.

**Cumulative severity band** (percentile_cumulative, current position vs. seasonal-to-date expectation):

| Band | Countries |
|---|---|
| Normal | 29 |
| Low | 22 |
| High | 12 |
| Extremely High | 9 |
| Unknown | 7 |
| Extremely Low | 6 |

The 9 at **Extremely High** cumulative severity (essentially unchanged from last pull's list): Cook Islands, Cuba, Guyana, Kenya, Cambodia, Sri Lanka, Maldives, Sudan, and Timor-Leste.

**Current-season severity band** (current_season_percentile, i.e. how this season is tracking overall):

| Band | Countries |
|---|---|
| Low | 35 |
| Normal | 27 |
| Extremely Low | 9 |
| High | 5 |
| Unknown | 6 |
| Extremely High | 3 |

Current-season **Extremely High**: Cuba (100.0), Kenya (100.0), Cambodia (99.5) — the same three as last pull, all still running hot on both cumulative and current-season readings. Current-season **High**: Maldives (91.9), Sri Lanka (89.1), Sudan (83.9, up sharply from 61.2 — the second-largest Category C move this snapshot), United Republic of Tanzania (81.5), Bangladesh (75.1).

**Notable pattern — a large current-season jump that GDO's own classifier can't yet place.** Timor-Leste's current-season percentile has jumped from 16.5 to 85.2 (Category C, the largest single move this snapshot, +68.7), while its cumulative standing stays Extremely High (99.8, unchanged). Despite that defined 85.2 percentile, `current_season_severity` still reads **"Unknown"** with interpretation **"Cannot determine"** — copied verbatim here despite the apparent internal inconsistency, the same upstream data-pipeline quirk flagged for Côte d'Ivoire two pulls ago. Treat the 85.2 figure as directionally real (a steep current-season rise) but the formal band as not yet resolved.

**Caveat — data recency.** Of this week's ten targeted countries (Section 3), four (Bolivia, Honduras, Jamaica, Suriname) have a latest observed month of 2026-08-01 (~2.1 months stale — at/just beyond the upper edge of GDO's 1–2 month nowcast sweet spot; treat as lower-confidence). The other six (Mexico, Nepal, Peru, Brazil, Colombia, Grenada) sit at 2026-09-01 (~1.1 months stale, comfortably within the sweet spot). **Small-baseline/large-ratio instability:** Suriname's reported case count this period is a single case against a ~27-case seasonal baseline (ratio 0.04×) — too small a sample to read as a trend on its own, even though the severity-band crossing (Above average → Average) is a separate, independently meaningful reading. Grenada sits on a similarly small baseline (~46 cases expected; 27 observed) — its ratio flip (see Section 3) should be read the same way.

## 3. News — targeted (10 countries)

**Country selection note:** `movers.csv` flagged 7 Category A (severity-interpretation band changes) and 5 Category B (monthly-ratio-descriptor changes) rows this week, 10 unique countries once de-duplicated — exactly the cap, with no Category C-only mover needed. Bolivia and Nepal are double movers (both A and B), each moving consistently in one direction (Bolivia worsening on both counts, Nepal easing on both).

### Bolivia (Category A — severity interpretation: Average → Above average; Category B — monthly ratio: tracking near → running well above)
- GDO figures: 870 reported cases (latest observed month 2026-08-01, ~2.1 months stale — at the edge of the nowcast sweet spot). Cumulative percentile 86.4 (High). Current-season percentile 7.3 (Low), interpretation "Below average." Estimated total seasonal cases: 51,337. Monthly ratio: running well above (1.58×, vs a ~549-case baseline — a large enough baseline that this isn't small-sample noise). The only double-category (A+B) mover this week, and both point the same way: worsening.
- News: no October-dated figure confirmed. Most recent available data is from epidemiological week 33 (11 September 2026): 48,240 cumulative dengue cases nationally for 2026, with Bolivia reported as having the most intense outbreak among larger nations earlier in the season (389 cases per 100,000 at week 20, ahead of Brazil's 383). **Caveat:** that 48,240 figure is a national cumulative annual total, not comparable to GDO's 870-case August observed-month figure — a scope difference, not a contradiction, but worth flagging so the two numbers aren't conflated. Directionally consistent with GDO's "worsening" read. [Emergence of dengue at high altitude: Cochabamba 2024 outbreak](https://link.springer.com/article/10.1186/s12985-026-03117-1) · [Statista, Bolivia dengue incidence](https://www.statista.com/statistics/1462638/dengue-cases-incidence-rate-bolivia/)

### Honduras (Category A — severity interpretation: Below average → Average)
- GDO figures: 2,202 reported cases (latest observed month 2026-08-01, ~2.1 months stale). Cumulative percentile 25.5 (Normal, just above the Low cut-off). Current-season percentile 17.9 (Low), interpretation "Below average." Estimated total seasonal cases: 14,092. Monthly ratio: running well below (0.35×, vs a ~6,207-case baseline) — unchanged this pull; only the severity-interpretation band crossed.
- News: **fresh and directionally consistent.** As of early October 2026, Honduras has 10,059 accumulated dengue cases for the year, up from 9,409 on 1 October (~6.9% rise over the preceding two weeks). Four deaths recorded in 2026 to date (a 50% reduction on 2025's eight). Tegucigalpa and San Pedro Sula lead, with Cortés and Francisco Morazán departments concentrating the majority of cases; health authorities link the rise to recent rains favouring *Aedes aegypti* breeding, with children under 15 the most affected group. A mild national uptick matches GDO's own "Below average → Average" crossing (a move toward typical, not a dramatic escalation). [El Heraldo, dengue supera los 10 mil casos](https://www.elheraldo.hn/portada/dengue-supera-10-mil-casos-salud-pide-reforzar-prevencion-ante-lluvias-CD32201120) · [La Prensa, dengue en Honduras 2026](https://www.laprensa.hn/honduras/dengue-honduras-2026-cortes-francisco-morazan-concentran-mas-casos-HG31042995)

### Jamaica (Category A — severity interpretation: Below average → Average)
- GDO figures: 38 reported cases (latest observed month 2026-08-01, ~2.1 months stale). Cumulative percentile 25.9 (Normal, just above the Low cut-off). Current-season percentile 16.0 (Low), interpretation "Below average." Estimated total seasonal cases: 344. Monthly ratio: running well below (0.43×, vs an ~88-case baseline).
- News: **no October 2026-dated figure confirmed — a genuine news gap, flagged rather than guessed at.** The freshest material found is from October 2025 (379 cases to 11 October 2025, well down on 2024's 1,819 for the same period), describing the 2025/2026 season as "delayed in onset, or a low activity season," with authorities expecting an *Aedes aegypti* population increase into November. Jamaica's dengue season typically runs September–January, peaking around epidemiological weeks 41–43 (roughly mid-to-late October) — so this pull's mild uptick sits right at the start of the historically riskiest window; worth watching rather than reading as settled. [Jamaica Observer, dengue numbers low, but…](https://www.jamaicaobserver.com/2025/10/15/dengue-numbers-low/) · [JIS, health ministry reports significant reduction in dengue cases for 2025](https://jis.gov.jm/health-ministry-reports-significant-reduction-in-dengue-cases-for-2025/)

### Mexico (Category A — severity interpretation: Average → Below average)
- GDO figures: 2,450 reported cases (latest observed month 2026-09-01, ~1.1 months stale, well within the sweet spot). Cumulative percentile 24.2 (Low). Current-season percentile 9.7 (Low), interpretation "Below average." Estimated total seasonal cases: 77,856. Monthly ratio: running well below (0.08×, vs a ~31,471-case baseline) — a very low ratio on a large, stable baseline, so this is a real signal, not noise.
- News: no September/October 2026-specific count was confirmed within the search window — a genuine gap. The most recent dated figures found are from epidemiological week 21 (ending 30 May 2026): 2,286 cases and 4 deaths nationally, below the equivalent 2025 week (3,692 cases, 18 deaths). DENV-3 is the dominant circulating serotype (~93% of specimens serotyped), and the July–October rainy season is historically when the largest surges occur, with one 2026 forward projection putting the full-year total at 52,149–54,501 cases. GDO's own easing read (Average → Below average, well-below ratio) is broadly consistent with the lower year-on-year spring figures, but neither source has a live September/October number to confirm the picture holds through the rainy-season peak. [Epidemiological characteristics of dengue in Mexico, 2014–2025](https://doi.org/10.3390/pathogens15020190) · [BEACON, confirmed dengue cases Mexico EW21](https://beaconbio.org/en/report/?reportid=3e661d06-e8a8-4847-8877-2e481ead62e4&eventid=24a3e49c-1a3e-4ee3-bfdc-b2b0b756ccac)

### Nepal (Category A — severity interpretation: Above average → Average; Category B — monthly ratio: tracking near → running well below)
- GDO figures: 1,908 reported cases (latest observed month 2026-09-01, ~1.1 months stale). Cumulative percentile 69.5 (Normal). Current-season percentile 60.5 (Normal), interpretation "Average." Estimated total seasonal cases: 10,999. Monthly ratio: running well below (0.47×, vs a ~4,073-case baseline). The second double-category (A+B) mover this week, both pointing toward easing.
- News: no October 2026-dated figure confirmed. The most recent available data is from 20 August 2026: Gandaki Province led with 1,010 cumulative cases, followed by Koshi (674), Lumbini (435) and Bagmati (427), with two confirmed dengue deaths for the year at that point. The national Epidemiology and Disease Control Division ran a three-month awareness campaign from mid-July to mid-October. **Caveat — this is the one target country where the seasonal calendar argues against GDO's easing read:** Nepal's dengue season characteristically follows the June–September monsoon and peaks in the post-monsoon period, i.e. October — so GDO's September-month "easing" reading arrives just before the historical peak window, not after it. Worth flagging to the researcher as "watch, don't close the story" rather than a confirmed downturn. [Xinhua, dengue cases spread across Nepal](https://english.news.cn/20260820/ca290954e03b473f963c089a2cf8a04b/c.html) · [Gavi, climate change threatens Nepal with spike in dengue](https://www.gavi.org/vaccineswork/climate-change-threatens-mountainous-nepal-spike-dengue-infections)

### Peru (Category A — severity interpretation: Average → Above average)
- GDO figures: 3,058 reported cases (latest observed month 2026-09-01, ~1.1 months stale). Cumulative percentile 81.2 (High). Current-season percentile 19.9 (Low), interpretation "Below average." Estimated total seasonal cases: 97,525. Monthly ratio: running well above (1.70×, vs a ~1,798-case baseline) — this ratio reading itself did **not** change category this pull (Peru is Category A only); it was already running well above last pull too.
- News: no September/October 2026-specific figure confirmed — a genuine gap. The most recent dated item found is a health-emergency declaration following more than 39,000 national cases reported through December 2025. Peru's dengue transmission is seasonally more intense between November and May, meaning October typically sits in the lower-transmission part of the year — so GDO's "running well above seasonal baseline" reading is a relative-to-expectation signal for an already-quiet month, not evidence of an active large-scale outbreak right now. [Outbreak News Today, Peru dengue epidemiological alert](https://outbreaknewstoday.substack.com/p/peru-dengue-epidemiological-alert) · [CIDRAP, Peru declares dengue health emergency](https://www.cidrap.umn.edu/dengue/peru-declares-dengue-health-emergency)

### Suriname (Category A — severity interpretation: Above average → Average)
- GDO figures: 1 reported case (latest observed month 2026-08-01, ~2.1 months stale). Cumulative percentile 68.5 (Normal). Current-season percentile 62.9 (Normal), interpretation "Average." Estimated total seasonal cases: 384. **Caveat:** this pull's case count (1) against a ~27-case baseline (ratio 0.04×) is a very small sample — treat it as noisy in isolation; the severity-band easing is a separate, independently meaningful reading from `latest_status.csv`, not derived from the single-case figure.
- News: no October-dated figure confirmed. The most recent available figure is from epidemiological week 33 (11 September 2026): 416 cumulative dengue cases reported in Suriname for 2026. Notably, Suriname is also managing a concurrent chikungunya outbreak (flagged as of 17 February 2026) — worth noting as a wider vector-borne-disease pressure on the country's health system, even though it is a separate pathogen from dengue. [CDC, travel health notices](https://wwwnc.cdc.gov/travel/notices) · [Statista, Suriname dengue cases 2014–2024](https://www.statista.com/statistics/1617156/reported-dengue-fever-infection-cases-suriname/)

### Brazil (Category B — monthly ratio: running well above → running well below)
- GDO figures: 23,818 reported cases (latest observed month 2026-09-01, ~1.1 months stale) — the largest raw case count of this week's ten. Cumulative severity "Unknown" (percentile not computed this pull). Current-season severity **Extremely Low** (percentile ~0.0, interpretation "Rare good event — unusually low cases to date"). Estimated total seasonal cases: 1,734,501. Monthly ratio: running well below (0.61×, vs a ~39,178-case baseline) — a sharp reversal from "running well above" last pull.
- News: **fresh and strongly corroborated — Brazil's clearest story this week.** From January to 11 April 2026, Brazil registered 227,500 probable dengue cases nationally, a 75% reduction on the 916,400 recorded over the same period in 2025 — itself already down from the 2024 peak of 6.6 million to roughly 1.7 million for the year. Control measures credited include ovitraps now deployed in 1,600 municipalities (forecast to reach 2,000 by year end), sterile-insect and Wolbachia-method expansion across 72 priority municipalities, and the April 2026 rollout of Butantan-DV, the world's first single-dose dengue vaccine. GDO's own sharp reversal to "running well below" this pull lines up cleanly with the sustained national decline described in every source found. [Brazil: Bahia state reports 41% drop in dengue in 2026](https://outbreaknewstoday.substack.com/p/brazil-bahia-state-reports-41-drop) · [Brazil makes progress in controlling dengue and malaria](https://outbreaknewstoday.substack.com/p/brazil-makes-progress-in-controlling) · [Epidemiology of dengue in Brazil: recent trends](https://link.springer.com/article/10.1186/s12982-025-00937-4)

### Colombia (Category B — monthly ratio: running slightly above → running well below)
- GDO figures: 2,114 reported cases (latest observed month 2026-09-01, ~1.1 months stale). Cumulative percentile 57.9 (Normal). Current-season percentile 40.5 (Normal), interpretation "Average." Estimated total seasonal cases: 105,492. Monthly ratio: running well below (0.30×, vs a ~7,135-case baseline).
- News: **a genuinely mixed picture — flag both readings, don't pick a side.** As of early October 2026, Colombia's National Health Institute (INS) had accumulated 56,797 dengue cases for 2026 and formally classified the situation as an outbreak, with 14 territories reporting above-expected case levels; Meta department alone recorded 12,198 cases (the national high) with 7 confirmed deaths and 6 more under investigation. Eight departments together (Meta, Cesar, Bolívar, Santander, Norte de Santander, Magdalena, La Guajira, Cartagena de Indias) account for 60.7% of national notifications. **Caveat:** GDO's monthly ratio compares September's observed cases against Colombia's own seasonally-expected baseline for that calendar month, not against a cumulative year-to-date outbreak threshold — so "running well below seasonal baseline" (GDO) and "national outbreak across 14 territories" (INS) are measuring different things and are not strictly contradictory, but presenting them side by side without this context would read as one. [consultorsalud, dengue Colombia semana 26 2026](https://consultorsalud.com/dengue-colombia-semana-26-2026-ins/) · [Cronista, alerta por dengue en Colombia](https://www.cronista.com/colombia/actualidad-co/alerta-por-dengue-en-colombia-reportan-siete-muertes-y-advierten-por-el-aumento-de-casos-en-meta/)

### Grenada (Category B — monthly ratio: running well above → running well below)
- GDO figures: 27 reported cases (latest observed month 2026-09-01, ~1.1 months stale). Cumulative percentile 56.2 (Normal). Current-season percentile 43.0 (Normal), interpretation "Average." Estimated total seasonal cases: 271. **Caveat:** small baseline (~46 cases expected) — a handful of cases either way can swing the ratio; treat the flip as directionally indicative on a small country, not a large-scale signal.
- News: no fresher item found than the one already covered two pulls ago (21 September report): the Ministry of Health's "urges vigilance" notice after cases rose from 6 (epi week 32) to 23 (epi week 33, 16–22 August). That earlier spike is what drove last pull's "running well above" reading; this pull's reversal to "running well below" has no independent September/October confirmation yet — a genuine gap, not evidence either way. [NOW Grenada, Ministry of Health urges vigilance](https://nowgrenada.com/2026/08/ministry-of-health-urges-vigilance-amid-increase-in-dengue-cases/)

## 4. News — general scan (5 items)

Independent broad scan, capped at 5; includes GDO-tracked countries with dramatic recent news outside this week's 10-country target list, and non-endemic/no-GDO-data settings per the routine's instruction.

1. **Florida, United States, as of 2026-10-02/03** — Florida's dengue outbreak is now the largest in the continental US in decades: 252 locally-acquired cases this year, with Hillsborough County alone accounting for 223 and Polk becoming the seventh county to report local transmission. Local emergency declarations have followed. GDO tracks the US as a Category C mover this pull (current-season percentile 30.7 → 52.4) but it wasn't among this week's 10 targeted countries — this is the sharpest, freshest US-specific figure found. [Washington Post, Florida's dengue outbreak is now the largest in the continental US in decades](https://www.washingtonpost.com/health/2026/10/02/dengue-virus-outbreak-florida/85f604c8-be9b-11f1-81fc-9b76f8343b6c_story.html) · [WFLA, Florida's dengue outbreak reportedly largest US has seen in decades](https://www.wfla.com/news/florida/floridas-dengue-outbreak-reportedly-largest-us-has-seen-in-decades/)
2. **Cuba, as of 2026-09-23, with October flagged as the likely seasonal peak** — Cuba's 2026 dengue cases run 7.4 times above the level expected for this point in the year, with the usual October peak apparently still ahead; all four serotypes (DENV-1 through 4) are co-circulating, raising the risk of severe/haemorrhagic disease, amid reported shortages of fumigants and drinking water. Notably, this press report cites "the Global Dengue Observatory" directly as its source for the 7.4× figure — GDO is already Cuba's current-season Extremely High and cumulative Extremely High in this week's own data (Section 2), so the independent coverage and GDO's own read are fully aligned here. [CiberCuba, dengue en Cuba supera 7.4 veces el nivel esperado en 2026](https://en.cibercuba.com/noticias/2026-09-23-u1-e208933-s27061-nid340943-dengue-cuba-supera-74-veces-nivel-esperado-2026-pico)
3. **Cambodia, through 2026-09-11** — Cambodia has recorded over 60,000 dengue cases for 2026, with an earlier early-August count of 54,697 cases and 72 deaths representing an 81.1% increase on the same period in 2025; the incidence rate has exceeded the epidemic threshold and been accelerating since epidemiological week 24, with heavy rains and flooding prompting intensified vector-control measures. Cambodia sits at Extremely High on both GDO's cumulative (99.9) and current-season (99.5) bands this pull (Section 2) — the news and GDO's own classification point the same direction. [Dengue Visual Atlas, increase in dengue cases in Cambodia](https://denguevisualatlas.com/en/increase-in-dengue-cases-in-cambodia/) · [WHO WPRO, Dengue Situation Update 748, 25 Jun 2026](https://cdn.who.int/media/docs/default-source/wpro---documents/emergency/surveillance/dengue/dengue_20260625.pdf)
4. **Bangladesh, as of 2026-10-01** — Bangladesh enters October warning its dengue outbreak could worsen further after its deadliest month of the year in September, with forecasting models and recent rainfall/weather patterns pointing to continued transmission through the month. GDO-tracked (current-season High, 75.1) but not among this week's 10 targeted countries. [BusinessWorld, Bangladesh warns dengue outbreak could worsen after deadly September](https://bworldonline.com/world/2026/10/01/783566/bangladesh-warns-dengue-outbreak-could-worsen-after-deadly-september/)
5. **Europe, seasonal/structural item — non-endemic, no GDO data** — Imported (travel-associated) dengue case numbers in the EU/EEA are notably higher from June through October than the rest of the year, driven by international travel to endemic regions rather than local transmission; in Italy, Thailand, Cuba, India and the Maldives together accounted for 43.0% of imported DENV infections diagnosed. With October a peak month for both Southeast Asian and Caribbean source-country transmission (see Cambodia and Cuba above), European public-health bodies are flagged as remaining vigilant for imported cases through the autumn. [ECDC, travel-associated cases of dengue in the EU/EEA](https://www.ecdc.europa.eu/en/dengue/surveillance/dengue-virus-infections-travellers) · [Molecular epidemiology of imported dengue in travellers returning to Spain, 2022–2024](https://www.sciencedirect.com/science/article/pii/S1477893926000360)

## 5. Trend since last update

10 unique mover countries flagged this week (7 Category A rows, 5 Category B rows; Bolivia and Nepal appear in both — see Section 3's selection note and the full table in Section 8.1).

**Category A — severity-band interpretation changes (7), worsening first, then easing:**
- Bolivia: Average → Above average (worsening, now High cumulative)
- Honduras: Below average → Average (mild worsening, toward typical)
- Jamaica: Below average → Average (mild worsening, toward typical)
- Peru: Average → Above average (worsening, now High cumulative)
- Nepal: Above average → Average (easing)
- Suriname: Above average → Average (easing)
- Mexico: Average → Below average (easing)

**Category B — monthly-ratio descriptor changes (5):**
- Bolivia: tracking near → running well above (worsening)
- Nepal: tracking near → running well below (easing)
- Brazil: running well above → running well below (easing — sharp reversal, Brazil's largest-magnitude mover this pull)
- Colombia: running slightly above → running well below (easing)
- Grenada: running well above → running well below (easing — reversal of last pull's spike)

**Category C — current-season percentile shifts (10, largest first):**

| Country | Prior | Current | Δ |
|---|---|---|---|
| Timor-Leste | 16.5 | 85.2 | +68.7 |
| Samoa | 6.3 | 60.6 | +54.3 |
| New Caledonia | 15.7 | 69.3 | +53.6 |
| Mauritania | 35.7 | 72.4 | +36.8 |
| Sudan | 61.2 | 83.9 | +22.7 |
| United States | 30.7 | 52.4 | +21.6 |
| Peru | 0.0 | 19.9 | +19.9 |
| Viet Nam | 32.6 | 49.5 | +16.8 |
| China | 39.0 | 53.6 | +14.6 |
| Panama | 53.8 | 68.2 | +14.4 |

Unlike recent pulls, every one of this week's 10 Category C movers is a **rise** — no country's current-season percentile fell this snapshot.

## 6. Social-media candidate flags

Ranked short-list, for the researcher drafting Tuesday's posts.

1. **Brazil — the biggest absolute story, and cleanly corroborated.** A sharp reversal from "running well above" to "running well below" seasonal baseline, backed by a 75% year-on-year case reduction (Jan–Apr 2026) and a multi-year decline from 2024's 6.6 million peak. Brazil's raw case count (23,818) and predicted seasonal total (1.7 million) dwarf every other country in this week's selection. *Caveat: the national decline is well documented through April; no fresher September/October figure was found, so treat the "still declining" framing as extrapolated from GDO's own September-month read rather than independently reconfirmed for autumn.*
2. **Cuba — independent press is already citing GDO's own numbers.** A 7.4× above-expected reading, all four serotypes co-circulating, and the usual October peak still ahead — with CiberCuba's coverage naming "the Global Dengue Observatory" as its source. A rare case this pull of GDO's own output appearing directly in secondary reporting. *No major caveat — GDO's read and the press account line up because they're drawing on the same data.*
3. **Colombia — a "read the ratio carefully" explainer opportunity.** GDO's own monthly ratio eased to "running well below" seasonal baseline even as Colombia's National Health Institute formally classifies 2026 as a national outbreak across 14 territories, with Meta department alone past 12,000 cases and several deaths under investigation. Good material for a post about why a seasonal-baseline ratio and a year-to-date outbreak declaration can both be true at once. *Caveat: frame as methodology, not a correction of either figure — see Section 3 for the full reconciliation.*
4. **Bolivia — this week's only country worsening on every GDO signal.** The sole double-category (A+B) mover, with both the severity-interpretation band and the monthly-ratio descriptor crossing upward in the same pull. *Caveat: no September/October-dated news confirms this independently yet; the most recent outside figure (48,240 cumulative cases, week 33) is a different kind of number (annual cumulative vs. GDO's August observed-month count) and shouldn't be quoted alongside GDO's 870 as if comparable.*
5. **Timor-Leste — the single largest number on the board, with an asterisk.** Current-season percentile jumped +68.7, the largest move of any country this pull, and it remains cumulative Extremely High (99.8th percentile) — but the severity classifier itself still reads "Unknown"/"Cannot determine" despite the defined percentile, a known data-pipeline quirk. *Caveat: a good "biggest mover" headline, but the researcher should note the band is formally unresolved before stating a confirmed severity level.*

## 7. Scientific literature findings

Lighter-effort pass; a handful of recent items across forecasting, climate, vaccine policy and surveillance methods.

- **Forecasting:** A narrative review of dengue early-warning systems finds Random Forest and LSTM models deliver the strongest short-term (up to 1-week) forecast performance, with rainfall, temperature and humidity the dominant predictors across recent studies — directly relevant to GDO's own nowcast approach. *PMC*, 2026. [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC12810927)
- **Climate drivers:** A spatiotemporal deep-learning framework built on Vietnamese data argues that most operational early-warning systems still rely on single-model, province-level forecasts that overlook lagged climate drivers and spatial spillover between provinces — a methodological gap worth flagging given Viet Nam's own current-season rise this pull (Section 5, +16.8). *Int J Biometeorol*, 2026. [DOI](https://link.springer.com/article/10.1007/s00484-026-03151-2)
- **Vaccine policy:** Brazil's pilot rollout of Butantan-DV (the world's first single-dose dengue vaccine, mentioned in Section 3) — over 500,000 doses administered to primary healthcare workers from February 2026 — was **halted in early June 2026** after two deaths and 42 serious adverse events (intense abdominal pain, persistent vomiting, bleeding) were reported among recipients. A significant caveat to the otherwise positive Brazil vaccine story. [The Lancet Microbe, Brazil develops and rolls out single-dose dengue vaccine](https://www.thelancet.com/journals/lanmic/article/PIIS2666-5247(26)00042-X/fulltext)
- **Regional policy:** PAHO member states approved a new ten-year regional strategy (1 October 2026) to strengthen surveillance, prevention, preparedness and integrated response to dengue and other arboviral diseases across the Americas — a direct institutional response to the region-wide pressure visible in this week's Bolivia, Honduras, Peru and Colombia items (Section 3). [PAHO/WHO, Health Ministers approve new regional strategy](https://paho.org/en/news/1-10-2026-health-ministers-approve-new-regional-strategy-prevent-and-control-dengue-and-other)
- **Vaccine access:** Qdenga (TAK-003) became available for GP ordering in Australia on 1 October 2026, after a four-year wait, following India's own first-ever dengue vaccine approval in July 2026 — two concrete, dated regulatory developments rather than modelling exercises. [AusDoc, dengue fever vaccine arrives in Australia](https://www.ausdoc.com.au/news/dengue-fever-vaccine-arrives-in-australia/)

## 8. Appendix

### 8.1 `movers.csv` (active snapshot, full table)

| iso3 | country | region | category | field | prior_value | current_value | delta |
|---|---|---|---|---|---|---|---|
| BOL | Bolivia | South America | A | severity_interpretation | Average - typical case load at this point | Above average - more cases than typical at this point | NA |
| HND | Honduras | North & Central America | A | severity_interpretation | Below average - fewer cases than typical at this point | Average - typical case load at this point | NA |
| JAM | Jamaica | Caribbean | A | severity_interpretation | Below average - fewer cases than typical at this point | Average - typical case load at this point | NA |
| MEX | Mexico | North & Central America | A | severity_interpretation | Average - typical case load at this point | Below average - fewer cases than typical at this point | NA |
| NPL | Nepal | South Asia | A | severity_interpretation | Above average - more cases than typical at this point | Average - typical case load at this point | NA |
| PER | Peru | South America | A | severity_interpretation | Average - typical case load at this point | Above average - more cases than typical at this point | NA |
| SUR | Suriname | South America | A | severity_interpretation | Above average - more cases than typical at this point | Average - typical case load at this point | NA |
| BOL | Bolivia | South America | B | monthly_ratio_descriptor | tracking near | running well above | NA |
| BRA | Brazil | South America | B | monthly_ratio_descriptor | running well above | running well below | NA |
| COL | Colombia | South America | B | monthly_ratio_descriptor | running slightly above | running well below | NA |
| GRD | Grenada | Caribbean | B | monthly_ratio_descriptor | running well above | running well below | NA |
| NPL | Nepal | South Asia | B | monthly_ratio_descriptor | tracking near | running well below | NA |
| TLS | Timor-Leste | East & Southeast Asia | C | current_season_percentile | 16.5 | 85.2 | +68.72 |
| WSM | Samoa | Pacific Islands | C | current_season_percentile | 6.3 | 60.6 | +54.25 |
| NCL | New Caledonia | Pacific Islands | C | current_season_percentile | 15.7 | 69.3 | +53.56 |
| MRT | Mauritania | Sub-Saharan Africa | C | current_season_percentile | 35.7 | 72.4 | +36.76 |
| SDN | Sudan | Europe, Middle East & North Africa | C | current_season_percentile | 61.2 | 83.9 | +22.70 |
| USA | United States Of America | North & Central America | C | current_season_percentile | 30.7 | 52.4 | +21.65 |
| PER | Peru | South America | C | current_season_percentile | 0.0 | 19.9 | +19.90 |
| VNM | Viet Nam | East & Southeast Asia | C | current_season_percentile | 32.6 | 49.5 | +16.84 |
| CHN | China | East & Southeast Asia | C | current_season_percentile | 39.0 | 53.6 | +14.63 |
| PAN | Panama | North & Central America | C | current_season_percentile | 53.8 | 68.2 | +14.38 |

### 8.2 Consolidated citation list

1. Springer, emergence of dengue at high altitude: characterization of the 2024 outbreak in Cochabamba, Bolivia — https://link.springer.com/article/10.1186/s12985-026-03117-1
2. Statista, dengue cases incidence rate Bolivia 2014–2025 — https://www.statista.com/statistics/1462638/dengue-cases-incidence-rate-bolivia/
3. El Heraldo, dengue supera los 10 mil casos en Honduras, mientras Salud llama a la prevención — https://www.elheraldo.hn/portada/dengue-supera-10-mil-casos-salud-pide-reforzar-prevencion-ante-lluvias-CD32201120
4. La Prensa, dengue Honduras 2026: Cortés y Francisco Morazán concentran más casos — https://www.laprensa.hn/honduras/dengue-honduras-2026-cortes-francisco-morazan-concentran-mas-casos-HG31042995
5. Jamaica Observer, dengue numbers low, but… (15 Oct 2025) — https://www.jamaicaobserver.com/2025/10/15/dengue-numbers-low/
6. JIS, health ministry reports significant reduction in dengue cases for 2025 — https://jis.gov.jm/health-ministry-reports-significant-reduction-in-dengue-cases-for-2025/
7. Pathogens (MDPI), epidemiological characteristics of dengue disease in Mexico (2014–2025) — https://doi.org/10.3390/pathogens15020190
8. BEACON, total confirmed dengue cases in Mexico in EW21 — https://beaconbio.org/en/report/?reportid=3e661d06-e8a8-4847-8877-2e481ead62e4&eventid=24a3e49c-1a3e-4ee3-bfdc-b2b0b756ccac
9. Xinhua, dengue cases spread across Nepal as it marks World Mosquito Day (20 Aug 2026) — https://english.news.cn/20260820/ca290954e03b473f963c089a2cf8a04b/c.html
10. Gavi, climate change threatens mountainous Nepal with a spike in dengue infections — https://www.gavi.org/vaccineswork/climate-change-threatens-mountainous-nepal-spike-dengue-infections
11. Outbreak News Today, Peru dengue epidemiological alert — https://outbreaknewstoday.substack.com/p/peru-dengue-epidemiological-alert
12. CIDRAP, Peru declares dengue health emergency — https://www.cidrap.umn.edu/dengue/peru-declares-dengue-health-emergency
13. CDC, travel health notices — https://wwwnc.cdc.gov/travel/notices
14. Statista, dengue cases reported in Suriname 2014–2024 — https://www.statista.com/statistics/1617156/reported-dengue-fever-infection-cases-suriname/
15. Outbreak News Today, Brazil: Bahia state reports 41% drop in dengue in 2026 — https://outbreaknewstoday.substack.com/p/brazil-bahia-state-reports-41-drop
16. Outbreak News Today, Brazil makes progress in controlling dengue and malaria — https://outbreaknewstoday.substack.com/p/brazil-makes-progress-in-controlling
17. Springer, epidemiology of dengue in Brazil: recent trends and public health response — https://link.springer.com/article/10.1186/s12982-025-00937-4
18. consultorsalud, dengue Colombia semana 26 2026: 14 territorios superan lo esperado — https://consultorsalud.com/dengue-colombia-semana-26-2026-ins/
19. Cronista, alerta por dengue en Colombia: reportan siete muertes y advierten por el aumento de casos en Meta — https://www.cronista.com/colombia/actualidad-co/alerta-por-dengue-en-colombia-reportan-siete-muertes-y-advierten-por-el-aumento-de-casos-en-meta/
20. NOW Grenada, Ministry of Health urges vigilance amid increase in dengue cases (Aug 2026) — https://nowgrenada.com/2026/08/ministry-of-health-urges-vigilance-amid-increase-in-dengue-cases/
21. Washington Post, Florida's dengue outbreak is now the largest in the continental US in decades (2 Oct 2026) — https://www.washingtonpost.com/health/2026/10/02/dengue-virus-outbreak-florida/85f604c8-be9b-11f1-81fc-9b76f8343b6c_story.html
22. WFLA, Florida's dengue outbreak reportedly largest US has seen in decades — https://www.wfla.com/news/florida/floridas-dengue-outbreak-reportedly-largest-us-has-seen-in-decades/
23. CiberCuba, dengue en Cuba supera 7.4 veces el nivel esperado en 2026, y el pico suele ocurrir en octubre (23 Sep 2026) — https://en.cibercuba.com/noticias/2026-09-23-u1-e208933-s27061-nid340943-dengue-cuba-supera-74-veces-nivel-esperado-2026-pico
24. Dengue Visual Atlas, increase in dengue cases in Cambodia — https://denguevisualatlas.com/en/increase-in-dengue-cases-in-cambodia/
25. WHO WPRO, Dengue Situation Update 748 (25 Jun 2026) — https://cdn.who.int/media/docs/default-source/wpro---documents/emergency/surveillance/dengue/dengue_20260625.pdf
26. BusinessWorld, Bangladesh warns dengue outbreak could worsen after deadly September (1 Oct 2026) — https://bworldonline.com/world/2026/10/01/783566/bangladesh-warns-dengue-outbreak-could-worsen-after-deadly-september/
27. ECDC, travel-associated cases of dengue in the EU/EEA — https://www.ecdc.europa.eu/en/dengue/surveillance/dengue-virus-infections-travellers
28. ScienceDirect, molecular epidemiology and surveillance of imported dengue in travellers returning to Spain, 2022–2024 — https://www.sciencedirect.com/science/article/pii/S1477893926000360
29. PMC, forecasting and early warning systems for dengue outbreaks: updated narrative review — https://pmc.ncbi.nlm.nih.gov/articles/PMC12810927
30. International Journal of Biometeorology, causal and spatiotemporal deep learning for dengue forecasting under climate variability: a framework from Vietnam — https://link.springer.com/article/10.1007/s00484-026-03151-2
31. The Lancet Microbe, Brazil develops and rolls out single-dose dengue vaccine — https://www.thelancet.com/journals/lanmic/article/PIIS2666-5247(26)00042-X/fulltext
32. PAHO/WHO, Health Ministers approve new regional strategy to prevent and control dengue and other arboviral diseases in the Americas (1 Oct 2026) — https://paho.org/en/news/1-10-2026-health-ministers-approve-new-regional-strategy-prevent-and-control-dengue-and-other
33. AusDoc, dengue fever vaccine arrives in Australia — https://www.ausdoc.com.au/news/dengue-fever-vaccine-arrives-in-australia/
