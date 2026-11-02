# GDO Internal News Report — 2026-11-02

*Source: Global Dengue Observatory (accessed 2026-11-02).*

## 1. Header

- **Report date:** 2026-11-02 (Monday routine run).
- **Active snapshot:** `snapshots/2026_10_19/` — **unchanged since 2026-10-19** (third consecutive news-only week; no new pull this run). Source data vintage (`target_render_date`): 2026-10-18. Source commit `67e82815d1cd625144c4021f338992c0ba6a31ee` (`DENV_global_observatory` `Output/2026_10_18/`, no fallback used). Prior snapshot: `snapshots/2026_10_05/` (vintage 2026-10-04).
- **Pull status this week:** **news-only week.** `target_render_date` for this run computes to 2026-10-18 (most recent of {this month's 4th = 2026-11-04, this month's 18th = 2026-11-18, last month's 18th = 2026-10-18} that is strictly before today, 2026-11-02 — the first two aren't due yet, so only 2026-10-18 qualifies). That matches the vintage already recorded in `snapshots/2026_10_19/manifest.json` — no new render has happened on the public site since the last pull, so Step 1's fetch/diff was skipped per Step 0.5, and this run reuses `snapshots/2026_10_19/` (including its `movers.csv`, a 2026-10-05 → 2026-10-19 comparison) as the active snapshot.
- **Countries covered:** 85.
- **Environment note:** this session's container had no R runtime pre-installed. Per the routine's Step 0 fallback, `apt-get update && apt-get install -y --no-install-recommends r-base-core` was run as a single attempt and succeeded (R 4.3.3). The subsequent `install.packages()` call for `httr`/`jsonlite`/`dplyr`/`readr`/`tibble`/`stringr`/`lubridate` failed — CRAN (`cloud.r-project.org`) is blocked by this sandbox's egress proxy (403 "policy denial" on the CONNECT tunnel, confirmed via the proxy status endpoint). Rather than retrying the same install in a loop, this run used the equivalent Ubuntu-packaged route instead (`apt-get install r-cran-httr r-cran-jsonlite r-cran-dplyr r-cran-readr r-cran-tibble r-cran-stringr r-cran-lubridate`), which succeeded cleanly and loads without error. This wasn't otherwise load-bearing this run, since Step 1 (the R pipeline) is skipped on a news-only week. `gh` CLI is on `PATH` (v2.89.0) but `gh auth status` failed ("the token in GH_TOKEN is invalid"); GitHub operations instead used the `mcp__github__*` tools, confirmed working (`get_me` succeeded, authenticated as `KMSusong`). `git push --dry-run` reports "Everything up-to-date" — push access is preconfigured; Step 7/8 below confirm it in practice.
- **Data-integrity check:** re-verified Sudan's and the United States' `percentile_cumulative` directly against `latest_status.csv` this run (94.53 and 78.46 respectively) against the correction logged in the 2026-10-26 report — both match; no new transposition or copying errors found.

---

## 2. This week's snapshot

Global picture across the 85 tracked countries/territories, from `latest_status.csv` only. These figures are identical to the last two reports' — the underlying data hasn't changed (see Header) — reproduced here in full per the routine's structure.

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

**Caveat — data recency.** This snapshot is now two weeks older than when it was first reported (2026-10-19) without a re-pull. Of this week's ten targeted countries (Section 3), China's `latest_observed_date` is 2026-08-01 (~3.1 months stale as of today, beyond GDO's 1–2 month nowcast sweet spot); the other eight sit at 2026-09-01 (~2.0 months stale, now at the very edge of/just past the sweet spot) except Mauritania, which sits at 2026-07-01 (~4.1 months stale). **Small-baseline/large-ratio instability:** Jamaica's reported case count this period is a single case against a ~263-case seasonal baseline, and French Guiana's is zero cases against a ~119-case baseline — both too small a sample to read the underlying severity-band move as a strong signal on its own.

---

## 3. News — targeted (10 countries)

**Selection note:** this is a news-only week reusing the active snapshot's existing `movers.csv` (a 2026-10-05 → 2026-10-19 comparison, unchanged for three weeks running): 9 Category A rows and 7 Category B rows, 15 unique countries once de-duplicated (China appears in both categories) — more than the 10-country cap. Per the routine's instructions, Category A/B band-crossings are prioritised over Category C. All 9 Category A countries — China, French Guiana, Honduras, Jamaica, Mexico, Mauritania, Peru, Sudan and the United States — take 9 of the 10 slots; the 10th goes to Brazil (Category B), whose swing from "running well below" to "running well above" is a two-band jump, the largest Category B move in this snapshot. (Same 10-country selection as the two prior news-only-week reports, since `movers.csv` hasn't changed.) What follows is a **fresh news search** for each, covering roughly the last two weeks (2026-10-19 to 2026-11-02); the GDO figures themselves remain unchanged from the last two reports.

### China (CHN) — category A (also category B)

GDO's severity-interpretation read sits at **"Above average – more cases than typical at this point"** (percentile_cumulative 81.4, High band; cases=836), with the monthly-ratio descriptor at "running slightly below" and current-season at Normal (percentile 51.8). **Caveat:** `latest_observed_date` is 2026-08-01, ~3.1 months stale — now the most lagged of this week's targeted figures, well beyond GDO's 1–2 month sweet spot. News lags similarly: WHO's Western Pacific updates (1 and 15 October 2026) put China's national count at 836 cases in August 2026, down from 1,120 in July — and, per the 15 October bulletin, roughly 51% below the same period in 2025. ECDC's own September overview gives a conflicting August figure (67 cases) that doesn't match WHO's — treat the WHO figure as the more reliable of the two. No September- or October-dated national count was found this cycle, despite China CDC's own seasonality work (2005–2023) pointing to a typical September–October peak.
*Source: [WHO Western Pacific dengue update, 1 October 2026](https://cdn.who.int/media/docs/default-source/wpro---documents/emergency/surveillance/dengue/dengue_20261001.pdf); [WHO Western Pacific dengue update, 15 October 2026](https://cdn.who.int/media/docs/default-source/wpro---documents/emergency/surveillance/dengue/dengue_20261015.pdf); [ECDC, Dengue worldwide overview](https://www.ecdc.europa.eu/en/dengue-monthly) (conflicting August figure, treated with caution).*

### French Guiana (GUF) — category A

Holds at **"Below average – fewer cases than typical at this point"** (percentile_cumulative 5.6, Low band). **Small-baseline caveat:** this read sits on a reported case count of 0 against a ~119-case seasonal baseline — essentially no case signal underlying the classification. No French Guiana-specific bulletin newer than August 2026 turned up this cycle (Santé publique France's regional-bulletin series appears to have no fresher instalment indexed yet); the most recent available (21 August) still describes dengue activity as low nationally, with chikungunya the active local concern — 1,507 laboratory-confirmed chikungunya cases since late January, with the West Coast and Savanes sectors both in epidemic phase at that time. Treat French Guiana as a genuine news gap this cycle rather than a confirmed "still quiet" read.
*Source: [Santé publique France, French Guiana bulletin, 21 August 2026](https://www.santepubliquefrance.fr/en/regions-and-territories/french-guiana/regional-bulletin/chikungunya-and-dengue-french-guiana-bulletin-dated-august-21-2026) — no newer bulletin found this cycle.*

### Honduras (HND) — category A

Holds at **"Below average – fewer cases than typical at this point"** (percentile_cumulative 24.6, Low band — just under the Normal cutoff). **Caveat:** `latest_observed_date` is 2026-09-01, ~2.0 months stale — now at the edge of GDO's nowcast sweet spot. Current news tells a less settled story than GDO's own "below average" read: El Heraldo's 27 October report puts the 2026 cumulative national total at 12,281 cases after 692 new confirmed cases that week, and a 28 October follow-up describes 7,217 new cases between epidemiological weeks 25 and 42, with four deaths. This conflicts with La Tribuna's mid-October figure of five deaths (plus a sixth under investigation) against a lower 10,749-case cumulative total at that point. **Caveat:** the case trajectory (rising cumulative total) doesn't obviously match GDO's "below average" band — the two outlets' death tolls and cutoff weeks also don't reconcile cleanly, so treat the overall direction as unsettled rather than confirmed easing, pending an official Sesal bulletin.
*Source: [El Heraldo, 27 October 2026](https://www.elheraldo.hn/honduras/honduras-confirma-692-nuevos-casos-dengue-acumula-12-281-ano-AA32459801); [El Heraldo, 28 October 2026](https://www.elheraldo.hn/honduras/dengue-casos-zancudo-vacuna-muertes-PD32468117); [La Tribuna, 13 October 2026](https://www.latribuna.hn/2026/10/13/honduras-reporta-cinco-muertes-por-dengue-grave-en-2026-e-investiga-otro-fallecimiento/).*

### Jamaica (JAM) — category A

Holds at **"Below average – fewer cases than typical at this point"** (percentile_cumulative 19.8, Low band). **Small-baseline caveat:** the underlying reported case count is 1, against a seasonal baseline of ~263 — a single observed case is not a trend in itself, however the classification reads. Still no 2026-dated, Jamaica-specific case count found this cycle; the most recent concrete figure located remains the Ministry's 2025 year-to-date count of 379 cases (versus 1,819 over the same period in 2024), with the Minister describing the 2025/2026 season as delayed-onset or simply low-activity. A January 2026 Jamaica Observer piece says cases "remain below the alert threshold" despite an increase, but without a number attached. This stays a genuine, unresolved news gap rather than a settled "quiet" story.
*Source: no current (2026) Jamaica-specific case count found; [Jamaica Observer, 14 October 2025](https://www.jamaicaobserver.com/2025/10/14/two-deaths-recorded-low-activity-delayed-dengue-season-tufton/) (most recent concrete figure, year-old); [Jamaica Observer, 9 January 2026](https://www.jamaicaobserver.com/2026/01/09/health-personnel-st-elizabeth-continue-campaign-prevent-spread-mosquito-borne-diseases/).*

### Mexico (MEX) — category A

Holds at **"Average – typical case load at this point"** (percentile_cumulative 28.8, Normal band). **Caveat:** `latest_observed_date` is 2026-09-01, ~2.0 months stale. No October-dated national total was found this cycle; reporting remains fragmented by state and cutoff week — a TV Azteca item cites week-29 federal surveillance data (>3,400 confirmed cases nationally) while an Excélsior figure of 4,152 cases (Sonora leading) isn't clearly dated to the same week, and the two don't reconcile. Separately, Hidalgo reported 28 cases as of 8 October and Guanajuato 161 cases year-to-date (a 73% drop on 2025) — both small, state-level, and broadly consistent with GDO's "typical" national read. **Caveat:** treat the national case counts as approximate and not mutually consistent across outlets; the direction (no escalation) is the more reliable read than any single total.
*Source: [TV Azteca, Mexico dengue 2026 overview](https://www.tvazteca.com/aztecanoticias/dengue-en-mexico-2026-estados-mas-casos-sintomas-y-prevencion/); [Excélsior, Mexico dengue cases](https://www.excelsior.com.mx/nacional/dengue-mexico-2026); [Milenio, Hidalgo/Guanajuato state figures, October 2026](https://www.milenio.com/buscador?text=DENGUE).*

### Mauritania (MRT) — category A

Holds at **"Average – typical case load at this point"** (Normal band, percentile_cumulative 29.3). Cases=36, `latest_observed_date` 2026-07-01 — ~4.1 months stale, well beyond GDO's 1–2 month sweet spot, so treat this read cautiously. Current-season percentile sits higher, at 72.5 ("Average"). No 2026-dated Mauritania-specific figures turned up this cycle, but one new piece of regional context: an Africa CDC-sourced aggregator describes Mali as having the largest 2026 dengue outbreak in West Africa (~590 cases), with Mauritania named alongside Senegal and the Central African Republic as a smaller 2026 outbreak location, without a specific case count. This is consistent with — though doesn't independently confirm — GDO's own "typical, not escalating" read for Mauritania (see also Section 4, Mali).
*Source: [Mappr, Dengue Outbreak 2026: Cases by Country](https://www.mappr.co/dengue-outbreak-map/) (Africa CDC-sourced, regional context only; no Mauritania-specific count); no newer Mauritania-specific bulletin found this cycle.*

### Peru (PER) — category A (also category C)

GDO: cumulative severity remains **"Rare bad event – unusually high cases to date"** (percentile_cumulative 97.9, Extremely High); current-season percentile 49.1 ("Average"). Cases=7,685, `latest_observed_date` 2026-09-01 (~2.0 months stale). News this cycle corroborates a continuing escalation, though exact figures diverge between outlets: Rio Times puts the cumulative 2026 total at 76,784 cases and 81 deaths as of 17 October (versus 32,372 cases and 51 deaths a year earlier), while Latin Times gives 78,912 cases through 23 October — a 122% year-on-year rise — and 72 confirmed deaths with 13 more under investigation; Canal N separately describes a ~79% year-on-year rise. The percentage comparisons don't agree between outlets, so lead with direction, not a specific growth figure. The more significant development: on 20–21 October, MINSA and Peru's CDC issued Epidemiological Alert No. 008-2026, warning that an anticipated El Niño event for 2026–2027 could drive a second dengue wave on top of the current season, alongside rising leptospirosis and diarrhoeal disease. La Libertad (~14,452 cases) and Piura (>14,000 cases, 13+ deaths) are the hardest-hit regions cited. **Caveat:** treat all case/death totals above as approximate and mutually inconsistent across sources; the El Niño second-wave warning and the overall escalating direction are the more reliable takeaways.
*Source: [Rio Times, Peru warns El Niño could fuel more dengue in 2026](https://www.riotimesonline.com/peru-warns-el-nino-could-fuel-more-dengue-2026/); [Latin Times, Peru dengue cases, El Niño second wave](https://www.latintimes.com/peru-dengue-cases-el-nino-second-wave-600565); [Canal N, casos de dengue aumentan en Perú](https://canaln.pe/actualidad/casos-dengue-aumentan-79-peru-minsa-advierte-que-podrian-incrementarse-altas-temperaturas-n495247).*

### Sudan (SDN) — category A (also category C)

GDO: cumulative severity remains **"Above average – more cases than typical at this point"** (percentile_cumulative 94.5, High band, just under the Extremely High cutoff); current-season percentile 72.6. Cases=2,636, `latest_observed_date` 2026-09-01 (~2.0 months stale). The Tawila/North Darfur story flagged last cycle has escalated further: the General Coordination of Displaced Persons and Refugees in Darfur reported over 500 dengue cases in Tawila on 12 October, revising this upward to 927 cases (September to 16 October) in a follow-up statement, warning of a severe medicine shortage and growing pressure on Tawila Rural Hospital amid a large, conflict-displaced population. **Caveat:** these figures come from a displaced-persons advocacy group, not an official health-ministry count, and conflict-disrupted surveillance means small-baseline/large-swing instability is a live risk — read the direction (a worsening, under-resourced local outbreak in Darfur specifically) with caution, not the precise numbers, and note this sits alongside, not in contradiction of, GDO's calmer national-level "above average" read.
*Source: [Sudan Tribune, 12 October 2026](https://sudantribune.com/?p=319868); [Sudan Tribune, 17 October 2026](https://sudantribune.com/?p=320054).*

### United States (USA) — category A (also category C)

GDO: cumulative severity remains **"Above average – more cases than typical at this point"** (percentile_cumulative 78.5, High band); current-season percentile 58.5. Cases=339, `latest_observed_date` 2026-09-01 (~2.0 months stale). Florida's outbreak keeps climbing: the Florida Department of Health's week-41 arbovirus report (11–17 October 2026) counts 425 locally-acquired dengue cases for the year across eleven counties, with 57 new cases in week 41 alone, up from 368 at week 40. Hillsborough County accounts for the large majority (346 cases), with Pinellas a distant second (51). Travel-associated cases are tracked separately and stood at 288 for the year as of the week-40 report. **Caveat:** a travel-blog claim of 721 cumulative cases "since September" circulating online does not match the official Department of Health weekly reports and should not be used; a reported first Florida dengue death (Hillsborough County) also could not be traced to a dated, primary source this cycle and should be treated as unverified pending an official confirmation. As before, frame any post around Hillsborough/Florida specifically, not a US-wide trend.
*Source: [Florida Department of Health, Arbovirus Surveillance Report, Week 41 2026](https://www.floridahealth.gov/wp-content/uploads/2026/10/fl-arbovirus-report-w41-2026.pdf); [Florida Department of Health, Arbovirus Surveillance Report, Week 40 2026](https://www.floridahealth.gov/wp-content/uploads/2026/10/fl-arbovirus-report-w40-2026.pdf).*

### Brazil (BRA) — category B

GDO: monthly ratio descriptor remains **"running well above"** — the largest Category B move in this snapshot, carried over from the last two reports. Cases=63,952 (`latest_observed_date` 2026-09-01). Cumulative severity remains Normal (percentile_cumulative 52.6); current-season severity is Extremely Low (percentile ≈0), so "running well above" continues to read as a relative-to-seasonal-baseline move within an otherwise quiet season, not a return to a major outbreak. No fresh Brazil-specific case count newer than an August Prensa Latina figure (~1.5 million cases, ~400 deaths nationally year-to-date) was found this cycle; an InfoDengue–Mosqlimate/Fiocruz forecast still projects 1.8 million cases nationally for 2026, 54% concentrated in São Paulo state, with most states expected to peak below 2024–2025 season levels. **Caveat:** no current (October) Brazil-specific figure corroborates this week's GDO signal directly — the direction is plausible against the broader PAHO regional picture (Section 4) but not independently confirmed for Brazil at a comparable, current cutoff.
*Source: [Prensa Latina, 12 August 2026](https://www.prensa-latina.cu/?p=748954); [PNNL / One Health, dengue forecasting study, 1 October 2026](https://www.pnnl.gov/publications/environmental-and-epidemiological-drivers-dengue-forecasting-across-heterogeneous) (forecast context, see also Section 7).*

---

## 4. News — general scan (5 items)

Independent broad scan, capped at 5, for the last ~2 weeks (2026-10-19 to 2026-11-02); includes GDO-tracked countries outside this week's 10-country target list and non-endemic/non-GDO settings per the routine's instruction.

1. **Bangladesh — a record month.** October 2026 set the year's monthly case record: 44,228 new dengue cases, edging out September's 43,774, per the Directorate General of Health Services (DGHS). Deaths climbed too — 139 fatalities in October alone, bringing the 2026 toll to 384 — and 15 October saw ten deaths in 24 hours, matching the year's single-day high. GDO independently flags Bangladesh High/High (cumulative and current-season), "running well above" — a rare case of national surveillance and GDO's nowcast pointing the same direction at the same time. Bangladesh is GDO-tracked but wasn't among this week's 10 targeted countries. *[Dhaka Tribune, upward trend in dengue cases, October](https://www.dhakatribune.com/bangladesh/health/394875/upward-trend-in-dengue-cases-october-sees-more); [bdnews24, 25 October 2026](https://bdnews24.com/health/3h6e1vg2ho).*
2. **Sri Lanka — a declining trend, with a monsoon caveat attached.** The National Dengue Control Unit's most recent available count (through early September) puts the 2026 cumulative total at 97,027 cases and 74 deaths, already well past 2025's full-year total of 51,479; weekly cases have fallen continuously since week 27, after a July peak of 29,978 infections (Western Province carrying over half the national burden). The Unit's own director has warned, though, that the North-East monsoon could push cases back up. GDO shows Sri Lanka cumulative Extremely High / current-season High — consistent with "elevated but past its peak." No October-dated figure was found this cycle, so treat the declining trend as the position in September, not now. *[Ada Derana, Sri Lanka dengue cases and deaths, 2026](https://www.adaderana.lk/news/123206/over-33000-dengue-cases-and-19-deaths-reported-so-far-in-2026); [mesvaccins.net, Sri Lanka weekly trend since week 27](https://www.mesvaccins.net/web/news/24340-sri-lanka-le-nombre-de-cas-de-dengue-diminue-de-maniere-continue-depuis-la-semaine-27-de-2026).*
3. **Philippines — national decline, local exception.** The Philippines' Department of Health reports national 2026 totals running 31–36% below the same period in 2025 (figures of 138,538 cases through 5 September and 161,925 "to date" both circulating, cutoffs unclear). Against that backdrop, Agusan del Sur province declared a province-wide dengue outbreak on 29 September — one of several areas (alongside Sulu, BARMM and Abra) that breached epidemic thresholds at least twice in the preceding four weeks. The Philippines isn't GDO-tracked; this is a useful reminder that a reassuring national trend can still mask a genuine local outbreak. *[GMA News, DOH dengue cases, October before typhoons](https://www.gmanetwork.com/news/topstories/nation/967023/doh-dengue-cases-went-down-to-14k-cases-in-october-before-typhoons/story); [Outbreak News Today, Agusan del Sur province-wide outbreak](https://outbreaknewstoday.substack.com/p/philippines-agusan-del-sur-health).*
4. **West Africa — Mali, not Mauritania, carries this year's largest regional outbreak.** An Africa CDC-sourced aggregator reports Mali's 2026 dengue outbreak (~590 cases) as the largest in West Africa this year, with Mauritania (one of this week's 10 targeted countries, Section 3), Senegal and the Central African Republic named as smaller 2026 outbreak locations, no case counts given for the latter three. Mali isn't GDO-tracked. Useful context for reading Mauritania's own "typical, not escalating" GDO signal — the wider region isn't reporting anything close to a 2025-style major outbreak this year. *[Mappr, Dengue Outbreak 2026: Cases by Country](https://www.mappr.co/dengue-outbreak-map/) (Africa CDC-sourced).*
5. **Spain — imported cases, a different seasonal pattern from locally-acquired Europe.** Spain's Ministry of Health's Aedes-disease surveillance bulletin (26 October 2026) reports imported dengue cases continuing to arrive from the Maldives — an importation pattern first identified in 2025 — through epidemiological week 43, alongside a renewed run of imported cases from Cuba since week 27; all of Spain's 2026 dengue cases are travel-associated (137 notified as of early August, total not yet updated in these results). Distinct from the France/Italy locally-acquired-case story covered in the 2026-10-26 report — this is the travel-import side of the same European dengue picture, not autochthonous transmission. Spain isn't GDO-tracked. *[Ministerio de Sanidad (Spain), Aedes-borne disease surveillance bulletin, 26 October 2026](https://www.sanidad.gob.es/en/areas/alertasEmergenciasSanitarias/preparacionRespuesta/docs/20261026_Informe_seguimiento_Enf_transmitidas_Aedes_2026.pdf).*

---

## 5. Trend since last update

No new GDO data this week — `latest_status.csv` and `movers.csv` are unchanged from the 2026-10-19 and 2026-10-26 reports (third consecutive news-only week; see Header). For completeness, the active `movers.csv` (a 2026-10-05 → 2026-10-19 comparison) breaks down as:

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

1. **Peru — the strongest, most official signal this week.** GDO's own category A/C crossing (cumulative now Extremely High) is now reinforced by an explicit MINSA/CDC Peru Epidemiological Alert (No. 008-2026, 20–21 October) warning that an anticipated El Niño 2026–2027 event could trigger a second dengue wave. *Caveat: cite the El Niño warning and the overall escalating direction, not a specific growth percentage — outlets disagree on the exact year-on-year rise (79% vs. 122%).*
2. **Bangladesh — a genuinely record month, corroborated independently.** 44,228 new cases in October (a 2026 monthly record), 139 deaths in the month, and a single-day record of 10 deaths on 15 October, all from DGHS — and GDO's own High/High, "running well above" read points the same direction. *No major caveat — official national surveillance data, directly consistent with GDO's nowcast.*
3. **Sudan — the Darfur story keeps escalating.** The displaced-persons-reported Tawila dengue outbreak has nearly doubled on paper, from 500+ cases (12 October) to 927 (by 16 October), amid a documented medicine shortage. *Caveat: figures come from a displaced-persons advocacy group, not an official count, and conflict-disrupted surveillance makes exact numbers unstable — lead with the humanitarian/access angle, not precise case counts.*
4. **Florida, United States — still climbing, now past 400 cases.** 425 locally-acquired cases through week 41 (up from 368 two weeks prior), heavily concentrated in Hillsborough County (346 of 425). *Caveat: frame as a Hillsborough/Florida story, not a US-wide trend; do not cite the unverified 721-case travel-blog figure or the unconfirmed single-death claim circulating online.*
5. **Honduras — rising case count, but treat the numbers as provisional.** Cumulative 2026 total now reported at 12,281 (up 692 in the latest week), a clear upward case trajectory that sits awkwardly against GDO's own "below average" read — worth a post on the divergence itself, framed carefully. *Caveat: death tolls (four vs. five, plus one under investigation) and cumulative totals disagree between El Heraldo and La Tribuna — do not quote a single precise figure as settled; an official Sesal bulletin would resolve this.*

---

## 7. Scientific literature findings

Lighter-effort pass; a handful of recent items across forecasting and vaccine policy.

- **Forecasting (Singapore, Nature Communications):** Adding circulating dengue-serotype data to a climate-driven model improved outbreak-risk prediction, with risk highest during El Niño conditions and useful lead time of up to two months — directly relevant to this week's Peru alert (Section 3/6), which cites the same El Niño mechanism. [BioSpectrum Asia, 2026](https://www.biospectrumasia.com/news/30/27364/singapore-researchers-combines-climate-and-virus-surveillance-to-predict-dengue-outbreak-risk-two-months-in-advance.html)
- **Forecasting (Brazil and Panama, One Health, October 2026):** An ensemble model combining surveillance, climate, environmental and demographic data cut forecasting error by roughly 20% in Brazil and 36% in Panama relative to the best single-model alternative. [PNNL, 1 October 2026](https://www.pnnl.gov/publications/environmental-and-epidemiological-drivers-dengue-forecasting-across-heterogeneous)
- **Vaccine policy (Brazil) — an update that revises last week's open question:** the 2026-10-26 report flagged that Brazil's single-dose Butantan-DV vaccine had been "confirmed for inclusion" in the national SUS programme within 2026. Fresher reporting this cycle complicates that: as of October 2026, Qdenga is described as the *only* dengue vaccine currently in SUS (two doses, ages 10–14), while the Butantan-DV vaccine has in fact been **suspended since 8 June 2026** as a precaution, with leftover doses being collected by state health centres. Treat the earlier "confirmed for SUS inclusion" line as superseded — the current, more reliable picture is Qdenga-only, Butantan-DV on hold. [Ground News, Brazil approves single-dose dengue vaccine (background)](https://ground.news/article/brazil-approves-worlds-first-single-dose-dengue-vaccine); Brazilian health-press reporting on the current SUS vaccine roster and Butantan-DV suspension, October 2026.
- **Vaccine policy (India) — new approval:** India's CDSCO authorised Qdenga, the country's first dengue vaccine, in July 2026, for ages 4–60. [The Policy Edge](https://www.policyedge.in/p/cdsco-approves-indias-first-dengue-vaccine-individuals-aged-460-years)

---

## 8. Appendix

### 8.1 `movers.csv` (active snapshot, full table — unchanged from the 2026-10-19 and 2026-10-26 reports)

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

1. WHO Western Pacific, dengue situation update, 1 October 2026 — https://cdn.who.int/media/docs/default-source/wpro---documents/emergency/surveillance/dengue/dengue_20261001.pdf
2. WHO Western Pacific, dengue situation update, 15 October 2026 — https://cdn.who.int/media/docs/default-source/wpro---documents/emergency/surveillance/dengue/dengue_20261015.pdf
3. ECDC, Dengue worldwide overview — https://www.ecdc.europa.eu/en/dengue-monthly
4. Santé publique France, French Guiana bulletin, 21 August 2026 — https://www.santepubliquefrance.fr/en/regions-and-territories/french-guiana/regional-bulletin/chikungunya-and-dengue-french-guiana-bulletin-dated-august-21-2026
5. El Heraldo (Honduras), 27 October 2026 — https://www.elheraldo.hn/honduras/honduras-confirma-692-nuevos-casos-dengue-acumula-12-281-ano-AA32459801
6. El Heraldo (Honduras), 28 October 2026 — https://www.elheraldo.hn/honduras/dengue-casos-zancudo-vacuna-muertes-PD32468117
7. La Tribuna (Honduras), 13 October 2026 — https://www.latribuna.hn/2026/10/13/honduras-reporta-cinco-muertes-por-dengue-grave-en-2026-e-investiga-otro-fallecimiento/
8. Jamaica Observer, 14 October 2025 — https://www.jamaicaobserver.com/2025/10/14/two-deaths-recorded-low-activity-delayed-dengue-season-tufton/
9. Jamaica Observer, 9 January 2026 — https://www.jamaicaobserver.com/2026/01/09/health-personnel-st-elizabeth-continue-campaign-prevent-spread-mosquito-borne-diseases/
10. TV Azteca, Mexico dengue 2026 overview — https://www.tvazteca.com/aztecanoticias/dengue-en-mexico-2026-estados-mas-casos-sintomas-y-prevencion/
11. Excélsior (Mexico), dengue cases — https://www.excelsior.com.mx/nacional/dengue-mexico-2026
12. Milenio (Mexico), dengue search results (Hidalgo/Guanajuato state figures) — https://www.milenio.com/buscador?text=DENGUE
13. Mappr, Dengue Outbreak 2026: Cases by Country (Africa CDC-sourced) — https://www.mappr.co/dengue-outbreak-map/
14. Rio Times, Peru warns El Niño could fuel more dengue in 2026 — https://www.riotimesonline.com/peru-warns-el-nino-could-fuel-more-dengue-2026/
15. Latin Times, Peru dengue cases, El Niño second wave — https://www.latintimes.com/peru-dengue-cases-el-nino-second-wave-600565
16. Canal N (Peru), casos de dengue aumentan en Perú — https://canaln.pe/actualidad/casos-dengue-aumentan-79-peru-minsa-advierte-que-podrian-incrementarse-altas-temperaturas-n495247
17. Sudan Tribune, 12 October 2026 — https://sudantribune.com/?p=319868
18. Sudan Tribune, 17 October 2026 — https://sudantribune.com/?p=320054
19. Florida Department of Health, Arbovirus Surveillance Report, Week 41 2026 — https://www.floridahealth.gov/wp-content/uploads/2026/10/fl-arbovirus-report-w41-2026.pdf
20. Florida Department of Health, Arbovirus Surveillance Report, Week 40 2026 — https://www.floridahealth.gov/wp-content/uploads/2026/10/fl-arbovirus-report-w40-2026.pdf
21. Prensa Latina, 12 August 2026 — https://www.prensa-latina.cu/?p=748954
22. PNNL / One Health, environmental and epidemiological drivers of dengue forecasting, 1 October 2026 — https://www.pnnl.gov/publications/environmental-and-epidemiological-drivers-dengue-forecasting-across-heterogeneous
23. Dhaka Tribune, upward trend in dengue cases, October — https://www.dhakatribune.com/bangladesh/health/394875/upward-trend-in-dengue-cases-october-sees-more
24. bdnews24, 25 October 2026 — https://bdnews24.com/health/3h6e1vg2ho
25. Ada Derana (Sri Lanka), over 33,000 dengue cases and 19 deaths so far in 2026 — https://www.adaderana.lk/news/123206/over-33000-dengue-cases-and-19-deaths-reported-so-far-in-2026
26. mesvaccins.net, Sri Lanka weekly dengue trend since week 27 — https://www.mesvaccins.net/web/news/24340-sri-lanka-le-nombre-de-cas-de-dengue-diminue-de-maniere-continue-depuis-la-semaine-27-de-2026
27. GMA News (Philippines), DOH dengue cases down to 14K in October before typhoons — https://www.gmanetwork.com/news/topstories/nation/967023/doh-dengue-cases-went-down-to-14k-cases-in-october-before-typhoons/story
28. Outbreak News Today, Philippines — Agusan del Sur province-wide outbreak — https://outbreaknewstoday.substack.com/p/philippines-agusan-del-sur-health
29. Ministerio de Sanidad (Spain), Aedes-borne disease surveillance bulletin, 26 October 2026 — https://www.sanidad.gob.es/en/areas/alertasEmergenciasSanitarias/preparacionRespuesta/docs/20261026_Informe_seguimiento_Enf_transmitidas_Aedes_2026.pdf
30. BioSpectrum Asia, Singapore dengue forecasting study (climate + serotype surveillance) — https://www.biospectrumasia.com/news/30/27364/singapore-researchers-combines-climate-and-virus-surveillance-to-predict-dengue-outbreak-risk-two-months-in-advance.html
31. Ground News, Brazil approves world's first single-dose dengue vaccine (background) — https://ground.news/article/brazil-approves-worlds-first-single-dose-dengue-vaccine
32. The Policy Edge, CDSCO approves India's first dengue vaccine (Qdenga), ages 4–60 — https://www.policyedge.in/p/cdsco-approves-indias-first-dengue-vaccine-individuals-aged-460-years
