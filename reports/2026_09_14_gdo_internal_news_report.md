# GDO Internal News Report — 2026-09-14

*Source: Global Dengue Observatory (accessed 2026-09-14).*

## 1. Header

- **Report date:** 2026-09-14 (Monday routine run)
- **Active snapshot:** `snapshots/2026_09_07/` — **unchanged since 2026-09-04** (source data vintage, `target_render_date`). Source commit: `92c2f221` (DENV_global_observatory `Output/2026_09_04/`). No new snapshot folder created this week.
- **Pull status this week:** **news-only week.** `target_render_date` (most recent of this month's 4th/18th, last month's 18th, strictly before today) resolves to 2026-09-04 — the same vintage already captured in `snapshots/2026_09_07/`. Step 1's fetch/diff was skipped per Step 0.5; this run reuses that snapshot's `latest_status.csv`/`movers.csv` unchanged.
- **Countries covered:** 84.

## 2. This week's snapshot

Global picture across the 84 tracked countries/territories, from `latest_status.csv` only. Unchanged from last week's report, since the underlying pull hasn't advanced.

**Cumulative severity band** (percentile_cumulative, current position vs. seasonal-to-date expectation):

| Band | Countries |
|---|---|
| Normal | 35 |
| Low | 19 |
| Extremely High | 11 |
| High | 10 |
| Unknown | 5 |
| Extremely Low | 4 |

The 11 at **Extremely High** cumulative severity: Afghanistan, Cambodia, Cook Islands, Cuba, Guyana, Kenya, Maldives, Sri Lanka, Sudan, Timor-Leste, and Wallis and Futuna.

**Current-season severity band** (current_season_percentile, i.e. how this season is tracking overall):

| Band | Countries |
|---|---|
| Low | 35 |
| Normal | 19 |
| Extremely Low | 17 |
| Unknown | 5 |
| Extremely High | 4 |
| High | 4 |

Current-season **Extremely High**: Cuba (percentile 100.0), Kenya (99.9), Guyana (96.7), Cambodia (95.6). Current-season **High**: Maldives (89.5), Sri Lanka (84.9), Sudan (81.2), Suriname (76.4).

