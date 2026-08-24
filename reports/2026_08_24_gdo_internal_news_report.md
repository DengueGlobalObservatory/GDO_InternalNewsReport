# GDO Internal News Report — 2026-08-24

*Source: Global Dengue Observatory (accessed 2026-08-24).*

## 1. Header

- **Report date:** 2026-08-24 (Monday routine run)
- **Active snapshot:** `snapshots/2026_08_24/` — **new pull this week**. Source data vintage (`target_render_date`): 2026-08-18. Source commit: `8f5519d7` (DENV_global_observatory `Output/2026_08_18/`). Prior snapshot: `snapshots/2026_08_12/` (vintage 2026-08-04) — this is the first genuine week-over-week comparison GDO has had (the prior pull was itself the first-ever pull, so its `movers.csv` was empty).
- **Pull status this week:** **pull week.** `target_render_date` advanced from 2026-08-04 to 2026-08-18, so Step 1's fetch/diff ran in full.
- **Countries covered:** 84.

## 2. This week's snapshot

Global picture across the 84 tracked countries/territories, from `latest_status.csv` only.

**Cumulative severity band** (percentile_cumulative, current position vs. seasonal-to-date expectation):

| Band | Countries |
|---|---|
| Normal | 30 |
| Low | 27 |
| High | 11 |
| Extremely High | 9 |
| Extremely Low | 4 |
| Unknown | 3 |

The 9 at **Extremely High** cumulative severity: Cuba, Kenya, Sudan, Maldives, Timor-Leste, Guyana, Afghanistan, Cook Islands, and — new to this band this week — **Sri Lanka**.

**Current-season severity band** (current_season_percentile, i.e. how this season is tracking overall):

| Band | Countries |
|---|---|
| Low | 35 |
| Extremely Low | 22 |
| Normal | 17 |
| Unknown | 5 |
| Extremely High | 4 |
| High | 1 |

The same four countries remain at **current-season Extremely High**: Cuba (percentile 100), Kenya (99.7), Cook Islands (97.8) and Guyana (95.7) — unchanged from last week's reading, though Guyana's *monthly* ratio has now swung to "running well below" (see Section 3) even as its season-to-date standing stays extreme.

**Caveat — data recency.** Of this week's ten targeted countries (Section 3), seven have a latest observed month of 2026-07-01 (~1.8 months stale, near the healthy end of GDO's 1–2 month nowcast sweet spot); three — Barbados, Antigua and Barbuda, Guyana — sit at 2026-06-01 (~2.8 months stale, just beyond that sweet spot). Treat figures from the latter three as somewhat lower-confidence reads. No small-baseline/large-ratio instability (a tiny expected count swinging the ratio wildly) was flagged among this week's ten targeted countries.

## 3. News — targeted (10 countries)

**Country selection note:** `movers.csv` flagged 4 Category A (severity-interpretation band changes) and 7 Category B (monthly-ratio-descriptor changes) countries this week — 10 unique countries in total once de-duplicated (Panama appears in both). Per the routine's prioritisation rule (A/B over C when there are more than 10 flagged), all 10 targeted countries below come from A/B; none of the 10 Category C (percentile-only) movers needed to be added to reach the cap.

### Sri Lanka (Category A — cumulative severity moved to Extremely High; Category C — current-season percentile 37.7 → 82.2)
- GDO figures: 29,973 reported cases in the latest observed month (2026-07-01, ~1.8 months stale). Cumulative percentile 97.1 (Extremely High); current-season percentile jumped to 82.2 (High) — the largest single-week percentile move of any country this snapshot. Estimated total seasonal cases: 153,381. Monthly ratio descriptor: running well above.
- News: WHO and Sri Lanka's Ministry of Health convened a "National Dengue Review 2026" (11–14 Aug) to reassess response priorities. Local wire reporting put cumulative 2026 cases above 90,000 by 11 Aug, with the death toll rising from 68 (13 Aug) to 69 alongside 92,854 cumulative cases (19 Aug) — Western Province (Gampaha, Colombo) worst affected. 2026 is on track to be the largest outbreak since 2017. [WHO Sri Lanka, 14 Aug](https://www.who.int/srilanka/news/detail/14-08-2026-national-dengue-review-2026-identifies-priorities-to-strengthen-sri-lanka-s-dengue-preparedness-and-response) · [Newswire, 19 Aug](https://www.newswire.lk/2026/08/19/sri-lankas-dengue-death-toll-rises-to-69/) · [ReliefWeb/IFRC DREF Operation](https://reliefweb.int/report/sri-lanka/sri-lanka-dengue-outbreak-2026-dref-operation-mdrlk024)

