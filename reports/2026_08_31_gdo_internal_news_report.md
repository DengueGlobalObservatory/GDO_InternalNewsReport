# GDO Internal News Report — 2026-08-31

*Source: Global Dengue Observatory (accessed 2026-08-31).*

## 1. Header

- **Report date:** 2026-08-31 (Monday routine run)
- **Active snapshot:** `snapshots/2026_08_24/` — **unchanged since 2026-08-24** (no new pull this week). Source data vintage (`target_render_date`): 2026-08-18. Source commit: `8f5519d7` (DENV_global_observatory `Output/2026_08_18/`).
- **Pull status this week:** **news-only week.** `target_render_date` (2026-08-18) is unchanged from the most recent snapshot's manifest, so Step 1's fetch/diff was skipped and `snapshots/2026_08_24/` was reused as the active snapshot. The next genuine data-pull week is expected once the public site's 2026-09-04 render goes live.
- **Countries covered:** 84.

## 2. This week's snapshot

Global picture across the 84 tracked countries/territories, from `latest_status.csv` only. Figures are identical to last week's report, since no new pull has happened.

**Cumulative severity band** (percentile_cumulative, current position vs. seasonal-to-date expectation):

| Band | Countries |
|---|---|
| Normal | 30 |
| Low | 27 |
| High | 11 |
| Extremely High | 9 |
| Extremely Low | 4 |
| Unknown | 3 |

The 9 at **Extremely High** cumulative severity: Afghanistan, Cook Islands, Cuba, Guyana, Kenya, Sri Lanka, Maldives, Sudan and Timor-Leste — unchanged from last week.

**Current-season severity band** (current_season_percentile, i.e. how this season is tracking overall):

| Band | Countries |
|---|---|
| Low | 35 |
| Extremely Low | 22 |
| Normal | 17 |
| Unknown | 5 |
| Extremely High | 4 |
| High | 1 |

The same four countries remain at **current-season Extremely High**: Cuba (percentile 100), Kenya (99.7), Cook Islands (97.8) and Guyana (95.7) — unchanged.

**Caveat — data recency.** With no new pull this week, the underlying data has aged a further seven days. Seven of this week's ten targeted countries (Section 3) have a latest observed month of 2026-07-01 — now ~2.0 months stale, sitting right at the outer edge of GDO's 1–2 month nowcast sweet spot rather than comfortably inside it. Three — Barbados, Antigua and Barbuda, Guyana — sit at 2026-06-01, ~3.0 months stale and clearly beyond the sweet spot; treat their figures as lower-confidence reads. Antigua and Barbuda (7 reported cases) and Barbados (14 reported cases) also carry a small-baseline caveat — a handful of cases can swing their ratios and percentiles disproportionately.

## 3. News — targeted (10 countries)

**Country selection note:** no new `movers.csv` was generated this week (news-only week), so the routine reused the same 10 flagged countries from the active snapshot's existing `movers.csv` — 4 Category A (severity-interpretation band changes) and 7 Category B (monthly-ratio-descriptor changes), 10 unique once de-duplicated. News below is a fresh search over the last ~2 weeks (17–31 August), not a repeat of prior citations.

### Sri Lanka (Category A — cumulative severity Extremely High; Category C — current-season percentile 37.7 → 82.2)
- GDO figures: 29,973 reported cases in the latest observed month (2026-07-01, ~2.0 months stale). Cumulative percentile 97.1 (Extremely High); current-season percentile 82.2 (High). Estimated total seasonal cases: 153,381. Monthly ratio descriptor: running well above.
- News: the outbreak has continued to deepen through the month. The National Dengue Control Unit's Week 34 situational report (covering 17–23 August, released 31 August) keeps the country under active vigilance; by 24 August cumulative 2026 cases had passed 94,000 with 71 deaths, rising to roughly 94,700–95,000 cases and 72 deaths by 29 August. Western Province remains hardest hit, with Gampaha (~20,000 cases) and Colombo (~18,700 cases) the worst-affected districts; the country is closing in on 100,000 cases for the year and remains on track to be the largest outbreak since 2017. [Newswire, 24 Aug](https://www.newswire.lk/2026/08/24/dengue-cases-in-sri-lanka-top-94000-71-deaths-reported/) · [Lanka Newspapers, 29 Aug](https://www.lankanewspapers.com/2026/08/29/sri-lanka-s-dengue-crisis-deepens-as-cases-approach-95-000-and-deaths-hit-72) · [Lanka Newspapers, Week 34 report, 31 Aug](https://www.lankanewspapers.com/2026/08/31/dengue-cases-continue-to-demand-vigilance-across-sri-lanka-as-week-34-report-released) · [Daily Mirror live tracker](https://www.dailymirror.lk/breaking-news/Sri-Lanka-Dengue-Cases-2026-Live-Tracker-and-Latest-Updates/108-345917)

