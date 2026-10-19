# GDO Internal News Report — 2026-10-19

**Source:** Global Dengue Observatory (accessed 2026-10-19)
**Snapshot:** `snapshots/2026_10_19/` — fetched from `Output/2026_10_18/` (target render date 2026-10-18), source commit `67e82815d1cd625144c4021f338992c0ba6a31ee`, no fallback used.
**Countries covered:** 85

This is a **pull week**: the public site's render date advanced from 2026-10-04 (last pull, 2026-10-05) to 2026-10-18, so the nowcast snapshot and movers table below are freshly fetched rather than reused.

---

## 1. This week's snapshot

Across the 85 countries in the current nowcast, the cumulative-season severity picture is:

| Severity (cumulative) | Countries |
|---|---|
| Extremely High | 9 |
| High | 14 |
| Normal | 28 |
| Low | 23 |
| Extremely Low | 5 |
| Unknown | 6 |

The nine **Extremely High** (cumulative percentile ≥95) countries are Cook Islands, Cuba, Guyana, Kenya, Cambodia, Sri Lanka, Maldives, Peru and Timor-Leste. On the narrower **current-season** measure (which strips out longer-running cumulative load and looks only at the active season), just three stay Extremely High: Cuba, Kenya and Cambodia — a reminder that cumulative and current-season severity tell different stories and shouldn't be conflated.

Regionally, the Caribbean and South America carry the heaviest current load (Caribbean: 1 Extremely High, 0 High, 8 Low/Normal split; South America: 2 Extremely High, 2 High), with South Asia and East & Southeast Asia also showing concentrated High/Extremely High activity (Sri Lanka, Maldives; Cambodia, China).

**Caveat:** `latest_observed_date` varies by country across this snapshot (spanning July–September 2026 for the countries highlighted below), reflecting GDO's standard 1–2 month nowcast gap-fill. Figures from the shorter end of that window are the most reliable; any number flagged below as resting on a longer gap or a small baseline should be read with proportionate caution.

---

## 2. News — targeted (movers)

**Selection note:** `movers.csv` flagged 16 unique countries across category A (severity-band crossings) and category B (monthly-ratio-descriptor crossings) this week — more than the 10-country cap — plus 9 additional category-C percentile movers. Per the agent instructions, A/B band-crossings were prioritised over C entirely. All 9 category-A countries are covered below; the 10th slot went to Brazil (category B), whose swing from "running well below" to "running well above" was the largest and most newsworthy of the remaining B-only movers.