### Guyana (Category B — monthly ratio: running well above → running well below)
- GDO figures: 710 reported cases (latest observed month 2026-06-01, ~2.8 months stale — beyond the sweet spot). Cumulative percentile 98.8 and current-season percentile 95.7 both remain Extremely High even as the monthly trend has cooled sharply. Estimated total seasonal cases: 83,305.
- News: no dengue-specific item confirmed within the last ~2 weeks. Most recent background found dates to 9 January 2026 (Region 6 rainy-season case rise) — well outside the window, so the news picture here is thin relative to GDO's still-extreme season-to-date standing.

### Panama (Category A — severity interpretation: Average → Above average; Category B — monthly ratio: running well below → running slightly below; Category C — current-season percentile 28.8 → 35.3)
- GDO figures: 1,056 reported cases (latest observed month 2026-07-01, ~1.8 months stale). Cumulative percentile 80.8 (High). Estimated total seasonal cases: 16,120.
- News: Panama's Ministry of Health (Minsa), via Prensa Latina (17 Aug), reported 5,318 cumulative 2026 dengue cases, 628 hospitalisations and 16 deaths — highest fatality counts in Bocas del Toro and Los Santos — with children aged 10–14 the most affected group (167 per 100,000; national incidence 115 per 100,000). Minsa frames vector-control efforts as having reduced cases year-on-year despite the toll. [Prensa Latina, 17 Aug](https://www.plenglish.com/news/2026/08/17/panama-records-over-5000-dengue-cases-children-make-up-the-majority/) · [Minsa Panamá dengue dashboard](https://www.minsa.gob.pa/informacion-salud/dengue-2026)