### Panama (Category A — severity interpretation: Average → Above average; Category B — monthly ratio: running well below → running slightly below; Category C — current-season percentile 28.8 → 35.3)
- GDO figures: 1,056 reported cases (2026-07-01, ~2.0 months stale). Cumulative percentile 80.8 (High). Estimated total seasonal cases: 16,120.
- News: a "numbers disagree" situation worth flagging. Panama's Ministry of Health, via Infobae (30 Aug), reported 6,616 cumulative 2026 cases across epidemiological weeks 31–32 (+475 in the latest week alone) — but this is 32.4% *down* on the same period in 2025 (9,791 cases), and Minsa separately claims a 48.8% year-on-year national reduction from strengthened vector control and surveillance. That national decline sits awkwardly against GDO's own read of Panama crossing into a worse severity band this fortnight — a genuine divergence, not a data error, and worth explaining rather than smoothing over. [Infobae, 30 Aug](https://www.infobae.com/panama/2026/08/30/panama-reporta-6616-casos-de-dengue-tras-sumar-475-en-una-semana/) · [Ministerio de Salud de Panamá](https://www.minsa.gob.pa/noticia/panama-reduce-en-488-los-casos-de-dengue-en-2026-tras-fortalecer-la-vigilancia)

### Peru (Category B — monthly ratio: running well below → running well above)
- GDO figures: 6,202 reported cases (2026-07-01, ~2.0 months stale). Estimated total seasonal cases: 49,003.
- News: a serious escalation. La República (28 Aug) reports Peru's 2026 dengue death toll has already surpassed the entire 2025 total, with cases up 53% year-on-year (roughly 46,700 cumulative through epidemiological week 33, ending 22 August, against 57 deaths). MINSA attributes the rise to El Niño-driven rainfall, flooding and heat; Piura leads the national count (~8,960 cases). A further MINSA update (30 Aug) flagged ~4,000 cases in Lima and issued a fresh advisory over the ongoing El Niño impact. [La República, 28 Aug](https://larepublica.pe/sociedad/2026/08/28/dengue-en-peru-muertes-ya-superan-todo-el-registro-de-2025-y-casos-aumentan-53-en-2026-1187284) · [Infobae, 28 Aug](https://www.infobae.com/peru/2026/08/28/peru-rompe-su-propio-record-de-muertes-por-dengue-en-ocho-meses-del-2026-ya-hay-mas-victimas-que-en-todo-el-2025/) · [La República, 30 Aug](https://larepublica.pe/sociedad/2026/08/30/dengue-en-peru-minsa-reporta-4000-contagios-en-lima-y-lanza-advertencia-por-impacto-del-fenomeno-de-el-nino-956100)

### Colombia (Category B — monthly ratio: running well below → running slightly below; Category C — current-season percentile 23.8 → 27.6)
- GDO figures: 6,885 reported cases (2026-07-01, ~2.0 months stale). Cumulative percentile 57.3 (Normal). Estimated total seasonal cases: 104,587.
- News: the Instituto Nacional de Salud (INS) reports cumulative 2026 cases have climbed past 70,000 (week ending 22 August) with 41 confirmed deaths (0.06% case-fatality rate); over half of all cases concentrate in 35 municipalities, with La Orinoquía region (led by Villavicencio, ~8,270 cases) the main epidemiological focus. Coverage also flags El Niño as a risk multiplier for the rest of the season. As with Panama, GDO's own monthly-ratio reading is easing even as the national cumulative picture keeps climbing — a cumulative-vs-monthly divergence worth explaining to readers rather than treating as contradictory. [El Tiempo, citing INS](https://www.eltiempo.com/colombia/otras-ciudades/el-fenomeno-del-nino-podria-intensificar-el-dengue-en-colombia-ya-hay-mas-de-50-000-casos-en-2026-segun-el-ins-3567093) · [Consultorsalud, citing INS](https://consultorsalud.com/dengue-colombia-semana-26-2026-ins/)

### India (Category B — monthly ratio: running slightly above → tracking near)
- GDO figures: 10,122 reported cases (2026-07-01, ~2.0 months stale). Cumulative percentile 60.9 (Normal); current-season percentile 6.9 (Low). Estimated total seasonal cases: 132,230.
- News: monsoon-season transmission continuing to build, consistent with GDO's "tracking near" seasonal-baseline read. Delhi has logged 1,379 dengue cases so far this monsoon with no reported fatalities; West Bengal's health department has flagged five districts (Kolkata, Howrah, North and South 24 Parganas, Murshidabad) as highest-risk, with national vector-borne disease data (NCVBDC) recording 8,264 cases and 7 deaths in West Bengal alone this year. Case counts typically peak August–October, so the season's high point is still likely ahead. [Business Standard](https://www.business-standard.com/india-news/delhi-logs-1-349-swine-flu-1-379-dengue-cases-this-monsoon-no-fatalities-126080700183_1.html) · [hi INDiA, West Bengal districts](https://hiindia.com/bengal-health-department-identifies-five-districts-as-most-dengue-prone/)

### Guyana (Category B — monthly ratio: running well above → running well below)
- GDO figures: 710 reported cases (2026-06-01, ~3.0 months stale — beyond the sweet spot). Cumulative percentile 98.8 and current-season percentile 95.7 both remain Extremely High even as the monthly trend has cooled. Estimated total seasonal cases: 83,305.
- News: no dengue-specific item confirmed within the last ~2 weeks. Background only: earlier-year reporting described rising cases in Region Six (East Berbice-Corentyne) linked to rainy-season mosquito breeding, and separate coverage of efforts to secure a Japanese-developed vaccine (cost and supply cited as barriers) — neither is dated within this window, so the news picture stays thin relative to GDO's still-extreme season-to-date standing.

### Brazil (Category B — monthly ratio: running well below → running slightly above)
- GDO figures: 68,345 reported cases (2026-07-01, ~2.0 months stale). Cumulative percentile 49.5 (Normal); current-season percentile effectively zero (Extremely Low) — a large gap between the monthly and seasonal reads. Estimated total seasonal cases: 1,657,363 (a very large projection off a huge baseline — treat as indicative, not precise).
- News: no dengue-specific item confirmed within the last ~2 weeks. Background context (undated within window): national reporting earlier in the year described a roughly 75% year-on-year drop in probable cases, credited to the Butantan single-dose vaccine rollout, Wolbachia releases and expanded surveillance — see Section 7 for a fresh vaccine-distribution development.

### Barbados (Category A — severity interpretation: Rare good event → Below average; Category C — current-season percentile 1.6 → 5.9)
- GDO figures: 14 reported cases (2026-06-01, ~3.0 months stale — beyond the sweet spot; small case count, treat the ratio as noise-sensitive). Both cumulative (21.1) and current-season (5.9) percentiles remain Low/Extremely Low despite the uptick. Estimated total seasonal cases: 176.
- News: no dengue-specific item confirmed within the last ~2 weeks.

### Paraguay (Category A — severity interpretation: Below average → Average)
- GDO figures: 256 reported cases (2026-07-01, ~2.0 months stale). Cumulative percentile 25.6 (Low); current-season percentile 1.1 (Extremely Low). Estimated total seasonal cases: 6,565.
- News: Paraguay's DGVS (health surveillance directorate) reported a stable, low-transmission picture as of epidemiological week 32 — around 293 cumulative cases nationally, with no district-level outbreaks flagged — consistent with GDO's own "Average"/Low read. 26 August was marked as International Dengue Day, used by DGVS for a prevention-awareness push. [DGVS](https://dgvs.mspbs.gov.py/dia-internacional-contra-el-dengue-un-dia-para-recordar-365-dias-para-prevenir/)

### Antigua and Barbuda (Category B — monthly ratio: running well below → running slightly below; Category C — current-season percentile 10.7 → 16.4)
- GDO figures: 7 reported cases (2026-06-01, ~3.0 months stale — beyond the sweet spot; a small case count makes this figure more sensitive to noise than most). Cumulative percentile 42.4 (Normal); current-season percentile 16.4 (Low). Estimated total seasonal cases: 74.
- News: no dengue-specific item confirmed within the last ~2 weeks.

## 4. News — general scan (3 items)

Independent broad scan; capped at 5, but only three distinct items — beyond the ten targeted countries above — could be confirmed within the ~2-week window.

1. **Bangladesh, 17–26 August 2026** — Bangladesh is a Category C mover in this snapshot but fell outside the top-10 A/B priority list. The outbreak has intensified through August: DGHS-reported hospitalisations reached roughly 16,070 for the month by 26 August (up from 9,206 in July), with the death toll and case count climbing through the month (over 20,000 cumulative cases by 10 August, rising further thereafter). Dhaka division remains the hotspot. [Xinhua, 26 Aug](https://english.news.cn/asiapacific/20260826/ccabd2b83b7344b99d3533340ce9f687/c.html) · [The Business Standard](https://www.tbsnews.net/bangladesh/730-new-dengue-cases-two-deaths-reported-24hrs-1515701)
2. **United States (Florida), continuing through August 2026** — Local transmission kept spreading geographically: 16 new locally-acquired cases were confirmed in a single week (9–15 August), taking the state total to 23 across four counties (Hillsborough 15, Miami-Dade 4, Pinellas 3, Palm Beach 1); Citrus County subsequently confirmed its first-ever local case, becoming the fifth affected county and the northernmost so far this year. Non-endemic, no GDO nowcast coverage. [Medical Daily, Hillsborough cluster](https://www.medicaldaily.com/florida-local-dengue-hillsborough-cluster-2026-477675) · [Medical Daily, Citrus County](https://www.medicaldaily.com/citrus-county-first-local-dengue-case-florida-2026-477688)
3. **Philippines, 2026 year-to-date** — Not a GDO-tracked country, but a notable counter-example this week: roughly 93,155 cumulative 2026 cases and 386 deaths, a 46% *decrease* in cases and steep drop in deaths (from 699) versus the same period in 2025 — a genuine good-news outlier worth flagging alongside this week's more severe stories. [Dengue Visual Atlas, Philippines](https://denguevisualatlas.com/en/dengue-in-the-philippines-2026/)

## 5. Trend since last update

No new data this week — `target_render_date` unchanged (2026-08-18), so no new `movers.csv` was generated. The mover set below is unchanged from last week's report (2026-08-24) and is shown here for reference only.

**Category A — severity-band interpretation changes (4, unchanged):**
- Sri Lanka: Above average → Rare bad event (Extremely High cumulative)
- Panama: Average → Above average (High)
- Paraguay: Below average → Average (Normal)
- Barbados: Rare good event → Below average (still Low)

**Category B — monthly-ratio descriptor changes (7, unchanged):**
- Peru: running well below → running well above
- Guyana: running well above → running well below
- Brazil: running well below → running slightly above
- Colombia: running well below → running slightly below
- Panama: running well below → running slightly below
- Antigua and Barbuda: running well below → running slightly below
- India: running slightly above → tracking near

**Category C — current-season percentile shifts (10, unchanged, largest first):**

| Country | Prior | Current | Δ |
|---|---|---|---|
| Sri Lanka | 37.7 | 82.2 | +44.5 |
| Panama | 28.8 | 35.3 | +6.5 |
| Antigua and Barbuda | 10.7 | 16.4 | +5.8 |
| Venezuela | 18.2 | 12.8 | −5.4 |
| Barbados | 1.6 | 5.9 | +4.3 |
| Colombia | 23.8 | 27.6 | +3.8 |
| USA | 12.9 | 15.4 | +2.5 |
| Grenada | 10.5 | 12.8 | +2.3 |
| Bangladesh | 51.3 | 48.6 | −2.7 |
| Thailand | 4.7 | 3.2 | −1.5 |

## 6. Social-media candidate flags

Ranked short-list, for the researcher drafting Tuesday's posts:

1. **Sri Lanka — outbreak keeps deepening, approaching 100,000 cases.** Cumulative 2026 cases have climbed past ~94,700 with 72 deaths by late August, and the country remains on track to be the largest outbreak since 2017; GDO's own current-season percentile jump (37.7 → 82.2) from last week's pull is well corroborated by the sustained rise in official figures since. *Caveat: GDO's underlying data point (2026-07-01) is now ~2.0 months old — at the edge of, not comfortably inside, the nowcast sweet spot.*
2. **Peru — death toll for 2026 already exceeds all of 2025.** A genuinely severe milestone: cases up 53% year-on-year and deaths surpassing the entire prior year's total, attributed to El Niño-driven weather. Strong, concrete, well-sourced story with a clear climate-driver hook. *Caveat: MINSA's national figures are not GDO's nowcast — don't conflate the two when drafting.*
3. **Panama and Colombia — a "the national trend and GDO's trend disagree" story, twice over.** Panama's own case count is down 32–49% year-on-year even as GDO's severity read moved it into a worse band; Colombia shows a similar split (INS cumulative cases still climbing past 70,000 while GDO's monthly ratio eases). Good opportunity for audience education on why a cumulative national count and GDO's monthly/seasonal nowcast trend can diverge. *Caveat: exact INS Colombia bulletin date range not fully confirmed — verify before quoting precise figures.*
4. **Bangladesh — sharp August intensification.** Hospitalisations nearly doubled month-on-month (9,206 in July to ~16,070 in August), a concrete and citable escalation, though Bangladesh sits outside this week's top-10 target list (a Category C mover only). *No major caveat — DGHS's own figures are used directly.*
5. **Florida's local-transmission footprint keeps growing.** A fifth county (Citrus) confirmed its first-ever local case, extending the northernmost reach of transmission this year, following a 16-case single week across Hillsborough, Miami-Dade, Pinellas and Palm Beach. Continues the "dengue's reach is expanding" theme flagged in recent weeks. *Caveat: still small absolute numbers — frame as an emerging-geography story, not an outbreak-scale one.*

## 7. Scientific literature findings

Lighter-effort pass; a handful of recent items across forecasting, climate drivers, and vaccine policy.

- **Forecasting/nowcasting:** LSTM-based dengue forecasting and outbreak detection across selected Brazilian cities, integrating human mobility data with climate variables (temperature and humidity as the strongest predictors) alongside historical case counts. *PMC*, 2026. [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC12657288/)
- **Forecasting/nowcasting:** Bayesian hybrid statistical and machine-learning models for a temporal/spatial dengue early-warning system in Bangladesh. *medRxiv preprint*, 2025/26. [medRxiv](https://www.medrxiv.org/content/10.1101/2025.09.14.25335716.full.pdf)
- **Forecasting/nowcasting:** Deep-learning and mobility-network model for forecasting dengue importation risk in Brazil. *npj Digital Public Health*, 2026. [Nature](https://www.nature.com/articles/s44482-026-00015-9)
- **Climate drivers:** Multiregion causal-analysis study disentangling climate's dual (both amplifying and suppressing) role in dengue transmission dynamics. *Science Advances*, 2026. [Science Advances](https://www.science.org/doi/10.1126/sciadv.adq1901)
- **Vaccine policy:** Sanofi's Dengvaxia — already discontinued for low demand — has its final doses expiring at the end of August 2026, effectively ending its availability entirely (it was already the only dengue vaccine authorised for the US market prior to withdrawal). *Healio / PharmaVoice*, 2026. [Healio](https://www.healio.com/news/infectious-disease/20250916/qa-the-us-is-losing-its-only-dengue-vaccine) · [PharmaVoice](https://www.pharmavoice.com/news/dengue-sanofi-takeda-vaccine-qdenga-dengvaxia/730611/)
- **Vaccine policy:** Brazil has agreed a manufacturing deal with WuXi Biologics to deliver roughly 30 million doses of the Butantan-DV single-dose dengue vaccine in the second half of 2026, building on the Institute's own production of over one million doses so far, for free distribution via the SUS public health system. *BioSpace*, 2026. [BioSpace](https://www.biospace.com/press-releases/wuxi-vaccines-drug-substance-facility-receives-brazil-anvisa-gmp-certification-for-dengue-vaccine-manufacturing)

## 8. Appendix

### 8.1 `movers.csv` (active snapshot — unchanged from last week; no new pull this week)

| iso3 | country | region | category | field | prior_value | current_value | delta |
|---|---|---|---|---|---|---|---|
| BRB | Barbados | Caribbean | A | severity_interpretation | Rare good event - unusually low cases to date | Below average - fewer cases than typical at this point | NA |
| LKA | Sri Lanka | South Asia | A | severity_interpretation | Above average - more cases than typical at this point | Rare bad event - unusually high cases to date | NA |
| PAN | Panama | North & Central America | A | severity_interpretation | Average - typical case load at this point | Above average - more cases than typical at this point | NA |
| PRY | Paraguay | South America | A | severity_interpretation | Below average - fewer cases than typical at this point | Average - typical case load at this point | NA |
| ATG | Antigua And Barbuda | Caribbean | B | monthly_ratio_descriptor | running well below | running slightly below | NA |
| BRA | Brazil | South America | B | monthly_ratio_descriptor | running well below | running slightly above | NA |
| COL | Colombia | South America | B | monthly_ratio_descriptor | running well below | running slightly below | NA |
| GUY | Guyana | South America | B | monthly_ratio_descriptor | running well above | running well below | NA |
| IND | India | South Asia | B | monthly_ratio_descriptor | running slightly above | tracking near | NA |
| PAN | Panama | North & Central America | B | monthly_ratio_descriptor | running well below | running slightly below | NA |
| PER | Peru | South America | B | monthly_ratio_descriptor | running well below | running well above | NA |
| LKA | Sri Lanka | South Asia | C | current_season_percentile | 37.7 | 82.2 | +44.48 |
| PAN | Panama | North & Central America | C | current_season_percentile | 28.8 | 35.3 | +6.49 |
| ATG | Antigua And Barbuda | Caribbean | C | current_season_percentile | 10.7 | 16.4 | +5.79 |
| VEN | Venezuela | South America | C | current_season_percentile | 18.2 | 12.8 | −5.45 |
| BRB | Barbados | Caribbean | C | current_season_percentile | 1.6 | 5.9 | +4.26 |
| COL | Colombia | South America | C | current_season_percentile | 23.8 | 27.6 | +3.80 |
| BGD | Bangladesh | South Asia | C | current_season_percentile | 51.3 | 48.6 | −2.69 |
| USA | United States Of America | North & Central America | C | current_season_percentile | 12.9 | 15.4 | +2.53 |
| GRD | Grenada | Caribbean | C | current_season_percentile | 10.5 | 12.8 | +2.34 |
| THA | Thailand | East & Southeast Asia | C | current_season_percentile | 4.7 | 3.2 | −1.54 |

### 8.2 Consolidated citation list

1. Newswire, Sri Lanka cases top 94,000 (24 Aug) — https://www.newswire.lk/2026/08/24/dengue-cases-in-sri-lanka-top-94000-71-deaths-reported/
2. Lanka Newspapers, cases approach 95,000, deaths hit 72 (29 Aug) — https://www.lankanewspapers.com/2026/08/29/sri-lanka-s-dengue-crisis-deepens-as-cases-approach-95-000-and-deaths-hit-72
3. Lanka Newspapers, Week 34 situational report (31 Aug) — https://www.lankanewspapers.com/2026/08/31/dengue-cases-continue-to-demand-vigilance-across-sri-lanka-as-week-34-report-released
4. Daily Mirror, Sri Lanka live case tracker — https://www.dailymirror.lk/breaking-news/Sri-Lanka-Dengue-Cases-2026-Live-Tracker-and-Latest-Updates/108-345917
5. Infobae, Panama 6,616 cumulative cases (30 Aug) — https://www.infobae.com/panama/2026/08/30/panama-reporta-6616-casos-de-dengue-tras-sumar-475-en-una-semana/
6. Ministerio de Salud de Panamá, 48.8% national reduction — https://www.minsa.gob.pa/noticia/panama-reduce-en-488-los-casos-de-dengue-en-2026-tras-fortalecer-la-vigilancia
7. La República, Peru deaths exceed 2025 total (28 Aug) — https://larepublica.pe/sociedad/2026/08/28/dengue-en-peru-muertes-ya-superan-todo-el-registro-de-2025-y-casos-aumentan-53-en-2026-1187284
8. Infobae, Peru death-toll record (28 Aug) — https://www.infobae.com/peru/2026/08/28/peru-rompe-su-propio-record-de-muertes-por-dengue-en-ocho-meses-del-2026-ya-hay-mas-victimas-que-en-todo-el-2025/
9. La República, Peru Lima cases + El Niño advisory (30 Aug) — https://larepublica.pe/sociedad/2026/08/30/dengue-en-peru-minsa-reporta-4000-contagios-en-lima-y-lanza-advertencia-por-impacto-del-fenomeno-de-el-nino-956100
10. El Tiempo, Colombia El Niño risk + INS case count — https://www.eltiempo.com/colombia/otras-ciudades/el-fenomeno-del-nino-podria-intensificar-el-dengue-en-colombia-ya-hay-mas-de-50-000-casos-en-2026-segun-el-ins-3567093
11. Consultorsalud, Colombia citing INS — https://consultorsalud.com/dengue-colombia-semana-26-2026-ins/
12. Business Standard, Delhi monsoon dengue cases — https://www.business-standard.com/india-news/delhi-logs-1-349-swine-flu-1-379-dengue-cases-this-monsoon-no-fatalities-126080700183_1.html
13. hi INDiA, West Bengal five high-risk districts — https://hiindia.com/bengal-health-department-identifies-five-districts-as-most-dengue-prone/
14. DGVS Paraguay, International Dengue Day / week 32 update — https://dgvs.mspbs.gov.py/dia-internacional-contra-el-dengue-un-dia-para-recordar-365-dias-para-prevenir/
15. Xinhua, Bangladesh August hospitalisations top 16,000 (26 Aug) — https://english.news.cn/asiapacific/20260826/ccabd2b83b7344b99d3533340ce9f687/c.html
16. The Business Standard, Bangladesh 24-hour case/death update — https://www.tbsnews.net/bangladesh/730-new-dengue-cases-two-deaths-reported-24hrs-1515701
17. Medical Daily, Florida Hillsborough cluster (16 cases in one week) — https://www.medicaldaily.com/florida-local-dengue-hillsborough-cluster-2026-477675
18. Medical Daily, Florida Citrus County first local case — https://www.medicaldaily.com/citrus-county-first-local-dengue-case-florida-2026-477688
19. Dengue Visual Atlas, Philippines 2026 — https://denguevisualatlas.com/en/dengue-in-the-philippines-2026/
20. PMC, LSTM dengue forecasting Brazil (2026) — https://pmc.ncbi.nlm.nih.gov/articles/PMC12657288/
21. medRxiv, Bayesian dengue forecasting Bangladesh — https://www.medrxiv.org/content/10.1101/2025.09.14.25335716.full.pdf
22. npj Digital Public Health, dengue importation-risk forecasting (2026) — https://www.nature.com/articles/s44482-026-00015-9
23. Science Advances, climate's dual role in dengue dynamics (2026) — https://www.science.org/doi/10.1126/sciadv.adq1901
24. Healio, Dengvaxia discontinuation Q&A — https://www.healio.com/news/infectious-disease/20250916/qa-the-us-is-losing-its-only-dengue-vaccine
25. PharmaVoice, Sanofi pulling Dengvaxia from US market — https://www.pharmavoice.com/news/dengue-sanofi-takeda-vaccine-qdenga-dengvaxia/730611/
26. BioSpace, WuXi Biologics/Butantan dengue vaccine manufacturing deal — https://www.biospace.com/press-releases/wuxi-vaccines-drug-substance-facility-receives-brazil-anvisa-gmp-certification-for-dengue-vaccine-manufacturing
