# GDO Internal News Report — 2026-09-07

*Source: Global Dengue Observatory (accessed 2026-09-07).*

## 1. Header

- **Report date:** 2026-09-07 (Monday routine run)
- **Active snapshot:** `snapshots/2026_09_07/` — **new pull this week**. Source data vintage (`target_render_date`): 2026-09-04. Source commit: `92c2f221` (DENV_global_observatory `Output/2026_09_04/`). Prior snapshot: `snapshots/2026_08_24/` (vintage 2026-08-18).
- **Pull status this week:** **pull week.** `target_render_date` advanced from 2026-08-18 to 2026-09-04, so Step 1's fetch/diff ran in full.
- **Countries covered:** 84.

## 2. This week's snapshot

Global picture across the 84 tracked countries/territories, from `latest_status.csv` only.

**Cumulative severity band** (percentile_cumulative, current position vs. seasonal-to-date expectation):

| Band | Countries |
|---|---|
| Normal | 35 |
| Low | 19 |
| High | 10 |
| Extremely High | 11 |
| Extremely Low | 4 |
| Unknown | 5 |

The 11 at **Extremely High** cumulative severity: Afghanistan, Cook Islands, Cuba, Guyana, Kenya, Sri Lanka, Maldives, Sudan, Timor-Leste, and — new to this band this week — **Cambodia** and **Wallis and Futuna**.

**Current-season severity band** (current_season_percentile, i.e. how this season is tracking overall):

| Band | Countries |
|---|---|
| Low | 35 |
| Extremely Low | 17 |
| Normal | 19 |
| Unknown | 5 |
| Extremely High | 4 |
| High | 4 |

Current-season **Extremely High**: Cuba (percentile 100.0), Kenya (99.9), Guyana (96.7), and — new to this band this week — **Cambodia** (95.6). Cook Islands, which held this position last week (97.8), has dropped sharply to 20.9 (see Category C in Section 5) even as its cumulative reading stays Extremely High — a season that ran hot early and has since gone quiet.