### Peru (Category B — monthly ratio: running well below → running well above)
- GDO figures: 6,202 reported cases (latest observed month 2026-07-01, ~1.8 months stale). This is the largest directional swing of any Category B mover this week. Estimated total seasonal cases: 49,003.
- News: MINSA reported 42,440 cumulative 2026 cases and 48 deaths nationally (data through 8 Aug, reported 18 Aug) — a 41% rise on the same period in 2025 — led by Piura, San Martín and La Libertad; several regions flagged medicine-supply difficulties (CENARES budget only 3.6% executed). Separately, MINSA distributed nearly 200,000 doses of the Qdenga (TAK-003) vaccine to seven priority regions for adolescents aged 10–20 (8 Aug), part of El Niño-season preparedness. [RPP Noticias, 18 Aug](https://rpp.pe/peru/actualidad/dengue-sube-41-en-peru-regiones-enfrentan-problemas-para-asegurar-medicamentos-noticia-1701328) · [La República, 8 Aug](https://larepublica.pe/sociedad/2026/08/08/minsa-refuerza-vacunacion-contra-el-dengue-con-casi-200000-dosis-enviadas-a-siete-regiones-del-peru-762832)

### Colombia (Category B — monthly ratio: running well below → running slightly below; Category C — current-season percentile 23.8 → 27.6)
- GDO figures: 6,885 reported cases (latest observed month 2026-07-01, ~1.8 months stale). Cumulative percentile 57.3 (Normal). Estimated total seasonal cases: 104,587.
- News: worth flagging a tension between GDO's easing monthly-ratio reading and the national picture — Colombia's Instituto Nacional de Salud (INS), in its epidemiological week 31 bulletin (~mid-Aug; exact publication date unconfirmed), classified the national dengue situation as an outbreak ("brote") against its endemic-channel threshold, reporting 68,370 cumulative 2026 cases and 41 confirmed deaths, concentrated in Meta, Amazonas, Magdalena, Guaviare, Casanare, Arauca and Bolívar. [La FM, citing INS](https://www.lafm.com.co/sociedad/dengue-piocaduras-zancudos-mosquitos-colombia-muertes-afectados-408539) · [Consultorsalud, citing INS](https://consultorsalud.com/dengue-colombia-semana-26-2026-ins/)

### Brazil (Category B — monthly ratio: running well below → running slightly above)
- GDO figures: 68,345 reported cases (latest observed month 2026-07-01, ~1.8 months stale). Cumulative percentile 49.5 (Normal); current-season percentile effectively zero (Extremely Low) — a large gap between the monthly and seasonal reads. Estimated total seasonal cases: 1,657,363 (a very large projection off a huge baseline — treat as indicative, not precise).
- News: no dengue-specific item confirmed within the last ~2 weeks. Background: Brazil's Ministério da Saúde reported a 75% year-on-year drop in probable cases for Jan–Apr 2026 (227,500 vs. 916,400), attributed to the Butantan single-dose vaccine rollout, Wolbachia releases and expanded ovitrap surveillance. A Mato Grosso do Sul state bulletin dated 2026-08-10 sits at the very edge of the search window but could not be independently date-confirmed.

### India (Category B — monthly ratio: running slightly above → tracking near)
- GDO figures: 10,122 reported cases (latest observed month 2026-07-01, ~1.8 months stale). Cumulative percentile 60.9 (Normal); current-season percentile 6.9 (Low). Estimated total seasonal cases: 132,230.
- News: monsoon-driven case rises reported in both Mumbai (rising OPD consultations for dengue/malaria as rains create breeding sites, 12 Aug) and Delhi-NCR (concurrent rise in dengue, swine flu and H3N2 described as a "triple viral threat", 21 Aug); separate Delhi coverage put the city at 1,379 season cases so far, with doctors warning the true peak (Aug–Oct) is still ahead. [The Week, 12 Aug](https://www.theweek.in/news/health/2026/08/12/dengue-malaria-mumbai-monsoon.html) · [NewsX, 21 Aug](https://www.newsx.com/health/delhis-dengue-peak-is-yet-to-come-why-august-october-could-be-crucial-262833/)

### Barbados (Category A — severity interpretation: Rare good event → Below average; Category C — current-season percentile 1.6 → 5.9)
- GDO figures: 14 reported cases (latest observed month 2026-06-01, ~2.8 months stale — beyond the sweet spot). Both cumulative (21.1) and current-season (5.9) percentiles remain Low/Extremely Low despite the uptick. Estimated total seasonal cases: 176.
- News: no dengue-specific item confirmed within the last ~2 weeks. Background: a Nation News piece (10 July) on illegal dumping creating mosquito-breeding risk mentioned dengue only in passing; PAHO maintains a general (undated) Eastern Caribbean dengue prevention programme page.

### Paraguay (Category A — severity interpretation: Below average → Average)
- GDO figures: 256 reported cases (latest observed month 2026-07-01, ~1.8 months stale). Cumulative percentile 25.6 (Low); current-season percentile 1.1 (Extremely Low). Estimated total seasonal cases: 6,565.
- News: no item confirmed within the last ~2 weeks. Background: Paraguay's DGVS (health surveillance directorate) weekly bulletins through mid-July showed a stable/declining curve (288 cumulative 2026 cases), DENV-1 predominant with a DENV-3 reintroduction from Brazil confirmed in April; local press (ABC Color, 23 May) flagged low vaccination uptake (4,056 of 70,200 stocked doses administered).

### Antigua and Barbuda (Category B — monthly ratio: running well below → running slightly below; Category C — current-season percentile 10.7 → 16.4)
- GDO figures: 7 reported cases (latest observed month 2026-06-01, ~2.8 months stale — beyond the sweet spot; a small case count makes this figure more sensitive to noise than most). Cumulative percentile 42.4 (Normal); current-season percentile 16.4 (Low). Estimated total seasonal cases: 74.
- News: no item confirmed within the last ~2 weeks. Background: the Health Minister publicly denied an outbreak in mid-January, citing a declining multi-year trend (2 cases in 2022 to 11 in 2025); the Central Board of Health ran a "Mosquito Awareness Week" source-reduction campaign 18–22 May.

## 4. News — general scan (3 items)

Independent broad scan; capped at 5, but only three distinct items — beyond the ten targeted countries above — could be confirmed within the ~2-week window. Two of the three are explicitly non-endemic/no-GDO-data settings, per the routine's instruction to surface that geography.

1. **France (Nouvelle-Aquitaine), 2026-08-19–21** — Santé publique France's regional arbovirus bulletin confirmed a locally-acquired dengue case in Dordogne (Mouleydier) alongside expanding local chikungunya clusters in Gironde, attributed to tiger-mosquito spread amid warming conditions. Non-endemic, no GDO nowcast coverage. [Santé publique France, 19 Aug](https://www.santepubliquefrance.fr/regions-et-territoires/nouvelle-aquitaine/bulletin-regional/chikungunya-dengue-et-zika-en-nouvelle-aquitaine-bulletin-du-19-aout-2026) · [The Local France, 21 Aug](https://www.thelocal.fr/20260821/chikungunya-and-dengue-fever-reported-in-south-west-france)
2. **United States (Florida, Citrus County), 2026-08-22** — Florida DOH-Citrus County confirmed the county's first-ever locally-acquired dengue case (no travel history), prompting increased truck fogging, aerial larviciding and ground inspections; follows earlier August local cases in Hillsborough, Miami-Dade and Palm Beach counties. Non-endemic, no GDO nowcast coverage. [WFLA, 22 Aug](https://www.wfla.com/news/local-news/citrus-county/citrus-county-confirms-first-case-of-locally-acquired-dengue-fever/)
3. **Bangladesh, 2026-08-23** — 839 new cases and 5 deaths reported in a single 24-hour period, bringing 2026 totals to 28,929 cases and 82 deaths; Khulna and Dhaka divisions currently most affected. Bangladesh is not among this week's ten GDO-targeted countries. [The Business Standard, 23 Aug](https://www.tbsnews.net/bangladesh/730-new-dengue-cases-two-deaths-reported-24hrs-1515701)

## 5. Trend since last update

First genuine week-over-week comparison (the prior pull, 2026-08-12, was itself GDO's first-ever pull, so it had nothing to diff against). 21 mover rows this week: 4 Category A, 7 Category B, 10 Category C.

**Category A — severity-band interpretation changes (4):**
- Sri Lanka: Above average → **Rare bad event** (now Extremely High cumulative)
- Panama: Average → Above average (now High)
- Paraguay: Below average → Average (now Normal)
- Barbados: Rare good event → Below average (still Low)

**Category B — monthly-ratio descriptor changes (7):**
- Peru: running well below → **running well above**
- Guyana: running well above → **running well below**
- Brazil: running well below → running slightly above
- Colombia: running well below → running slightly below
- Panama: running well below → running slightly below
- Antigua and Barbuda: running well below → running slightly below
- India: running slightly above → tracking near

**Category C — current-season percentile shifts (10, largest first):**

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

1. **Sri Lanka — largest outbreak since 2017, GDO's biggest percentile jump corroborated by WHO and rising death toll.** Current-season percentile leapt from 37.7 to 82.2 in one week, cumulative severity crossed into Extremely High, and this is independently confirmed by a WHO-convened national review and local wire reports of the death toll rising from 68 to 69 alongside 92,854 cumulative cases. Strong, well-corroborated story. *Caveat: GDO's underlying data point is ~1.8 months old — near the healthy end of the sweet spot, not stale, but not real-time either.*
2. **Peru — sharpest reversal in this week's data, paired with a concrete medicine-shortage angle.** GDO's monthly ratio flipped from "well below" to "well above," and MINSA independently reports a 41% year-on-year case rise alongside budget/medicine-supply strain — a relatable, human angle beyond raw numbers. Pairs naturally with the Qdenga vaccine-distribution news for a "response in motion" framing. *Caveat: MINSA's case/death figures are national totals, not GDO's nowcast — don't conflate the two sources when drafting.*
3. **Colombia — a "the numbers disagree" story worth careful framing.** GDO's monthly ratio is easing ("well below" → "slightly below"), yet Colombia's own national institute (INS) has classified the situation as an outbreak against its endemic-channel threshold. Good opportunity to explain that GDO's *monthly* trend and a *cumulative* outbreak classification can diverge — useful audience education, not a contradiction. *Caveat: exact INS bulletin publication date could not be confirmed — verify before quoting a precise date.*
4. **Panama — concrete, dated ministry figures with a child-health hook.** Panama's own Minsa reports 16 deaths and disproportionate impact on 10–14-year-olds (167 per 100,000), alongside GDO's own band-crossing into "High." Citable, specific, human-interest angle. *No major caveat — data points align well.*
5. **Continued non-endemic local transmission (France, Florida).** A locally-acquired case in a new French département and Florida's first-ever locally-acquired case in Citrus County, in the same window, echo the "dengue's reach is expanding" theme flagged in prior weeks. *Caveat: small absolute case numbers in each location — frame as an emerging-geography story, not an outbreak-scale one.*

## 7. Scientific literature findings

Lighter-effort pass; a handful of recent items across forecasting, climate drivers, surveillance and vaccine policy.

- **Forecasting/nowcasting:** Probabilistic dengue forecasting and early-warning system across Mexican states (1985–2026), combining machine learning and statistical ensembles with conformal calibration; reports a median error of ~21 cases per state per month at a 3-month horizon during the current DENV-3 resurgence. *Research Square preprint*, 2026. [Research Square](https://www.researchsquare.com/article/rs-10035640/v1)
- **Forecasting/nowcasting:** M-SDT, a modelling framework combining transmission dynamics, forecasting and intervention-strategy simulation for dengue in Ahmedabad Municipal Corporation, India. *arXiv preprint*, ~May 2026. [arXiv](https://arxiv.org/pdf/2605.17975)
- **Climate drivers:** Semi-mechanistic modelling study projecting expanded dengue transmission-suitable months and regions in California under continued climate warming — relevant given the state's first locally-acquired cases in recent years. *The Lancet Regional Health – Americas*, 2026. [The Lancet](https://www.thelancet.com/journals/lanam/article/PIIS2667-193X(26)00139-0/fulltext)
- **Surveillance methods:** E-Dengue, a predictive surveillance tool deployed across selected Mekong Delta (Vietnam) districts from early 2026, feeding real public-health decisions during 2026–2028 alongside a randomised evaluation. Science-news coverage, *The Microbiologist*, 2026. [The Microbiologist](https://www.the-microbiologist.com/news/global-study-to-evaluate-whether-dengue-outbreaks-can-be-anticipated-earlier/7638.article)
- **Surveillance methods:** Peer-reviewed modelling study estimating wastewater detection limits for dengue virus, based on urinary/faecal shedding in symptomatic vs. asymptomatic infections. *ScienceDirect*, 2026. [ScienceDirect](https://www.sciencedirect.com/science/article/pii/S2589914726000654)
- **Vaccine policy:** Brazil's Ministry of Health suspended its Butantan-DV single-dose dengue vaccine pilot (~500,000 doses administered) on 8 June 2026, following two deaths and roughly 42 serious adverse-event reports, pending investigation; described as precautionary, with no confirmed causal link established. *The Lancet* and other outlets, June 2026. [The Lancet](https://www.thelancet.com/journals/lancet/article/PIIS0140-6736(26)01239-0/abstract)
- **Vaccine policy:** A US "Gold Standard Childhood Vaccine Recommendations" presidential action (10 August 2026) names dengue vaccination for high-risk groups; separately, CDC guidance notes remaining Dengvaxia stock (expiring August 2026) should only be used to complete existing series, not to start new ones. [White House, 10 Aug](https://www.whitehouse.gov/presidential-actions/2026/08/delivering-gold-standard-childhood-vaccine-recommendations-for-americans/) · [CDC](https://www.cdc.gov/dengue/hcp/vaccine/index.html)

## 8. Appendix

### 8.1 `movers.csv` (active snapshot)

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

1. WHO Sri Lanka, National Dengue Review 2026 (14 Aug) — https://www.who.int/srilanka/news/detail/14-08-2026-national-dengue-review-2026-identifies-priorities-to-strengthen-sri-lanka-s-dengue-preparedness-and-response
2. Newswire, Sri Lanka death toll rises to 69 (19 Aug) — https://www.newswire.lk/2026/08/19/sri-lankas-dengue-death-toll-rises-to-69/
3. Newswire, Sri Lanka cases top 90,000 (11 Aug) — https://www.newswire.lk/2026/08/11/sri-lanka-dengue-cases-top-90000-in-2026/
4. ReliefWeb/IFRC, Sri Lanka DREF Operation — https://reliefweb.int/report/sri-lanka/sri-lanka-dengue-outbreak-2026-dref-operation-mdrlk024
5. Prensa Latina, Panama case/death figures (17 Aug) — https://www.plenglish.com/news/2026/08/17/panama-records-over-5000-dengue-cases-children-make-up-the-majority/
6. Ministerio de Salud de Panamá, dengue dashboard — https://www.minsa.gob.pa/informacion-salud/dengue-2026
7. RPP Noticias, Peru case rise/medicine shortage (18 Aug) — https://rpp.pe/peru/actualidad/dengue-sube-41-en-peru-regiones-enfrentan-problemas-para-asegurar-medicamentos-noticia-1701328
8. La República, Peru Qdenga vaccine distribution (8 Aug) — https://larepublica.pe/sociedad/2026/08/08/minsa-refuerza-vacunacion-contra-el-dengue-con-casi-200000-dosis-enviadas-a-siete-regiones-del-peru-762832
9. La FM Colombia, citing INS week 31 (mid-Aug) — https://www.lafm.com.co/sociedad/dengue-piocaduras-zancudos-mosquitos-colombia-muertes-afectados-408539
10. Consultorsalud, citing INS Colombia — https://consultorsalud.com/dengue-colombia-semana-26-2026-ins/
11. The Week, Mumbai monsoon dengue rise (12 Aug) — https://www.theweek.in/news/health/2026/08/12/dengue-malaria-mumbai-monsoon.html
12. NewsX, Delhi dengue peak yet to come (21 Aug) — https://www.newsx.com/health/delhis-dengue-peak-is-yet-to-come-why-august-october-could-be-crucial-262833/
13. Santé publique France, Nouvelle-Aquitaine arbovirus bulletin (19 Aug) — https://www.santepubliquefrance.fr/regions-et-territoires/nouvelle-aquitaine/bulletin-regional/chikungunya-dengue-et-zika-en-nouvelle-aquitaine-bulletin-du-19-aout-2026
14. The Local France, chikungunya/dengue in south-west France (21 Aug) — https://www.thelocal.fr/20260821/chikungunya-and-dengue-fever-reported-in-south-west-france
15. WFLA, Citrus County first local case (22 Aug) — https://www.wfla.com/news/local-news/citrus-county/citrus-county-confirms-first-case-of-locally-acquired-dengue-fever/
16. The Business Standard, Bangladesh 24-hour case/death update (23 Aug) — https://www.tbsnews.net/bangladesh/730-new-dengue-cases-two-deaths-reported-24hrs-1515701
17. Research Square, Mexico probabilistic forecasting preprint (2026) — https://www.researchsquare.com/article/rs-10035640/v1
18. arXiv, M-SDT modelling framework (~2026-05) — https://arxiv.org/pdf/2605.17975
19. The Lancet Regional Health – Americas, California climate suitability study (2026) — https://www.thelancet.com/journals/lanam/article/PIIS2667-193X(26)00139-0/fulltext
20. The Microbiologist, E-Dengue Mekong Delta surveillance tool (2026) — https://www.the-microbiologist.com/news/global-study-to-evaluate-whether-dengue-outbreaks-can-be-anticipated-earlier/7638.article
21. ScienceDirect, wastewater dengue detection-limit study (2026) — https://www.sciencedirect.com/science/article/pii/S2589914726000654
22. The Lancet, Butantan-DV vaccine suspension (June 2026) — https://www.thelancet.com/journals/lancet/article/PIIS0140-6736(26)01239-0/abstract
23. White House, Gold Standard Childhood Vaccine Recommendations (10 Aug) — https://www.whitehouse.gov/presidential-actions/2026/08/delivering-gold-standard-childhood-vaccine-recommendations-for-americans/
24. CDC, Dengvaxia remaining-stock guidance — https://www.cdc.gov/dengue/hcp/vaccine/index.html