**Caveat — data recency.** Of this week's ten targeted countries (Section 3), two (Bolivia, Nepal) have a latest observed month of 2026-08-01 (~1.4 months stale, within GDO's 1–2 month nowcast sweet spot); seven (Burkina Faso, Cambodia, China, New Caledonia, Vanuatu, Wallis and Futuna, Samoa) sit at 2026-07-01 (~2.4 months stale, just beyond the sweet spot's upper end); Malaysia sits at 2026-06-01 (~3.4 months stale, clearly beyond it — treat its figures as lower-confidence). These are the same nowcast vintages as last week's report; they have not moved, because no new pull has happened. **Small-baseline/large-ratio instability:** Vanuatu (monthly ratio 15.9× off a ~7.6-case seasonal baseline) and Wallis and Futuna (9.2× off a ~6.7-case baseline) both have tiny expected-case baselines — treat their "running well above" monthly reads as noisy on their own.

## 3. News — targeted (10 countries)

**Country selection note:** `movers.csv` is unchanged from last week (same snapshot, no new pull) — it still flags 19 Category A and 11 Category B rows (27 unique countries once de-duplicated), well beyond the 10-country cap. Since the underlying data hasn't moved, this week reuses last week's same 10-country selection (Cambodia, Wallis and Futuna, Vanuatu, Samoa, Malaysia, New Caledonia, Burkina Faso, China, Bolivia, Nepal) rather than re-deriving a different judgement call from an identical table — but every news search below is fresh, covering the ~2 weeks up to 2026-09-14.

### Cambodia (Category A — severity interpretation: Above average → Rare bad event, Extremely High cumulative *and* current-season; Category C — current-season percentile 72.7 → 95.6)
- GDO figures: 29,580 reported cases (latest observed month 2026-07-01, ~2.4 months stale). Cumulative percentile 99.3 (Extremely High); current-season percentile 95.6 (Extremely High). Estimated total seasonal cases: 108,342. Monthly ratio: running well above (6.3×).
- News: no item confirmed within the last ~2 weeks — the most recent figures found remain the mid-July count of 28,074 cumulative 2026 cases and 38 deaths (case-fatality rate 0.1%), a 58.1% rise on the same period in 2025 and past the epidemic threshold since epi week 24; full-year 2025 totalled 63,016 cases (79 deaths), a 232% rise on 2024. No newer update surfaced this week — flag to the researcher as a data gap, not a sign the situation has eased. [Outbreak News Today, 12 Jul](https://outbreaknewstoday.substack.com/p/cambodia-reports-232-increase-in)

### Wallis and Futuna (Category A — severity interpretation: Below average → Rare bad event, Extremely High cumulative; Category B — monthly ratio: running well below → running well above; Category C — current-season percentile 5.1 → 48.0)
- GDO figures: 61 reported cases (latest observed month 2026-07-01, ~2.4 months stale). Cumulative percentile ~100.0 (Extremely High). Current-season percentile 48.0 (Normal). Estimated total seasonal cases: 740. **Caveat:** small seasonal baseline (~6.7 cases/month expected) makes the 9.2× monthly ratio noisy in isolation.
- News: no item confirmed within the last ~2 weeks, in either English or French. Background unchanged from last week: local transmission was first confirmed in Futuna on 22 April 2026, the epidemic was declared mid-May, and by mid-July it was reported to be slowing in Futuna while progressing in Wallis. [La 1ère, 17 Jul](https://la1ere.franceinfo.fr/wallisfutuna/dengue-l-epidemie-ralentit-a-futuna-mais-progresse-a-wallis-1711747.html)

### Vanuatu (Category A — severity interpretation: Average → Above average; Category B — monthly ratio: running well below → running well above)
- GDO figures: 120 reported cases (latest observed month 2026-07-01, ~2.4 months stale). Cumulative percentile 92.1 (High); current-season percentile 36.7 (Normal). Estimated total seasonal cases: 297. **Caveat:** small seasonal baseline (~7.6 cases/month expected) makes the 15.9× monthly ratio noisy on its own, though independently corroborated by a growing confirmed case count below.
- News: no update confirmed within the last ~2 weeks. Most recent confirmed figure remains 112 confirmed cases (since 14 June) as of the 31 August situation report, with ongoing local transmission across South-West Efate, most-affected area Erakor. Outbreak first declared 26 June 2026. [ReliefWeb, Vanuatu Dengue Outbreak Situation Report #6, 31 Aug](https://reliefweb.int/report/vanuatu/vanuatu-dengue-outbreak-situation-report-6-south-west-efate-shefa-province) · [U.S. Embassy Vanuatu, 26 Jun](https://vt.usembassy.gov/health-alert-the-vanuatu-ministry-of-health-declared-a-dengue-outbreak-in-south-efate-shefa-province-june-26-2026/)

### Samoa (Category A — severity interpretation: Average → Above average; Category C — current-season percentile 7.2 → 59.8, the largest current-season swing in this snapshot)
- GDO figures: 167 reported cases (latest observed month 2026-07-01, ~2.4 months stale). Cumulative percentile 87.8 (High); current-season percentile 59.8 (Normal). Estimated total seasonal cases: 15,279. Monthly ratio: running well below (0.17×) — a striking divergence from the sharp current-season percentile jump above; flag both figures to the researcher rather than picking one.
- News: outbreak described as ongoing as of 2026-09-13 per regional tracking, but no new case-count figure could be confirmed within the window. Most recent hard numbers: 132 new cases in the week of 4–10 May (a 33% fall on the previous week); 17,778 clinically diagnosed cases (5,234 lab-confirmed) since January 2025, 9 deaths total, DENV-1 (68%)/DENV-2 (32%) co-circulating, 74% of cases in children under 15, as of late March. [BEACON, event tracker, accessed 13 Sep](https://beaconbio.org/en/event/?eventid=dfad95fd-d4df-42ba-be95-28b3c048279b) · [Samoa Observer, 4–10 May](https://www.samoaobserver.ws/category/samoa/120060) · [Outbreak News Today, 22 Mar](https://outbreaknewstoday.substack.com/p/samoa-dengue-outbreak-continues-into)

### Malaysia (Category B — monthly ratio: running slightly below → running well above)
- GDO figures: 8,756 reported cases (latest observed month 2026-06-01, ~3.4 months stale — beyond GDO's nowcast sweet spot; treat as lower-confidence). Cumulative percentile 59.9 (Low); current-season percentile 24.7 (Low). Estimated total seasonal cases: 80,971.
- News: **fresh this week.** Nationwide cases up 66% to 65,979 as of epidemiological week 35 (vs. 39,616 over the same period in 2025); deaths up 93.8% to 62 (vs. 32 last year). Cabinet is discussing gotong-royong (community clean-up) programmes coordinated by the Housing and Local Government Ministry (KPKT) in red-zone areas. This is a marked escalation on the 56% year-on-year rise reported three weeks ago — worth flagging that the gap between GDO's stale (~3.4-month) nowcast and the live ministry count is widening further. [Malay Mail, 9 Sep](https://www.malaymail.com/news/malaysia/2026/09/09/dengue-cases-soar-66pc-deaths-hit-62-in-malaysia-almost-double-2025-toll/234576)

### New Caledonia (Category B — monthly ratio: running well below → running well above)
- GDO figures: 57 reported cases (latest observed month 2026-07-01, ~2.4 months stale). Cumulative percentile 70.2 (Low); current-season percentile 13.8 (Low). Estimated total seasonal cases: 2,313.
- News: no item confirmed within the last ~2 weeks. Most recent figure remains 1,786 cases reported since January 2026 as of 21 May, DENV-1 predominant, limited hospitalisations and no reported severe/ICU cases, transmission more intense outside Greater Nouméa, with no dengue vaccination campaign currently in place. [Islands Business, 21 May](https://islandsbusiness.com/news-break/new-caledonia-reports-spike-in-dengue-cases/)

### Burkina Faso (Category A — severity interpretation: Cannot determine → Above average)
- GDO figures: 4,138 reported cases (latest observed month 2026-07-01, ~2.4 months stale). Cumulative percentile 93.3 (High); current-season percentile 44.4 (Normal). Estimated total seasonal cases: 170,427.
- News: **fresh this week, and directionally consistent.** The Governor of Oubritenga region (central Burkina Faso) issued an alert on 10 September over an "unusual and rapid increase in dengue cases" in Ziniaré and Zorgho. This is the first live 2026 situation-report-style item found for Burkina Faso — it corroborates GDO's own reading, which had just become classifiable this snapshot (from "Cannot determine" to "Above average"). [Wakat Séra, 10 Sep](https://www.wakatsera.com/burkina-une-augmentation-inhabituelle-et-rapide-de-cas-de-dengue-a-ziniare-et-zorgho/)

### China (Category A — severity interpretation: Above average → Cannot determine; Category C — current-season percentile 21.8 → 39.0)
- GDO figures: 1,120 reported cases (latest observed month 2026-07-01, ~2.4 months stale). Cumulative severity is **"Cannot determine"** (percentile unavailable this pull) — a data-availability caveat about GDO's own pipeline, not an epidemiological claim about China. Current-season percentile 39.0 (Normal). Estimated total seasonal cases: 40,458.
- News: no fresh case-count item confirmed within the last ~2 weeks. Two contextual findings worth flagging: (1) historical analysis shows August–October typically account for the bulk of China's annual dengue cases, with September the usual peak month — timely context even without a fresh number; (2) a Guangdong genomic study found evidence of local overwintering transmission from an early pre-season 2025 case, raising the possibility of earlier/extended 2026 season activity in subtropical China. [PMC, China 2005–2025 seasonality](https://pmc.ncbi.nlm.nih.gov/articles/PMC13187653/) · [PMC, Guangdong overwintering](https://pmc.ncbi.nlm.nih.gov/articles/PMC13497276/)

### Bolivia (Category A — severity interpretation: Above average → Average; Category B — monthly ratio: running well above → running slightly below)
- GDO figures: 472 reported cases (latest observed month 2026-08-01, ~1.4 months stale — within GDO's sweet spot). Cumulative percentile 46.8 (Normal); current-season percentile 0.1 (Extremely Low) — among the lowest readings in the entire dataset. Estimated total seasonal cases: 27,994.
- News: no fresh item confirmed within the last ~2 weeks. PAHO's most recent regional bulletin (mid-February) described Bolivia as in a "favourable control phase" with low dengue transmission, while flagging a concurrent chikungunya surge (5,371 cases over 8 weeks, 84.9% concentrated in Santa Cruz, 5 deaths) — worth noting to the researcher as a related vector-borne disease to watch even as dengue itself eases. Bolivia's own Ministry of Health corroborates a downward/stable dengue trend versus the prior year. [PAHO, Actualización Epidemiológica, 18 Feb](https://www.paho.org/sites/default/files/2026/02/2026-18feb-phe-actualizacion-dengue-es-final1.pdf) · [Ministerio de Salud y Deportes de Bolivia, Boletines 2026](https://www.minsalud.gob.bo/9104-boletines-epidemiologicos-2026)

### Nepal (Category A — severity interpretation: Above average → Average)
- GDO figures: 1,776 reported cases (latest observed month 2026-08-01, ~1.4 months stale — within GDO's sweet spot). Cumulative percentile 74.6 (Normal, just below the High threshold); current-season percentile 50.8 (Normal). Estimated total seasonal cases: 13,444. Monthly ratio: tracking near baseline.
- News: no hard case-count update confirmed within the strict ~2-week window, though two opinion pieces published this week (14 September) discuss dengue's climate-driven expansion beyond Nepal's traditional lowland range into hill and high-altitude districts. Most recent hard figures remain slightly lower than GDO's own count: 2,844 cases across 74 of 77 districts for 1 January–15 August (EDCD data via Xinhua, 20 Aug), Gandaki Province highest (1,010), then Koshi (674), Lumbini (435), Bagmati (427); 2 confirmed dengue deaths for the year as of that date. A district-level item flagged Baglung district cases climbing to 289 within one month as of 15 August, already surpassing the prior full fiscal year's total there (250). [Kathmandu Post, 14 Sep — climate/dengue opinion](https://kathmandupost.com/columns/2026/09/14/why-nepal-s-climate-crisis-is-also-a-public-health-emergency) · [Xinhua, 20 Aug](https://english.news.cn/asiapacific/20260820/b75ee9f2ee9947f59f49604180a9c25e/c.html) · [Kathmandu Post, Baglung, 15 Aug](https://kathmandupost.com/national/2026/08/15/dengue-cases-surge-to-289-in-baglung-within-a-month)

## 4. News — general scan (5 items)

Independent broad scan, capped at 5; includes GDO-tracked countries with dramatic recent news outside this week's 10-country target list, and non-endemic/no-GDO-data settings per the routine's instruction.

1. **Bangladesh, 2026-09-14 (ongoing, worsening)** — 52 deaths recorded in the first 13 days of September alone — the highest monthly toll of the year — bringing the cumulative 2026 death toll to 149, with 51,837 hospitalised so far. Continues (and sharpens) the surge flagged in last week's report. GDO-tracked but not among this week's 10 targeted countries; GDO's own latest observed month (2026-07-01, ~2.4 months stale) predates this surge entirely. [SocialNews.xyz, 14 Sep](https://www.socialnews.xyz/2026/09/14/bangladesh-dengue-outbreak-worsens-as-52-die-in-just-13-days/)
2. **Europe, week 37 (5–11 Sep 2026)** — ECDC's weekly communicable disease threats report recorded a sharp rise in indigenous (locally-acquired) dengue across France, Spain and Italy; France reported 57 locally-transmitted cases, Spain 8 cases in Catalonia. Non-endemic, no GDO nowcast coverage — continues the "dengue's reach is expanding into Europe" theme flagged in prior weeks. [ECDC, Surveillance and updates on dengue](https://www.ecdc.europa.eu/en/dengue-fever/surveillance-and-disease-data)
3. **Cuba, 2026-09-02** — Cuba met ECDC's criteria for "high transmission" travel-associated dengue status (10 or more traveller cases reported in the prior three months). Consistent with GDO's own reading: Cuba remains at Extremely High on both cumulative (~100.0) and current-season (100.0) percentiles this week (Section 2), independently corroborated by traveller-surveillance data. [ECDC, Dengue worldwide overview](https://www.ecdc.europa.eu/en/dengue-monthly)
4. **Florida, United States, as of 2026-09-01** — 33 locally-acquired dengue cases reported this season. Non-endemic in GDO terms, but continues a running "dengue's US range is expanding" thread alongside prior weeks' Europe items. [Custom Map Poster summary, 1 Sep](https://custommapposter.com/article/florida-s-dengue-outbreak-what-you-need-to-know)
5. **Imported cases, non-endemic Europe (general)** — Case-report literature continues to document travel-associated dengue in patients returning from the Maldives and Brazil who become symptomatic on arrival in Europe — a reminder that GDO's tracked-country list doesn't capture every dengue-relevant story; imported-case volume itself is a signal worth occasional coverage. [Frontiers in Tropical Diseases, case report](https://www.frontiersin.org/journals/tropical-diseases/articles/10.3389/fitd.2026.1771412/full)

## 5. Trend since last update

**No new data this week.** This is a news-only week — `target_render_date` (2026-09-04) is unchanged from last week's pull, so `latest_status.csv` and `movers.csv` are byte-identical to the 2026-09-07 report. There is no new Category A/B/C movement to report; see that report's Section 5 (or Section 8.1 below, reproduced unchanged) for the last recorded set of crossings. The next genuine data-pull week is expected around 2026-09-18 (this month's 18th), per Step 0.5's rule.

## 6. Social-media candidate flags

Ranked short-list, for the researcher drafting Tuesday's posts. With no new GDO data this week, this list leans on fresh news corroborating or updating last week's GDO-flagged movers, rather than new nowcast movement.

1. **Malaysia — escalating, and now with a bigger, more current number than last week's.** Ministry of Health figures jumped from a 56% year-on-year rise (58,079 cases, mid-August) to a 66% rise (65,979 cases, epi-week 35) in three weeks, with deaths nearly doubling (62 vs. 32 last year). GDO's own monthly ratio already flagged "running well above" last pull. *Caveat: GDO's raw case figure (8,756) is ~3.4 months stale and far below the ministry's live count (65,979) — don't juxtapose the two numbers without explaining the vintage gap.*
2. **Burkina Faso — a live, dated alert that corroborates GDO's own severity upgrade.** A regional governor's 10 September alert over an "unusual and rapid increase" in Ziniaré and Zorgho is the first live 2026 situation update found for the country, and it lines up with GDO's own severity_interpretation crossing from "Cannot determine" to "Above average" (High cumulative band) two pulls ago. *Caveat: the alert is regional (Oubritenga), not national — don't extrapolate to a countrywide claim GDO's own aggregate figures don't support.*
3. **Bangladesh — continues to be the most dramatic real-world number, and it's worsening, not just persisting.** 52 deaths in 13 days of September is the highest monthly toll of the year, pushing the cumulative total to 149. Outside GDO's own 10-country target list and well outside its nowcast vintage (July data). *Caveat: as flagged last week — do not attribute the September figures to GDO; they're government/press figures on a data vintage GDO's nowcast hasn't reached.*
4. **Cambodia — still GDO's strongest internally-corroborated story, but the news trail has gone quiet.** Current-season percentile at 95.6, both severity measures Extremely High, and the underlying 58% year-on-year case rise (mid-July figure) remains the best available corroboration — but nothing newer surfaced this week despite a dedicated search. Flag as "ongoing, unconfirmed recently" rather than claiming fresh escalation. *Caveat: don't imply the situation has newly worsened — no news update means no update, not stability.*
5. **Europe (France/Spain/Italy) — building "reach is expanding" thread, now with a harder weekly figure.** ECDC's week-37 threats report puts a number on locally-acquired dengue in France (57 cases) for the first time in this report's coverage, alongside Spain (8, Catalonia) and Italy. Good for the recurring non-endemic-spread narrative; ties together Florida/Cuba/imported-case items in Section 4. *No major caveat — ECDC is a primary surveillance source, not press coverage.*

## 7. Scientific literature findings

Lighter-effort pass; a handful of recent items across forecasting, climate drivers, surveillance and vaccine policy.

- **Forecasting:** A systematic review of dengue forecasting models (2014–2024) synthesises methods across the field, noting the growing dominance of machine-learning approaches using weather data as central inputs. *medRxiv*, Feb 2026. [medRxiv](https://www.medrxiv.org/content/10.64898/2026.02.18.26346534v1.full.pdf)
- **Forecasting/climate:** A causal, spatiotemporal deep-learning framework for dengue forecasting and extreme-outbreak risk in Vietnam under climate variability, built on weekly district-level surveillance plus 17 satellite-derived meteorological variables. *PubMed*, 2026. [PubMed](https://pubmed.ncbi.nlm.nih.gov/41860701/)
- **Vaccine policy:** A comparative analysis of 18 advisory bodies across 17 countries finds substantially different Qdenga (TAK-003) guidance for travellers despite shared underlying trial evidence — a reminder that "the data" doesn't map neatly onto "the guidance" when the researcher is drafting anything vaccine-related. *PubMed*, Mar–Apr 2026. [PubMed](https://pubmed.ncbi.nlm.nih.gov/42485451/)
- **Vaccine policy:** A Singapore modelling study on adult dengue vaccination, intended to inform national vaccine policy decisions. *medRxiv preprint*, 2026. [medRxiv](https://www.medrxiv.org/content/10.1101/2025.10.01.25337064.full.pdf)
- **Surveillance methods:** A systematic review and meta-analysis of methodological approaches to detecting dengue virus in wastewater, assessing positivity rates as a surveillance signal — relevant to GDO's own interest in alternative/earlier-warning data sources. *PMC*, accepted Apr 2026. [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC13211638/)
- **Climate drivers:** The Guangdong overwintering-transmission genomic study already cited in Section 3 (China) belongs here too — it challenges assumptions of strict seasonality for subtropical dengue transmission, with direct relevance to forecasting methodology generally, not just China. *PMC*, 2026. [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC13497276/)

## 8. Appendix

### 8.1 `movers.csv` (active snapshot — unchanged from last week; reproduced for reference)

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
3. ReliefWeb, Vanuatu Dengue Outbreak Situation Report #6 (31 Aug) — https://reliefweb.int/report/vanuatu/vanuatu-dengue-outbreak-situation-report-6-south-west-efate-shefa-province
4. U.S. Embassy Vanuatu, Health Alert: dengue outbreak declared, South Efate (26 Jun) — https://vt.usembassy.gov/health-alert-the-vanuatu-ministry-of-health-declared-a-dengue-outbreak-in-south-efate-shefa-province-june-26-2026/
5. BEACON event tracker, Samoa dengue event (accessed 13 Sep) — https://beaconbio.org/en/event/?eventid=dfad95fd-d4df-42ba-be95-28b3c048279b
6. Samoa Observer, seven hospitalised, 132 new dengue cases (4–10 May) — https://www.samoaobserver.ws/category/samoa/120060
7. Outbreak News Today, Samoa dengue outbreak continues into 2026 (22 Mar) — https://outbreaknewstoday.substack.com/p/samoa-dengue-outbreak-continues-into
8. Malay Mail, dengue cases soar 66pc, deaths hit 62 in Malaysia (9 Sep) — https://www.malaymail.com/news/malaysia/2026/09/09/dengue-cases-soar-66pc-deaths-hit-62-in-malaysia-almost-double-2025-toll/234576
9. Islands Business, New Caledonia reports spike in dengue cases (21 May) — https://islandsbusiness.com/news-break/new-caledonia-reports-spike-in-dengue-cases/
10. Wakat Séra, unusual and rapid increase in dengue cases, Ziniaré/Zorgho, Burkina Faso (10 Sep) — https://www.wakatsera.com/burkina-une-augmentation-inhabituelle-et-rapide-de-cas-de-dengue-a-ziniare-et-zorgho/
11. PMC, comparative epidemiology of dengue in China 2005–2025 — https://pmc.ncbi.nlm.nih.gov/articles/PMC13187653/
12. PMC, genomic/epidemiological evidence of overwintering transmission, Guangdong, China — https://pmc.ncbi.nlm.nih.gov/articles/PMC13497276/
13. PAHO, Actualización Epidemiológica dengue, Región de las Américas (18 Feb) — https://www.paho.org/sites/default/files/2026/02/2026-18feb-phe-actualizacion-dengue-es-final1.pdf
14. Ministerio de Salud y Deportes de Bolivia, Boletines Epidemiológicos 2026 — https://www.minsalud.gob.bo/9104-boletines-epidemiologicos-2026
15. Kathmandu Post, why Nepal's climate crisis is also a public-health emergency (14 Sep) — https://kathmandupost.com/columns/2026/09/14/why-nepal-s-climate-crisis-is-also-a-public-health-emergency
16. Xinhua, dengue cases spread across Nepal as it marks World Mosquito Day (20 Aug) — https://english.news.cn/asiapacific/20260820/b75ee9f2ee9947f59f49604180a9c25e/c.html
17. Kathmandu Post, dengue cases surge to 289 in Baglung within a month (15 Aug) — https://kathmandupost.com/national/2026/08/15/dengue-cases-surge-to-289-in-baglung-within-a-month
18. SocialNews.xyz, Bangladesh dengue outbreak worsens as 52 die in just 13 days (14 Sep) — https://www.socialnews.xyz/2026/09/14/bangladesh-dengue-outbreak-worsens-as-52-die-in-just-13-days/
19. ECDC, Surveillance and updates on dengue (week 37 threats report) — https://www.ecdc.europa.eu/en/dengue-fever/surveillance-and-disease-data
20. ECDC, Dengue worldwide overview (Cuba high-transmission status, accessed 2 Sep) — https://www.ecdc.europa.eu/en/dengue-monthly
21. Custom Map Poster, Florida's dengue outbreak — what you need to know (1 Sep) — https://custommapposter.com/article/florida-s-dengue-outbreak-what-you-need-to-know
22. Frontiers in Tropical Diseases, case report: clinical presentation of imported dengue cases — https://www.frontiersin.org/journals/tropical-diseases/articles/10.3389/fitd.2026.1771412/full
23. medRxiv, dengue forecasting models: a systematic review (Feb 2026) — https://www.medrxiv.org/content/10.64898/2026.02.18.26346534v1.full.pdf
24. PubMed, causal and spatiotemporal deep learning for dengue forecasting, Vietnam — https://pubmed.ncbi.nlm.nih.gov/41860701/
25. PubMed, shared evidence, different recommendations: Qdenga guidance for travellers — https://pubmed.ncbi.nlm.nih.gov/42485451/
26. medRxiv, adult dengue vaccination in Singapore: a modelling study to inform policy — https://www.medrxiv.org/content/10.1101/2025.10.01.25337064.full.pdf
27. PMC, methodological approaches to dengue virus detection in wastewater — https://pmc.ncbi.nlm.nih.gov/articles/PMC13211638/