**Caveat — data recency.** Of this week's ten targeted countries (Section 3), two (Bolivia, Nepal) have a latest observed month of 2026-08-01 (~1.2 months stale, within GDO's 1–2 month nowcast sweet spot); seven (Burkina Faso, Cambodia, China, New Caledonia, Vanuatu, Wallis and Futuna, Samoa) sit at 2026-07-01 (~2.2 months stale, just beyond the sweet spot's upper end); Malaysia sits at 2026-06-01 (~3.2 months stale, clearly beyond it — treat its figures as lower-confidence). **Small-baseline/large-ratio instability:** Vanuatu (monthly ratio 15.9× off a ~7.6-case seasonal baseline) and Wallis and Futuna (9.2× off a ~6.7-case baseline) both have tiny expected-case baselines — their "running well above" monthly reads should be treated as noisy, not necessarily a sustained shift, even though the underlying severity-band and percentile moves (Category A/C) are independently corroborated by case counts.

## 3. News — targeted (10 countries)

**Country selection note:** `movers.csv` flagged 19 Category A (severity-interpretation band changes) and 11 Category B (monthly-ratio-descriptor changes) rows this week — 27 unique countries once de-duplicated (Bolivia, Vanuatu and Wallis and Futuna each appear in both A and B). This is well beyond the 10-country cap, so per the routine's prioritisation rule (A/B over C), all 10 below come from A/B; no Category C-only mover needed to be added. Within that pool of 27, the 10 selected below were chosen for the size/severity of the crossing (newly-Extremely-High entrants, largest percentile swings, sharpest ratio reversals) and for a spread across regions, rather than any single mechanical rule — a judgement call the routine's instructions leave open when more than 10 countries are flagged.

### Cambodia (Category A — severity interpretation: Above average → Rare bad event, now Extremely High cumulative *and* current-season; Category C — current-season percentile 72.7 → 95.6)
- GDO figures: 29,580 reported cases (latest observed month 2026-07-01, ~2.2 months stale). Cumulative percentile 99.3 (Extremely High); current-season percentile 95.6 (Extremely High) — newly entered this band this week. Estimated total seasonal cases: 108,342. Monthly ratio: running well above.
- News: no item confirmed within the last ~2 weeks. Background: as of 12 July 2026, Cambodia had recorded 28,074 cumulative 2026 cases and 38 deaths (case-fatality rate 0.1%), a 58.1% rise on the same period in 2025 and past the epidemic threshold since epi week 24; full-year 2025 totalled 63,016 cases (79 deaths) — itself a 232% rise on 2024. [Outbreak News Today, 12 Jul](https://outbreaknewstoday.substack.com/p/cambodia-reports-232-increase-in)

### Wallis and Futuna (Category A — severity interpretation: Below average → Rare bad event, now Extremely High cumulative; Category B — monthly ratio: running well below → running well above; Category C — largest single mover this week, current-season percentile 5.1 → 48.0)
- GDO figures: 61 reported cases (latest observed month 2026-07-01, ~2.2 months stale). Cumulative percentile 99.99999 (Extremely High) — newly entered this band. Current-season percentile 48.0 (Normal). Estimated total seasonal cases: 740. **Caveat:** small seasonal baseline (~6.7 cases/month expected) makes the 9.2× monthly ratio noisy — read the band crossing (a step from a tiny handful of cases) with that in mind, even though it is directionally consistent with the news below.
- News: no item confirmed within the last ~2 weeks. Background: as of 17 July 2026, Wallis and Futuna had recorded 47 confirmed/probable cases since the start of the year (27 in Futuna, 20 in Wallis); local transmission was first confirmed in Futuna on 22 April, and by mid-July the epidemic was reported to be slowing in Futuna even as it progressed in Wallis. [La 1ère, 17 Jul](https://la1ere.franceinfo.fr/wallisfutuna/dengue-l-epidemie-ralentit-a-futuna-mais-progresse-a-wallis-1711747.html)

### Vanuatu (Category A — severity interpretation: Average → Above average; Category B — monthly ratio: running well below → running well above)
- GDO figures: 120 reported cases (latest observed month 2026-07-01, ~2.2 months stale). Cumulative percentile 92.1 (High); current-season percentile 36.7 (Normal). Estimated total seasonal cases: 297. **Caveat:** small seasonal baseline (~7.6 cases/month expected) makes the 15.9× monthly ratio noisy on its own, though it is corroborated by an independently-confirmed, growing case count below.
- News: Vanuatu's Ministry of Health declared a dengue outbreak in South Efate, Shefa Province in late June 2026; case counts have grown steadily since — 29 confirmed cases as of 2 July, rising to 112 confirmed cases (since 14 June) as of 31 August 2026, with ongoing local transmission across South-West Efate. [U.S. Embassy Vanuatu, 26 Jun](https://vt.usembassy.gov/health-alert-the-vanuatu-ministry-of-health-declared-a-dengue-outbreak-in-south-efate-shefa-province-june-26-2026/) · [ReliefWeb, Vanuatu Dengue Situation Update 01](https://reliefweb.int/report/vanuatu/vanuatu-dengue-situation-update-01-18-may-2026)

### Samoa (Category A — severity interpretation: Average → Above average; Category C — current-season percentile 7.2 → 59.8, the largest current-season swing of any country this snapshot)
- GDO figures: 167 reported cases (latest observed month 2026-07-01, ~2.2 months stale). Cumulative percentile 87.8 (High); current-season percentile 59.8 (Normal). Estimated total seasonal cases: 15,279. Monthly ratio: running well below (0.17×) — a striking divergence from the sharp current-season percentile jump above; flag both figures to the researcher rather than picking one.
- News: Samoa's outbreak, running since early 2025, remained active as of 4 September 2026 per regional tracking, though a specific recent case count could not be confirmed within the ~2-week window. Background: 17,402 cumulative clinically-diagnosed cases (5,117 lab-confirmed) as of March 2026, 9 deaths, children under 15 accounting for 74% of cases; Samoa was one of six Pacific Island Countries and Territories with active outbreaks as of 11 June 2026 (alongside American Samoa, Kiribati, New Caledonia, Tonga and Tuvalu). [Outbreak News Today](https://outbreaknewstoday.substack.com/p/samoa-dengue-outbreak-continues-into) · [WHO Western Pacific](https://www.who.int/westernpacific/newsroom/feature-stories/item/samoa-mobilizes-dengue-outbreak-response-with-support-from-who-and-partners)

### Malaysia (Category B — monthly ratio: running slightly below → running well above)
- GDO figures: 8,756 reported cases (latest observed month 2026-06-01, ~3.2 months stale — beyond GDO's nowcast sweet spot; treat as lower-confidence). Cumulative percentile 59.9 (Low); current-season percentile 24.7 (Low). Estimated total seasonal cases: 80,971.
- News: Malaysia's Ministry of Health reported 58,079 cumulative 2026 cases as of 15 August — 56.2% higher than the same period in 2025 — with 55 deaths recorded through epidemiological week 32. Kuala Lumpur/Putrajaya cases rose 106% and Perlis 207% year-on-year; the ministry issued a nationwide risk warning on 21 August as clusters spread beyond the initial Selangor/KL/Putrajaya hotspot. DENV-3 is now the dominant circulating serotype nationally. [Free Malaysia Today, 21 Aug](https://www.freemalaysiatoday.com/category/nation/2026/08/21/health-ministry-warns-of-increased-nationwide-dengue-risk-as-cases-rise) · [Sowetan/wire, 21 Aug](https://www.sowetan.co.za/news/world/2026-08-21-dengue-fever-cases-up-56-in-klang-valley-health-ministry-warns/)

### New Caledonia (Category B — monthly ratio: running well below → running well above)
- GDO figures: 57 reported cases (latest observed month 2026-07-01, ~2.2 months stale). Cumulative percentile 70.2 (Low); current-season percentile 13.8 (Low). Estimated total seasonal cases: 2,313.
- News: no item confirmed within the last ~2 weeks; the two most recent sources found also disagree with each other on scale, so treat the figures as indicative only. New Caledonia logged the highest case count of any Pacific territory in the region for early 2026 (1,786 cases by 21 May), with an epidemic phase declared in late March and a DENV-1 red alert issued; a separate, undated report cites a lower "640+ cases since the start of 2026" figure, with transmission concentrated outside Greater Nouméa and Wolbachia-mosquito releases credited with suppressing urban spread. [ReliefWeb, 21 May](https://reliefweb.int/report/vanuatu/vanuatu-dengue-situation-update-01-18-may-2026) · [Islands Business, undated](https://islandsbusiness.com/news-break/new-caledonia-reports-spike-in-dengue-cases/)

### Burkina Faso (Category A — severity interpretation: Cannot determine → Above average)
- GDO figures: 4,138 reported cases (latest observed month 2026-07-01, ~2.2 months stale). Cumulative percentile 93.3 (High) — now defined, versus "Cannot determine" last pull; current-season percentile 44.4 (Normal). Estimated total seasonal cases: 170,427.
- News: no 2026 outbreak situation report could be confirmed. Available 2026 coverage is retrospective research on the 2023 Hauts-Bassins outbreak (impact of delayed medical consultation on severity/mortality, climatic outbreak-threshold analysis) rather than a live 2026 update. Worth flagging to the researcher: GDO's own reading just became classifiable (from "Cannot determine" to "Above average"), and no matching real-time news coverage could be found to corroborate or contextualise it — a gap, not a null result. [Frontiers, 2026](https://www.frontiersin.org/journals/tropical-diseases/articles/10.3389/fitd.2026.1754235/full) · [PMC, 2026](https://pmc.ncbi.nlm.nih.gov/articles/PMC13486771/)

### China (Category A — severity interpretation: Above average → Cannot determine; Category C — current-season percentile 21.8 → 39.0)
- GDO figures: 1,120 reported cases (latest observed month 2026-07-01, ~2.2 months stale). Cumulative severity is now **"Cannot determine"** (percentile unavailable this pull, versus a defined "Above average" reading last time) — a data-availability caveat about GDO's own pipeline, not an epidemiological claim about China. Current-season percentile 39.0 (Normal). Estimated total seasonal cases: 40,458.
- News: no item confirmed within the last ~2 weeks. Background: China recorded 841 cumulative dengue cases through mid-March 2026 (epi week 12), 59.6% higher than the same period in 2025, with monthly counts of 92–94 cases across January–March; a dengue/Zika virus co-infection imported from Kuala Lumpur, Malaysia was reported in Sichuan Province in January 2026. [WHO WPRO Dengue Situation Update](https://cdn.who.int/media/docs/default-source/wpro---documents/emergency/surveillance/dengue/dengue_20260416.pdf) · [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC13171624/)

### Bolivia (Category A — severity interpretation: Above average → Average; Category B — monthly ratio: running well above → running slightly below)
- GDO figures: 472 reported cases (latest observed month 2026-08-01, ~1.2 months stale — within GDO's sweet spot). Cumulative percentile 46.8 (Normal); current-season percentile 0.1 (Extremely Low) — among the lowest readings in the entire dataset this week. Estimated total seasonal cases: 27,994.
- News: Bolivia's Ministry of Health and Sports describes the country as in a phase of "favourable control and low transmission" for 2026 — a marked shift from 2025's accumulated incidence of 302.7 cases per 100,000 — with DEN-1 the predominant circulating serotype in January–February 2026 (versus DEN-1/DEN-2 co-circulation in 2025). This corroborates GDO's own easing reading well; a good, low-drama double-improvement story. [Atlas Visual del Dengue](https://denguevisualatlas.com/es/dengue-en-bolivia-situacion-actual-zonas-de-riesgo-y-guia-de-prevencion-2025-2026/) · [Pathogenos](https://pathogenos.com/dengue-in-latin-america-in-2026-the-latest-outbreak-updates/)

### Nepal (Category A — severity interpretation: Above average → Average)
- GDO figures: 1,776 reported cases (latest observed month 2026-08-01, ~1.2 months stale — within GDO's sweet spot). Cumulative percentile 74.6 (Normal, just below the High threshold); current-season percentile 50.8 (Normal). Estimated total seasonal cases: 13,444. Monthly ratio: tracking near baseline.
- News: dengue spread continued through Nepal's post-monsoon period. By 20 August 2026, Gandaki Province led with 1,010 cases, followed by Koshi (674), Lumbini (435) and Bagmati (427), with two confirmed dengue deaths for the year as of that date. Cases had reached 19,599 nationally earlier in the season, spread across most of the country's 77 districts. [Xinhua, 20 Aug](https://english.news.cn/20260820/ca290954e03b473f963c089a2cf8a04b/c.html) · [Rising Nepal Daily](https://risingnepaldaily.com/news/50432)

## 4. News — general scan (5 items)

Independent broad scan, capped at 5; includes GDO-tracked countries with dramatic recent news outside this week's 10-country target list, and non-endemic/no-GDO-data settings per the routine's instruction.

1. **Bangladesh, 2026-09 (ongoing)** — A sharp September surge is straining hospitals: 42,590 people hospitalised and 117 deaths for the year so far, with 1,558 hospitalisations in a single 24-hour period — the highest daily tally of the year. One epidemiologist's forecasting model suggests hospitalisations could exceed 30,000 during September alone if the trend holds. GDO-tracked but not among this week's 10 targeted countries; GDO's own latest observed month (2026-07-01, ~2.2 months stale) predates this surge entirely, so the nowcast has not yet caught up with what the news is reporting. [Dubai Eye, Sept 2026](https://www.dubaieye1038.com/news/international/bangladesh-dengue-outbreak-accelerates-as-hospitals-come-under-strain/)
2. **Cuba, 2026-09-02** — Cuba met CDC's criteria for "high transmission" status, with 10 or more cases reported among travellers in the last three months. Consistent with GDO's own reading: Cuba remains at Extremely High on both cumulative (99.99) and current-season (100.0) percentiles this week (Section 2), unchanged in position though now independently corroborated by traveller-surveillance data. [CDC, accessed via search, 2 Sep](https://www.cdc.gov/dengue/areas-with-risk/index.html)
3. **Americas region-wide, epi week 32 (through early Sept 2026)** — PAHO reported 1,567,004 suspected cases region-wide, a cumulative incidence of 150 per 100,000 — down 58% on the same period in 2025 and 65% below the five-year average. Useful counter-narrative to this week's individual country stories: the region as a whole is well below its recent-years baseline even as several GDO-tracked countries (Bolivia, this week's Section 3) show local improvement and others (Cambodia, outside the Americas) do not. [PAHO/WHO, Epi Week 32](https://www.paho.org/en/documents/dengue-epidemiological-situation-region-americas-epidemiological-week-32-2026)
4. **Italy, 2026 year-to-date (as of 30 Aug)** — Three confirmed locally-acquired (non-travel) dengue cases reported in the Puglia and Tuscany regions during 2026. Non-endemic, no GDO nowcast coverage. [NaTHNaC/travelhealthpro summary, accessed 30 Aug–2 Sep window](https://www.cidrap.umn.edu/chikungunya/european-nations-report-more-local-detections-chikungunya-dengue)
5. **United States, 2026 year-to-date** — Locally-acquired and travel-associated dengue cases nationally have surpassed 500 for 2026, with coverage noting *Aedes aegypti*'s range continuing to expand northward under warming conditions. Continues the "dengue's reach is expanding" theme flagged in prior weeks' reports (France/Florida local cases, 24 Aug report). Non-endemic in most of the affected geography, no GDO nowcast coverage. [Medical Daily, 2026](https://www.medicaldaily.com/dengue-fever-2026-us-cases-mosquito-expanding-north-476323)

## 5. Trend since last update

27 unique mover countries flagged this week (19 Category A rows, 11 Category B rows, 10 Category C rows; some countries appear in more than one category — see Section 3's selection note and the full table in Section 8.1).

**Category A — severity-band interpretation changes (19), newly-defined or worsening first:**
- Cambodia: Above average → **Rare bad event** (now Extremely High cumulative and current-season)
- Wallis and Futuna: Below average → **Rare bad event** (now Extremely High cumulative)
- Burkina Faso: Cannot determine → Above average (now High)
- Vanuatu: Average → Above average (now High)
- Samoa: Average → Above average (now High)
- China: Above average → **Cannot determine** (data-availability caveat, see Section 3)
- Bolivia: Above average → Average (improving)
- Nepal: Above average → Average (improving)
- Argentina: Below average → Average (improving)
- Jamaica: Average → Below average (improving)
- 9 further minor A crossings among small-baseline countries/territories (Cayman Islands, French Guiana, Marshall Islands, Micronesia, Reunion, Seychelles, Solomon Islands, Tonga, Tuvalu) — see Section 8.1 for the full table.

**Category B — monthly-ratio descriptor changes (11):**
- Malaysia: running slightly below → **running well above**
- New Caledonia: running well below → **running well above**
- Vanuatu: running well below → **running well above**
- Wallis and Futuna: running well below → **running well above**
- Bolivia: running well above → running slightly below (improving)
- Colombia, Antigua and Barbuda, Ethiopia, Fiji, Australia, USA: minor below-band shifts (well below → slightly below) — see Section 8.1.

**Category C — current-season percentile shifts (10, largest first):**

| Country | Prior | Current | Δ |
|---|---|---|---|
| Cook Islands | 97.8 | 20.9 | −76.9 |
| Samoa | 7.2 | 59.8 | +52.6 |
| Wallis and Futuna | 5.1 | 48.0 | +42.9 |
| Kiribati | 70.9 | 40.7 | −30.2 |
| Cambodia | 72.7 | 95.6 | +22.9 |
| Afghanistan | 31.8 | 51.0 | +19.2 |
| Bangladesh | 48.6 | 66.6 | +18.1 |
| China | 21.8 | 39.0 | +17.2 |
| Mauritania | 18.3 | 34.6 | +16.4 |
| Maldives | 73.2 | 89.5 | +16.3 |

## 6. Social-media candidate flags

Ranked short-list, for the researcher drafting Tuesday's posts:

1. **Cambodia — genuine, corroborated escalation into GDO's most severe band on both cumulative and current-season measures.** Current-season percentile jumped from 72.7 to 95.6, cumulative and current-season severity both crossed into Extremely High, and this lines up with independently-reported (if slightly dated, mid-July) figures showing a 58% year-on-year case rise past the epidemic threshold. Strongest, best-corroborated story this week. *Caveat: GDO's underlying data point is ~2.2 months old — just beyond the healthy end of the sweet spot; no news item within the last two weeks specifically, so frame as "ongoing/escalating" rather than breaking.*
2. **Vanuatu — small-island outbreak with a clean, dated case-count trajectory.** GDO's monthly ratio flipped from "well below" to "well above" and severity crossed into "Above average," matching an independently-tracked, growing outbreak (29 cases as of 2 July → 112 as of 31 August) in Shefa Province. Concrete numbers, clear trend, easy to caption responsibly. *Caveat: small seasonal baseline makes GDO's own ratio figure noisy in isolation — lean on the external case counts for the headline number, use GDO for the trend direction.*
3. **Malaysia — a large, high-profile country with a sharp, well-documented national surge.** Ministry of Health figures show cases up 56% year-on-year (58,079 by 15 August) with Kuala Lumpur/Putrajaya up 106% and a new dominant serotype (DENV-3); GDO's own monthly ratio swung to "running well above" too, though off a stale (~3.2-month) data point. Good "large, familiar country, credible numbers" story. *Caveat: GDO's figure predates the ministry's most recent, higher counts — don't quote GDO's raw case number (8,756) alongside the ministry's (58,079) without explaining they're different vintages.*
4. **Bolivia — a good-news story, worth telling occasionally.** Severity improved on both the cumulative and monthly-ratio measures, and Bolivia's own Ministry of Health independently frames 2026 as a "favourable control" year after a rough 2025. Rare, well-corroborated downturn — useful for balance against a week otherwise dominated by escalation stories. *No major caveat — data points align well.*
5. **Bangladesh — the most dramatic real-world number this week, but it's outside GDO's own targeted list.** A September surge (1,558 hospitalisations in a single day, forecasts of 30,000+ September hospitalisations) is well outside what GDO's nowcast — anchored to July data — currently reflects. Flag as a "watch this space" item: strong human-interest/urgency angle, but GDO's own figures can't yet corroborate the scale. *Caveat: do not attribute the September hospitalisation figures to GDO — they are Bangladesh government/press figures on a different data vintage entirely.*

## 7. Scientific literature findings

Lighter-effort pass; a handful of recent items across forecasting, climate drivers, surveillance and vaccine policy.

- **Nowcasting:** NowcastPNN, an attention-based probabilistic neural network architecture to estimate occurred-but-not-yet-reported dengue cases, demonstrated on São Paulo, Brazil surveillance data. *Epidemics*, March 2026. [ScienceDirect](https://www.sciencedirect.com/science/article/pii/S1755436525000684)
- **Forecasting:** A hybrid machine-learning/wavelet approach for weekly dengue case forecasting, aimed at earlier outbreak detection. *PMC*, accepted July 2026. [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC13349185/)
- **Forecasting:** Comparative evaluation of machine-learning strategies (including gradient-boosting and deep-learning approaches) for short-term dengue forecasting across Brazilian capital municipalities. *PMC*, accepted August 2026. [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC13476183/)
- **Climate drivers:** Deep-learning models linking climatic and temporal dynamics to dengue transmission in Bangladesh — topical given this week's Bangladesh surge (Section 4); short-term (3–7 day) lags in surface pressure, precipitation and wind speed were the strongest predictors. *PMC*, 2026. [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC13362098/)
- **Vaccine policy:** India's drug regulator (CDSCO) approved Takeda's Qdenga dengue vaccine for ages 4–60, following a quality/safety/efficacy review — a significant new-market approval. July 2026. [Medical Xpress](https://medicalxpress.com/news/2026-07-india-dengue-vaccine.html)
- **Vaccine policy:** Sanofi is discontinuing US marketing of its dengue vaccine (Dengvaxia) in Q3 2026, citing low global demand — a contraction in available products even as India's market opens up (above). [BioPharma Dive](https://www.biopharmadive.com/news/dengue-sanofi-takeda-vaccine-qdenga-dengvaxia/730846/)

## 8. Appendix

### 8.1 `movers.csv` (active snapshot)

| iso3 | country | region | category | field | prior_value | current_value | delta |
|---|---|---|---|---|---|---|---|
| ARG | Argentina | South America | A | severity_interpretation | Below average - fewer cases than typical at this point | Average - typical case load at this point | NA |
| BFA | Burkina Faso | Sub-Saharan Africa | A | severity_interpretation | Cannot determine | Above average - more cases than typical at this point | NA |
| BOL | Bolivia | South America | A | severity_interpretation | Above average - more cases than typical at this point | Average - typical case load at this point | NA |
| CHN | China | East & Southeast Asia | A | severity_interpretation | Above average - more cases than typical at this point | Cannot determine | NA |
| CYM | Cayman Islands | Caribbean | A | severity_interpretation | Below average - fewer cases than typical at this point | Rare good event - unusually low cases to date | NA |
| FSM | Micronesia (Federated States Of) | Pacific Islands | A | severity_interpretation | Below average - fewer cases than typical at this point | Average - typical case load at this point | NA |
| GUF | French Guiana | South America | A | severity_interpretation | Below average - fewer cases than typical at this point | Rare good event - unusually low cases to date | NA |
| JAM | Jamaica | Caribbean | A | severity_interpretation | Average - typical case load at this point | Below average - fewer cases than typical at this point | NA |
| KHM | Cambodia | East & Southeast Asia | A | severity_interpretation | Above average - more cases than typical at this point | Rare bad event - unusually high cases to date | NA |
| MHL | Marshall Islands | Pacific Islands | A | severity_interpretation | Rare good event - unusually low cases to date | Cannot determine | NA |
| NPL | Nepal | South Asia | A | severity_interpretation | Above average - more cases than typical at this point | Average - typical case load at this point | NA |
| REU | Reunion | Sub-Saharan Africa | A | severity_interpretation | Below average - fewer cases than typical at this point | Average - typical case load at this point | NA |
| SLB | Solomon Islands | Pacific Islands | A | severity_interpretation | Below average - fewer cases than typical at this point | Average - typical case load at this point | NA |
| SYC | Seychelles | Sub-Saharan Africa | A | severity_interpretation | Rare good event - unusually low cases to date | Cannot determine | NA |
| TON | Tonga | Pacific Islands | A | severity_interpretation | Below average - fewer cases than typical at this point | Average - typical case load at this point | NA |
| TUV | Tuvalu | Pacific Islands | A | severity_interpretation | Below average - fewer cases than typical at this point | Average - typical case load at this point | NA |
| VUT | Vanuatu | Pacific Islands | A | severity_interpretation | Average - typical case load at this point | Above average - more cases than typical at this point | NA |
| WLF | Wallis And Futuna | Pacific Islands | A | severity_interpretation | Below average - fewer cases than typical at this point | Rare bad event - unusually high cases to date | NA |
| WSM | Samoa | Pacific Islands | A | severity_interpretation | Average - typical case load at this point | Above average - more cases than typical at this point | NA |
| ATG | Antigua And Barbuda | Caribbean | B | monthly_ratio_descriptor | running slightly below | running well below | NA |
| AUS | Australia | Pacific Islands | B | monthly_ratio_descriptor | running well below | running slightly below | NA |
| BOL | Bolivia | South America | B | monthly_ratio_descriptor | running well above | running slightly below | NA |
| COL | Colombia | South America | B | monthly_ratio_descriptor | running slightly below | running well below | NA |
| ETH | Ethiopia | Sub-Saharan Africa | B | monthly_ratio_descriptor | running well below | running slightly below | NA |
| FJI | Fiji | Pacific Islands | B | monthly_ratio_descriptor | running well below | running slightly below | NA |
| MYS | Malaysia | East & Southeast Asia | B | monthly_ratio_descriptor | running slightly below | running well above | NA |
| NCL | New Caledonia | Pacific Islands | B | monthly_ratio_descriptor | running well below | running well above | NA |
| USA | United States Of America | North & Central America | B | monthly_ratio_descriptor | running well below | running slightly below | NA |
| VUT | Vanuatu | Pacific Islands | B | monthly_ratio_descriptor | running well below | running well above | NA |
| WLF | Wallis And Futuna | Pacific Islands | B | monthly_ratio_descriptor | running well below | running well above | NA |
| COK | Cook Islands | Pacific Islands | C | current_season_percentile | 97.8 | 20.9 | −76.90 |
| WSM | Samoa | Pacific Islands | C | current_season_percentile | 7.2 | 59.8 | +52.63 |
| WLF | Wallis And Futuna | Pacific Islands | C | current_season_percentile | 5.1 | 48.0 | +42.94 |
| KIR | Kiribati | Pacific Islands | C | current_season_percentile | 70.9 | 40.7 | −30.22 |
| KHM | Cambodia | East & Southeast Asia | C | current_season_percentile | 72.7 | 95.6 | +22.88 |
| AFG | Afghanistan | South Asia | C | current_season_percentile | 31.8 | 51.0 | +19.16 |
| BGD | Bangladesh | South Asia | C | current_season_percentile | 48.6 | 66.6 | +18.06 |
| CHN | China | East & Southeast Asia | C | current_season_percentile | 21.8 | 39.0 | +17.16 |
| MRT | Mauritania | Sub-Saharan Africa | C | current_season_percentile | 18.3 | 34.6 | +16.36 |
| MDV | Maldives | South Asia | C | current_season_percentile | 73.2 | 89.5 | +16.28 |

### 8.2 Consolidated citation list

1. Outbreak News Today, Cambodia 232% increase / July 2026 case update — https://outbreaknewstoday.substack.com/p/cambodia-reports-232-increase-in
2. La 1ère, Wallis-et-Futuna epidemic slowing in Futuna, progressing in Wallis (17 Jul) — https://la1ere.franceinfo.fr/wallisfutuna/dengue-l-epidemie-ralentit-a-futuna-mais-progresse-a-wallis-1711747.html
3. U.S. Embassy Vanuatu, Health Alert: dengue outbreak declared, South Efate (26 Jun) — https://vt.usembassy.gov/health-alert-the-vanuatu-ministry-of-health-declared-a-dengue-outbreak-in-south-efate-shefa-province-june-26-2026/
4. ReliefWeb, Vanuatu Dengue Situation Update 01 (18 May) — https://reliefweb.int/report/vanuatu/vanuatu-dengue-situation-update-01-18-may-2026
5. Outbreak News Today, Samoa dengue outbreak continues into 2026 — https://outbreaknewstoday.substack.com/p/samoa-dengue-outbreak-continues-into
6. WHO Western Pacific, Samoa mobilizes dengue outbreak response — https://www.who.int/westernpacific/newsroom/feature-stories/item/samoa-mobilizes-dengue-outbreak-response-with-support-from-who-and-partners
7. Free Malaysia Today, health ministry warns of nationwide dengue risk (21 Aug) — https://www.freemalaysiatoday.com/category/nation/2026/08/21/health-ministry-warns-of-increased-nationwide-dengue-risk-as-cases-rise
8. Sowetan/wire, Klang Valley dengue cases up 56% (21 Aug) — https://www.sowetan.co.za/news/world/2026-08-21-dengue-fever-cases-up-56-in-klang-valley-health-ministry-warns/
9. Islands Business, New Caledonia reports spike in dengue cases (undated) — https://islandsbusiness.com/news-break/new-caledonia-reports-spike-in-dengue-cases/
10. Frontiers, Burkina Faso dengue incident management system, 2023 retrospective (2026) — https://www.frontiersin.org/journals/tropical-diseases/articles/10.3389/fitd.2026.1754235/full
11. PMC, delayed medical consultation impact on Burkina Faso 2023 outbreak (2026) — https://pmc.ncbi.nlm.nih.gov/articles/PMC13486771/
12. WHO WPRO, Dengue Situation Update 743 (16 Apr) — https://cdn.who.int/media/docs/default-source/wpro---documents/emergency/surveillance/dengue/dengue_20260416.pdf
13. PMC, imported dengue/Zika coinfection, Sichuan, China (2026) — https://pmc.ncbi.nlm.nih.gov/articles/PMC13171624/
14. Atlas Visual del Dengue, dengue en Bolivia 2025–2026 — https://denguevisualatlas.com/es/dengue-en-bolivia-situacion-actual-zonas-de-riesgo-y-guia-de-prevencion-2025-2026/
15. Pathogenos, Dengue in Latin America 2026 outbreak updates — https://pathogenos.com/dengue-in-latin-america-in-2026-the-latest-outbreak-updates/
16. Xinhua, Nepal dengue spreads on World Mosquito Day (20 Aug) — https://english.news.cn/20260820/ca290954e03b473f963c089a2cf8a04b/c.html
17. Rising Nepal Daily, 19,599 dengue cases reported throughout country — https://risingnepaldaily.com/news/50432
18. Dubai Eye, Bangladesh dengue outbreak accelerates, hospitals under strain (Sept 2026) — https://www.dubaieye1038.com/news/international/bangladesh-dengue-outbreak-accelerates-as-hospitals-come-under-strain/
19. CDC, Areas with Risk of Dengue (Cuba high-transmission status, accessed 2 Sep) — https://www.cdc.gov/dengue/areas-with-risk/index.html
20. PAHO/WHO, Dengue Epidemiological Situation, Region of the Americas, Epi Week 32 2026 — https://www.paho.org/en/documents/dengue-epidemiological-situation-region-americas-epidemiological-week-32-2026
21. CIDRAP, European nations report more local detections of chikungunya, dengue — https://www.cidrap.umn.edu/chikungunya/european-nations-report-more-local-detections-chikungunya-dengue
22. Medical Daily, dengue surpasses 500 US cases, mosquito range expanding north (2026) — https://www.medicaldaily.com/dengue-fever-2026-us-cases-mosquito-expanding-north-476323
23. ScienceDirect, NowcastPNN attention-based probabilistic neural network, São Paulo (Mar 2026) — https://www.sciencedirect.com/science/article/pii/S1755436525000684
24. PMC, hybrid wavelet/ML weekly dengue forecasting (Jul 2026) — https://pmc.ncbi.nlm.nih.gov/articles/PMC13349185/
25. PMC, comparative ML evaluation, Brazilian capital municipalities (Aug 2026) — https://pmc.ncbi.nlm.nih.gov/articles/PMC13476183/
26. PMC, deep learning climatic/temporal dengue dynamics, Bangladesh (2026) — https://pmc.ncbi.nlm.nih.gov/articles/PMC13362098/
27. Medical Xpress, India approves Takeda's Qdenga dengue vaccine (Jul 2026) — https://medicalxpress.com/news/2026-07-india-dengue-vaccine.html
28. BioPharma Dive, Sanofi discontinuing US dengue vaccine marketing (2026) — https://www.biopharmadive.com/news/dengue-sanofi-takeda-vaccine-qdenga-dengvaxia/730846/