### China (CHN) — category A
Severity interpretation moved from "Cannot determine" to **"Above average – more cases than typical at this point"** (percentile 81.4, cumulative). Note this sits alongside a category-B move in the *opposite* direction (monthly ratio descriptor: "running well above" → "running slightly below"), i.e. the most recent month eased even as the season-to-date position firmed up as "above average" — a sign of slowing rather than accelerating transmission.
Recent coverage is thin for October specifically: Chinese CDC reporting in May 2026 noted local outbreaks fell sharply in 2025 even as imported cases rose, and a Chinese CDC seasonality study (2005–2023) puts the typical local-transmission window at June–November, peaking September/October — consistent with, but not confirming, current activity.
*Source: [China CDC Weekly](https://weekly.chinacdc.cn/en/article/pdf/preview/10.46234/ccdcw2024.217) (background); no dated October 2026 outbreak report found — treat as a reporting gap, not an all-clear.*

### French Guiana (GUF) — category A
Moved from "Rare good event – unusually low cases to date" to **"Below average – fewer cases than typical at this point"** — i.e. still mild, just slightly less unusually quiet. Santé publique France's regional bulletin (21 August 2026) recorded only 12 laboratory-confirmed dengue cases since the start of the year. The bigger local arbovirus story is chikungunya, with 1,604 confirmed cases and active epidemic transmission on the West Coast and in the Savanes sector as of the same bulletin — worth flagging for context even though it isn't a GDO-tracked number.
*Source: [Santé publique France, French Guiana bulletin, 21 August 2026](https://www.santepubliquefrance.fr/en/regions-and-territories/french-guiana/regional-bulletin/chikungunya-and-dengue-french-guiana-bulletin-dated-august-21-2026).*

### Honduras (HND) — category A
Moved from "Average – typical case load at this point" to **"Below average – fewer cases than typical at this point."** This tracks with national reporting: cumulative 2026 cases (~5,780 by early July) are running roughly half of 2025's total, per El Heraldo, with Cortés and Francisco Morazán departments carrying the heaviest suspected-case load and under-15s the most affected group. No national figures newer than July 2026 were found, so the "below average" read is consistent with the trend but not confirmed into October.
*Source: [El Heraldo, 8 July 2026](https://www.elheraldo.hn/honduras/honduras-registra-2026-acumulado-5-780-casos-dengue-CB31477746).*

### Jamaica (JAM) — category A
Moved from "Average – typical case load at this point" to **"Below average – fewer cases than typical at this point."** No reliable 2026-dated Jamaican reporting turned up — most search results trace back to Jamaica's 2023 outbreak (serotype DENV-2 dominant) rather than current activity, so this is a case where the nowcast is the only live signal; worth a direct check of the Ministry of Health and Wellness or PAHO's arbo-portal before using in a social post.
*Source: no current (2026) news corroboration found; GDO nowcast only.*

### Mexico (MEX) — category A
Moved from "Below average – fewer cases than typical at this point" to **"Average – typical case load at this point."** National figures to mid-August 2026 show 4,152 confirmed cases (2,237 with warning signs/severe dengue, 7 confirmed deaths), with Sonora, Veracruz, Tabasco, Sinaloa and Quintana Roo accounting for 72% of cases. Separately, Mexico's health authorities added a tetravalent dengue vaccine to the national compendium on 19 August 2026, indicated only for ages 10–14 without comorbidities — a policy move, not yet a rollout.
*Source: [Excélsior, 17 August 2026](https://www.excelsior.com.mx/nacional/dengue-mexico-2026).*

### Mauritania (MRT) — category A
Moved from "Below average – fewer cases than typical at this point" to **"Average – typical case load at this point."** The most recent dated figures found are from UK TravelHealthPro (3 December 2025): 7,280 cases (4,050 confirmed), one death, across 13 of 15 regions since an outbreak that began in May 2025. No 2026 update was found, so this move is **not independently corroborated** by current news — flag as nowcast-only if used externally.
*Source: [TravelHealthPro, 3 December 2025](https://travelhealthpro.org.uk/updates.php?base=4999) — outdated relative to this snapshot; use with caution.*

### Peru (PER) — category A (also category C)
Moved from "Above average" to **"Rare bad event – unusually high cases to date"** (cumulative percentile 97.9 — Extremely High), and current-season percentile jumped from 19.9 to 49.1. Peru's MINSA reported 46,669 cases through epidemiological week 33 (up ~53% on 2025) and 57 confirmed dengue deaths as of 22 August, with Piura the hardest-hit region. Officials attribute the rise to high temperatures and are extending the vaccination strategy to 10–16-year-olds. **Caveat:** cited YoY growth figures vary by outlet (53%, 79%, 22%, 31%) depending on cutoff date — treat the direction, not the precise magnitude, as the reliable signal, and note the ~2-month gap between these MINSA figures and this report.
*Source: [Exitosa Noticias, 22 August 2026](https://www.exitosanoticias.pe/actualidad/peru-supera-ocho-meses-2026-record-fallecidos-dengue-todo-2025-n182564); [Canal N](https://canaln.pe/actualidad/casos-dengue-aumentan-79-peru-minsa-advierte-que-podrian-incrementarse-altas-temperaturas-n495247).*

### Sudan (SDN) — category A
Moved from "Rare bad event – unusually high cases to date" to **"Above average – more cases than typical at this point"** — an improvement in relative terms, though the country remains High severity overall (percentile 78.5). This masks a serious humanitarian picture: the Blue Nile outbreak (reported late July 2026) was linked to 39 deaths and 300+ cases by the Sudan Doctors Union, compounding earlier Khartoum/Omdurman transmission (211 new cases, 39 deaths reported in January). WHO's August 2026 update lists dengue alongside cholera, malaria and measles as active Sudan outbreaks, with its emergency appeal only 19.3% funded. **Caveat:** conflict-disrupted surveillance in Sudan means small-baseline/large-swing risk is high here — treat precise percentile moves cautiously even as the broader "serious and under-resourced" story holds.
*Source: [WHO EMRO, Sudan Health Spotlight, August 2026](https://www.emro.who.int/images/stories/sudan/Sudan-Health-Spotlight-August-2026.pdf); [Sudan Tribune](https://sudantribune.com/?p=311068).*

### United States (USA) — category A (also category C)
Moved from "Average" to **"Above average – more cases than typical at this point"** (cumulative percentile 94.5); current-season percentile also rose (52.4→58.5). This sits against a striking subnational story: Florida's Department of Health describes its 2026 season (296 locally-acquired cases through the week of 27 September–3 October) as the state's most significant dengue outbreak since the 1930s, with Hillsborough, Pasco and Pinellas counties declaring local states of emergency and Orange County beginning aerial mosquito spraying on 16 October. **Caveat:** CDC's own national weekly table (week ending 3 October) put 2026 cases at 801 nationally, actually *down* from 1,088 at the same point in 2025 — the GDO "above average" nowcast and the raw national YTD count point in different directions, which is itself worth flagging rather than resolving in this report; the real story may be concentration (Florida) rather than national volume.
*Source: [mysuncoast.com, 24 September 2026](https://www.mysuncoast.com/2026/09/24/florida-reports-392-dengue-cases-2026-cdc-data-show/); [CDC weekly arbonet tables](https://stacks.cdc.gov/view/cdc/262201/cdc_262201_DS1.pdf).*

### Brazil (BRA) — category B
Monthly ratio descriptor swung from "running well below" to **"running well above"** — the largest B-category move this week, which is why it was selected as the tenth targeted country ahead of other category-C-only movers. PAHO has declared a Grade 3 (highest level) multi-country emergency for the Americas; Brazil accounts for roughly 811,000 of the region's ~1.1 million suspected cases through epidemiological week 20, and is currently the only country with all four dengue serotypes co-circulating — a genuine severity signal, not just a nowcast artefact. **Caveat:** the 2026 regional total is running ~64% *below* 2025 (itself a record year), so "running well above" reflects a jump against a normal seasonal baseline, not a return to 2025's extremes.
*Source: [PAHO/PLISA regional update](https://www.mappr.co/dengue-outbreak-map/); [outbreaknewstoday.substack.com](https://outbreaknewstoday.substack.com/p/brazil-mato-grosso-do-sul-reports).*

---

## 3. News — general scan

1. **Cuba** — Extremely High on both cumulative and (implicitly, via persistently elevated figures) current-season measures in this snapshot. News corroborates: 11,235 cases reported for 2026, with September alone reaching 4,102 — the highest monthly count of the year to date. *(Outbreak News Today, citing Global Dengue Observatory figures.)*
2. **Sri Lanka** — case counts climbed sharply from 25,082 in early May to roughly 92,854 by 18 August 2026, with officials linking the surge to heavy rain and flooding. Matches GDO's Extremely High cumulative severity classification for Sri Lanka this snapshot. *(Outbreak News Today.)*
3. **Maldives-linked imported dengue in Europe** — a genuinely non-endemic/no-GDO-data angle: at least 46 imported cases linked to Maldives travel were reported across four EU/EEA countries in 2026; Spain separately reported 114 cases with known exposure location through mid-August, 46% imported from the Maldives and a further 10 from Cuba. ECDC assesses onward local-transmission risk in continental Europe as currently low given unfavourable mosquito conditions. *(ECDC Communicable Disease Threats Report; Spanish Ministry of Health Aedes-borne disease surveillance report, 17 August 2026.)*
4. **Marshall Islands** — 112 confirmed dengue cases (DENV-1) reported as of late September 2026, a Pacific outbreak with no equivalent GDO country entry in this snapshot's targeted list. *(Outbreak News Today.)*
5. **PAHO regional emergency declaration** — PAHO's Grade 3 emergency designation for the Americas (see Brazil entry above) is itself a regional policy/news item distinct from any single country's numbers: ~1.1 million suspected cases across 44 reporting countries/territories through week 20, ~27% laboratory-confirmed. *(PAHO/PLISA.)*

---

## 4. Trend since last update

*Snapshot-to-snapshot comparison: `snapshots/2026_10_19/` vs. prior snapshot `snapshots/2026_10_05/`.*

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

**Category C — current-season percentile movers:** 9 countries flagged (largest absolute moves: Peru +29.2 pts, Australia −46.3 pts, Sudan −11.3 pts). Full list in Appendix.

---

## 5. Social-media candidate flags

Ranked shortlist — strongest, most defensible stories for Tuesday's social drafts:

1. **Peru** — clean, strong signal: category A *and* C crossing in the same direction (both cumulative and current-season percentiles rising), corroborated by MINSA case/death figures and an explicit ministry statement anticipating further rises. *Caveat: cite the direction of change, not a single precise growth percentage — sources disagree on magnitude.*
2. **Brazil** — PAHO's Grade 3 regional emergency plus all-four-serotypes co-circulation is a strong, verifiable hook. *Caveat: frame as "up on a normal season," not "up on 2025" — 2026 remains well below last year's record regionally.*
3. **Sudan** — humanitarian and funding-gap angle (WHO appeal 19.3% funded) alongside Blue Nile mortality figures is compelling. *Caveat: conflict-affected surveillance makes exact figures unstable; lead with the funding/response gap rather than precise case counts.*
4. **Florida (USA)** — "most significant outbreak since the 1930s," multiple county emergency declarations, is a vivid, highly shareable story. *Caveat: national CDC YTD total is actually down year-on-year — be explicit that this is a Florida/subnational story, not a US-wide trend, to avoid an easily-checked inconsistency.*
5. **Cuba** — Extremely High on both severity measures, with a clean news match (record September case count). *Caveat: this is a persistently severe country rather than a week-over-week mover, so frame as "still/further elevated," not as new news.*

---

## 6. Scientific literature findings

- **Forecasting (Singapore):** Finch, Lowe and colleagues (with Singapore's National Environment Agency) built a model combining >20 years of climate data with circulating-serotype surveillance to forecast outbreak risk up to two months ahead; the same group estimates expanded Wolbachia releases averted ~28% of expected 2023 cases. [BioSpectrum Asia](https://www.biospectrumasia.com/news/30/27364/singapore-researchers-combines-climate-and-virus-surveillance-to-predict-dengue-outbreak-risk-two-months-in-advance.html)
- **Forecasting (Brazil):** The Barcelona Supercomputing Center's GHRmodel (Bayesian spatiotemporal, using temperature/precipitation/drought indicators) was among the strongest performers in the InfoDengue–Mosqlimate forecasting challenge; the challenge's headline finding was that no single model wins consistently across regions/seasons, favouring ensemble approaches — which Brazilian health authorities have since adopted. [BSC](https://ess.bsc.es/news/new-models-improve-dengue-forecasting-in-brazil-amid-unprecedented-outbreaks)
- **Climate projections (Costa Rica):** a district-level study linking high-resolution precipitation/temperature data to dengue diagnoses, projecting mid-century (2035–2065) incidence under SSP5-8.5 using eight global climate models. [CONARE repository record](https://kimuk.conare.ac.cr/Record/KUCR_6c7394750d9df8a919bb94891c9f9df2)
- **Surveillance (Vietnam):** an AI-based early-warning system incorporating rainfall, temperature, humidity and population density is being piloted across districts in the Mekong Delta in early 2026 (reported in general news coverage; primary publication not located).
- **Vaccine policy:** India's drug regulator (CDSCO) approved Qdenga for ages 4–60 (private market, not yet in the national immunisation programme) as of 21 July 2026. Brazil's Anvisa approved the single-dose Butantan-DV vaccine for ages 12–59 in November 2025, with the health ministry planning to add it to the national immunisation programme (PNI) — no confirmed rollout start date found yet.

---

## 7. Appendix

### Full movers table (`snapshots/2026_10_19/movers.csv`)

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

### Consolidated citation list

- El Heraldo (Honduras): https://www.elheraldo.hn/honduras/honduras-registra-2026-acumulado-5-780-casos-dengue-CB31477746
- La Prensa (Honduras): https://www.laprensa.hn/honduras/dengue-honduras-2026-cortes-francisco-morazan-concentran-mas-casos-HG31042995
- Excélsior (Mexico): https://www.excelsior.com.mx/nacional/dengue-mexico-2026
- Riviera Maya News (Quintana Roo, Mexico): https://www.rivieramayanews.mx/quintana-roo-reports-8-new-dengue-cases-as-2026-total-hits-167/
- Santé publique France, French Guiana bulletin (21 August 2026): https://www.santepubliquefrance.fr/en/regions-and-territories/french-guiana/regional-bulletin/chikungunya-and-dengue-french-guiana-bulletin-dated-august-21-2026
- Santé publique France, mainland France Aedes-borne surveillance bulletin: https://www.santepubliquefrance.fr/en/vector-borne-diseases/chikungunya/national-bulletin/chikungunya-dengue-zika-and-west-nile-virus-mainland-france-enhanced-surveillance-bulletin-july-29
- TravelHealthPro, Mauritania (3 December 2025): https://travelhealthpro.org.uk/updates.php?base=4999
- Exitosa Noticias (Peru): https://www.exitosanoticias.pe/actualidad/peru-supera-ocho-meses-2026-record-fallecidos-dengue-todo-2025-n182564
- Canal N (Peru): https://canaln.pe/actualidad/casos-dengue-aumentan-79-peru-minsa-advierte-que-podrian-incrementarse-altas-temperaturas-n495247
- WHO EMRO, Sudan Health Spotlight (August 2026): https://www.emro.who.int/images/stories/sudan/Sudan-Health-Spotlight-August-2026.pdf
- Sudan Tribune: https://sudantribune.com/?p=311068
- EpiNews/EMPHNET (Sudan, Northern State): https://epinews.emphnet.net/en/news/dengue-fever-cases-rise-to-80-in-sudans-northern-state
- mysuncoast.com (Florida, USA): https://www.mysuncoast.com/2026/09/24/florida-reports-392-dengue-cases-2026-cdc-data-show/
- CDC ArboNET weekly tables: https://stacks.cdc.gov/view/cdc/262201/cdc_262201_DS1.pdf
- PAHO/PLISA regional dengue map summary: https://www.mappr.co/dengue-outbreak-map/
- Outbreak News Today (Brazil, Mato Grosso do Sul): https://outbreaknewstoday.substack.com/p/brazil-mato-grosso-do-sul-reports
- Outbreak News Today (Cuba, Sri Lanka, Marshall Islands — general scan items)
- ECDC Communicable Disease Threats Report, week 13 2026: https://www.ecdc.europa.eu/sites/default/files/documents/Communicable-disease-threats-report-week-13-2026.pdf
- Spanish Ministry of Health, Aedes-borne disease surveillance report (17 August 2026): https://www.sanidad.gob.es/fr/areas/alertasEmergenciasSanitarias/preparacionRespuesta/docs/20260817_Informe_seguimineto_Enf_transmitidas_Aedes_2026.pdf
- BioSpectrum Asia (Singapore forecasting model): https://www.biospectrumasia.com/news/30/27364/singapore-researchers-combines-climate-and-virus-surveillance-to-predict-dengue-outbreak-risk-two-months-in-advance.html
- Barcelona Supercomputing Center (Brazil forecasting ensemble): https://ess.bsc.es/news/new-models-improve-dengue-forecasting-in-brazil-amid-unprecedented-outbreaks
- CONARE repository (Costa Rica climate projection): https://kimuk.conare.ac.cr/Record/KUCR_6c7394750d9df8a919bb94891c9f9df2
- The Policy Edge (India, Qdenga approval): https://www.policyedge.in/p/cdsco-approves-indias-first-dengue-vaccine-individuals-aged-460-years
- ictq.com.br (Brazil, Butantan-DV vaccine/PNI plans): https://ictq.com.br/farmacia-clinica/4240-governo-anuncia-vacina-brasileira-contra-dengue-no-sus-a-partir-de-2026
