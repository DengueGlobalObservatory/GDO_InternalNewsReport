# GDO Internal News Report — 2026-09-28

*Source: Global Dengue Observatory (accessed 2026-09-28).*

## 1. Header

- **Report date:** 2026-09-28 (Monday routine run)
- **Active snapshot:** `snapshots/2026_09_21/` — **unchanged since 2026-09-21** (news-only week; no new pull this run). Source data vintage (`target_render_date`): 2026-09-18. Source commit: `215eb24d` (DENV_global_observatory `Output/2026_09_18/`). Prior snapshot: `snapshots/2026_09_07/` (vintage 2026-09-04).
- **Pull status this week:** **news-only week.** `target_render_date` for this run computes to 2026-09-18 (most recent of {2026-09-04, 2026-09-18, 2026-08-18} strictly before today) — the same vintage already recorded in `snapshots/2026_09_21/manifest.json`. No new render has happened on the public site since the last pull, so Step 1's fetch/diff was skipped per Step 0.5 and this run reuses `snapshots/2026_09_21/` (including its `movers.csv`, itself a 2026-09-07 → 2026-09-21 comparison) as the active snapshot.
- **Countries covered:** 85.
- **Environment note:** this session's container had no R runtime pre-installed; `r-base-core` was self-installed successfully via `apt-get` per the routine's fallback instructions (not otherwise needed this run, since Step 1 was skipped). `gh` CLI is not on `PATH`; GitHub access used the `mcp__github__*` tools instead, authenticated and working. `git push` is preconfigured (`GITHUB_TOKEN` + credential rewrite).

## 2. This week's snapshot

Global picture across the 85 tracked countries/territories, from `latest_status.csv` only. Figures are identical to last week's report — the underlying data hasn't changed (see Header) — reproduced here in full per the routine's structure.

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

Current-season **Extremely High**: Cuba (percentile 100.0), Kenya (100.0), Cambodia (99.2). Current-season **High**: Maldives (90.2), Sri Lanka (87.7), United Republic of Tanzania (78.9), Suriname (76.4). Sri Lanka is worth flagging alongside this week's fresh news (Section 4) — its cumulative standing (96.8th percentile) and current-season standing (87.7, High) are both elevated together, unlike Guyana/Samoa below.

**Notable current-season cooling despite Extremely High cumulative standing:** Guyana's current-season percentile sits at 5.9 (down from 96.7 two pulls ago; Category C, the largest single move in the active `movers.csv`) even as its cumulative severity stays Extremely High (98.6) — a season that ran hot early and has since gone quiet. Samoa shows the same shape on a smaller scale: cumulative High (79.6) but current-season Low (6.3, down from 59.8).

**Caveat — data recency.** This snapshot is now a week older than when it was first reported (2026-09-21) without a re-pull. Of this week's ten targeted countries (Section 3), nine (Afghanistan, Argentina, Burkina Faso, Côte d'Ivoire, Grenada, Malaysia, Panama, Vietnam, Wallis and Futuna) have a latest observed month of 2026-08-01 — now ~1.9 months stale as of today, just past the upper edge of GDO's 1–2 month nowcast sweet spot; Timor-Leste sits at 2026-07-01 (~2.9 months stale, well beyond the sweet spot — treat its figures as lower-confidence). **Small-sample/large-ratio instability:** Argentina's monthly ratio (0.02×) rests on a single observed case against a ~50-case seasonal baseline. Côte d'Ivoire shows the same shape in reverse: 12 observed cases against a much larger ~1,145-case baseline (ratio 0.01×) — treat as a likely reporting-lag/data-availability issue rather than a confirmed collapse (see Section 3).

## 3. News — targeted (10 countries)

**Country selection note:** this is a news-only week reusing the active snapshot's existing `movers.csv` (a 2026-09-07 → 2026-09-21 comparison), so the country pool is unchanged from last week's report: 17 Category A rows and 18 Category B rows (31 unique countries once de-duplicated), well beyond the 10-country cap. The same 10 countries are carried forward — Vietnam, Afghanistan, Malaysia, Wallis and Futuna, Argentina, Burkina Faso, Timor-Leste, Panama, Côte d'Ivoire, Grenada — since the underlying GDO figures and mover flags have not changed; what follows is a **fresh news search** for each (last ~2 weeks, 2026-09-14 to 2026-09-28), not a re-derivation of the GDO data.

### Vietnam (Category A — severity interpretation: Average → Above average; Category B — monthly ratio: running well below → running well above; Category C — current-season percentile 2.4 → 32.6)
- GDO figures (unchanged from last week): 24,069 reported cases (latest observed month 2026-08-01, ~1.9 months stale). Cumulative percentile 85.5 (High); current-season percentile 32.6 (Normal). Estimated total seasonal cases: 237,572. Monthly ratio: running well above (1.31×, off an ~18,422-case baseline).
- News: **fresh, and still escalating.** A US State Department (OSAC) health alert (~18 Sep) reports Hanoi logged over 2,000 dengue cases in a single week — roughly double the count of preceding weeks — concentrated in Phú Xuyên, Hoàng Mai, Cầu Giấy, Hà Đông, Đống Đa, Đan Phượng, Thanh Oai and Thanh Trì districts. Background: 78,000+ cases and 13 deaths nationally by mid-August (20% up on 2025). [OSAC Vietnam Health Alert, ~18 Sep](https://osac.gov/Country/Vietnam/Content/Detail/Report/6fb8fff1-ca66-4489-8f98-226658445563) · [Dengue Visual Atlas, background](https://denguevisualatlas.com/en/78000-cases-of-dengue-in-vietnam-in-2026-20-more-than-the-previous-year/)

### Afghanistan (Category A — severity interpretation: Rare bad event → Above average; Category B — monthly ratio: running well above → tracking near; Category C — current-season percentile 51.0 → 33.2)
- GDO figures (unchanged): 279 reported cases (latest observed month 2026-08-01, ~1.9 months stale). Cumulative percentile 82.2 (High). Current-season percentile 33.2 (Normal), down from 51.0. Estimated total seasonal cases: 6,717. Monthly ratio: tracking near baseline (1.05×).
- News: **fresh, and directionally consistent with GDO's own easing read.** A WHO-sourced report (~27 Sep) states Afghanistan's dengue cases declined 41% in August versus the prior month — lining up with GDO's own percentile pull-back this fortnight, though the underlying data point is itself a month old. [DID Press Agency, ~27 Sep](https://en.didpress.com/37994/)

### Malaysia (Category A — severity interpretation: Average → Above average; Category C — current-season percentile 24.7 → 56.7, the largest current-season increase this snapshot)
- GDO figures (unchanged): 11,629 reported cases (latest observed month 2026-08-01, ~1.9 months stale). Cumulative percentile 83.6 (High). Current-season percentile 56.7 (Normal), up from 24.7. Estimated total seasonal cases: 121,276. Monthly ratio: running well above (1.82×).
- News: no article dated within the strict 2-week window was found this cycle; the most current confirmed figure remains the Ministry of Health's Epidemiological Week 35 report (9 Sep, ~19 days old): 65,979 cases (+66% vs. 39,616 for the same period in 2025) and 62 deaths (vs. 32 in 2025), alongside cabinet-level discussion of *gotong-royong* (community clean-up) vector-control programmes in red-zone areas. **Data-quality note:** a "58,400 cases / 176 deaths (17 Sep)" figure surfaced in search but was excluded here — cross-checking against Section 4 shows this figure actually belongs to Bangladesh, not Malaysia; a search-summarisation mix-up, not a real Malaysia data point. [Malay Mail, 9 Sep](https://www.malaymail.com/news/malaysia/2026/09/09/dengue-cases-soar-66pc-deaths-hit-62-in-malaysia-almost-double-2025-toll/234576)

### Wallis and Futuna (Category A — severity interpretation: Rare bad event → Average; Category B — monthly ratio: running well above → running well below)
- GDO figures (unchanged): 12 reported cases (latest observed month 2026-08-01, ~1.9 months stale). Cumulative percentile 71.7 (Normal). Current-season percentile 44.8 (Normal). Estimated total seasonal cases: 487. Monthly ratio: running well below (0.17×).
- News: **no item within the ~2-week fresh window, again this cycle.** All findable coverage still relates to the territory's earlier-2026 outbreak (local transmission first confirmed on Futuna ~22 April; ~225 cumulative cases cited mid-year without a firm date). Directionally consistent with GDO's own easing read, but not independently confirmed for September for a second consecutive week. [La 1ère, background](https://la1ere.franceinfo.fr/wallisfutuna/dengue-l-epidemie-ralentit-a-futuna-mais-progresse-a-wallis-1711747.html)

### Argentina (Category A — severity interpretation: Average → Below average; Category C — current-season percentile 22.3 → 10.7)
- GDO figures (unchanged): 1 reported case (latest observed month 2026-08-01, ~1.9 months stale). Cumulative percentile 15.9 (Low). Current-season percentile 10.7 (Low). Estimated total seasonal cases: 79. **Caveat:** the monthly ratio (0.02×) rests on a single case against a ~50-case seasonal baseline — noisy in isolation.
- News: **fresh, and consistent with a low-transmission off-season.** Argentina's National Epidemiological Bulletin (Week 38, reported 22 Sep) records one new travel-associated dengue case (history of travel to Ecuador, serotype DENV-3) in Buenos Aires province — the season's third confirmed case so far — alongside six probable chikungunya cases under investigation. No autochthonous transmission; authorities maintain a low-risk classification. This is the main 2026–2027 transmission season not yet under way; it does not contradict GDO's easing read, it confirms the off-season lull. [Diario Crónica, 22 Sep](https://www.diariocronica.com.ar/noticias/2026/09/22/168238-reportan-un-caso-de-dengue-y-seis-probables-de-chikungunya)

### Burkina Faso (Category A — severity interpretation: Above average → Cannot determine; Category B — monthly ratio: running well above → running well below)
- GDO figures (unchanged): 1,142 reported cases (latest observed month 2026-08-01, ~1.9 months stale). Cumulative severity remains **"Cannot determine"** (a data-availability caveat about GDO's own pipeline, not an epidemiological claim). Current-season percentile 42.1 (Normal). Estimated total seasonal cases: 93,174. Monthly ratio: running well below (0.41×).
- News: no item within the strict ~2-week window this cycle either. The Oubritenga regional governor's 10 September alert over an "unusual and rapid increase" in Ziniaré and Zorgho — carried in last week's report as the freshest available item — is now over two weeks old with no update found. The mismatch flagged last week stands: ground reporting suggested continued/worsening transmission even as GDO's own classification shows "Cannot determine" — a data gap, not evidence either way. [Wakat Séra, 10 Sep](https://www.wakatsera.com/burkina-une-augmentation-inhabituelle-et-rapide-de-cas-de-dengue-a-ziniare-et-zorgho/)

### Timor-Leste (Category B — monthly ratio: running well above → running well below; currently the most severe country in this snapshot — Extremely High cumulative, 99.8th percentile)
- GDO figures (unchanged): 18 reported cases (latest observed month 2026-07-01, ~2.9 months stale — beyond GDO's nowcast sweet spot; treat as lower-confidence). Cumulative percentile 99.8 (Extremely High). Current-season severity "Unknown" (percentile 16.5, interpretation "Cannot determine"). Estimated total seasonal cases: 5,230. Monthly ratio: running well below (0.47×).
- News: no item within the ~2-week fresh window; the freshest available figure — an estimated 4,824 cases year-to-date (4.4× an average year), declining month-on-month since April — is itself unchanged from last week and now ~24 days old, so outside the strict window. A WHO SEARO regional epidemiological bulletin dated September 2026 exists but its Timor-Leste-specific content was not verified this pass; worth a follow-up read if a genuinely current figure is needed. [Mappr, Timor-Leste background](https://www.mappr.co/dengue-outbreak-map/) · [WHO SEARO Epi Bulletin, Sep 2026 (unverified content)](https://cdn.who.int/media/docs/default-source/searo/whe/wherepib/2026_09_searo_epi_bulletin1.2.pdf)

### Panama (Category B — monthly ratio: running slightly below → running well above)
- GDO figures (unchanged): 1,688 reported cases (latest observed month 2026-08-01, ~1.9 months stale). Cumulative percentile 84.2 (High). Current-season percentile 53.8 (Normal). Estimated total seasonal cases: 18,528. Monthly ratio: running well above (1.40×).
- News: **fresh, and the mixed-picture story from last week continues with newer figures.** MINSA's most current report (26 Sep) puts cumulative 2026 cases above 8,000 (495 new in the latest reporting week alone), following a 16 September update of 7,565 cumulative cases, 918 hospitalisations YTD (−12.6% vs. 2025), and 19 dengue-associated deaths. A separate MINSA release cites a 27.3% year-on-year decrease versus 2025's 11,088 cases over the same period. **Caveat, unchanged from last week:** GDO's monthly ratio compares this month's cases against Panama's own seasonally-expected baseline for the same calendar month, not against 2025 — so "running well above" (vs. seasonal baseline) and "down 27.3% year-on-year" are not contradictory, but presenting them side-by-side without this context would read as one. **Also note:** a Metro Libre headline juxtaposes the case count with a separate "63 muertes por influenza" (influenza deaths) figure — don't conflate that with dengue deaths (19, per MINSA above). [Infobae, 26 Sep](https://www.infobae.com/panama/2026/09/26/panama-supera-los-8000-casos-de-dengue-tras-sumar-495-en-una-semana/) · [Infobae, 16 Sep](https://www.infobae.com/panama/2026/09/16/panama-registra-7565-casos-acumulados-de-dengue-y-baja-las-hospitalizaciones-en-145/) · [EcoTV Panama, YoY decrease](https://www.ecotvpanama.com/nacionales/minsa-reporta-disminucion-del-273-los-casos-dengue-panama-n6093122)

### Côte d'Ivoire (Category A — severity interpretation: Average → Below average; Category C — current-season percentile 35.8 → 10.0)
- GDO figures (unchanged): 12 reported cases (latest observed month 2026-08-01, ~1.9 months stale). Cumulative percentile 11.8 (Low). Current-season severity "Unknown" (percentile 10.0, interpretation "Cannot determine" — copied verbatim despite the apparent internal inconsistency, likely an upstream pipeline quirk). Estimated total seasonal cases: 509. **Caveat:** the monthly ratio (0.01×, 12 cases against a ~1,145-case baseline) is a near-total collapse relative to expectation — more likely a reporting-lag/data-availability issue than a confirmed improvement.
- News: **correction to last week's report.** No 2026-dated dengue news for Côte d'Ivoire was found this cycle despite multiple targeted searches. Last week's report cited a Ministry of Health "6th dengue epidemic" item (73 confirmed cases, 2 deaths, Cocody-Bingerville) as current; on closer dating this cycle, that item traces to **Bulletin Épidémiologique N°770/2023 — July 2023**, not 2026. Flagging this for the researcher so the 2023 figure isn't carried forward as a live 2026 data point in future posts. Recommend noting "no current dengue news identified for Côte d'Ivoire" rather than citing that item again.

### Grenada (Category B — monthly ratio: running well below → running well above)
- GDO figures (unchanged): 63 reported cases (latest observed month 2026-08-01, ~1.9 months stale). Cumulative percentile 55.1 (Normal). Current-season percentile 30.2 (Normal). Estimated total seasonal cases: 255. Monthly ratio: running well above (1.60×).
- News: no fresher item found despite renewed searches for Epi Weeks 36/37. The Ministry of Health "urges vigilance" item cited last week (a rise from 6 to 23 cases, Epi Week 33, 16–22 Aug) remains the most recent Grenada-specific coverage, now 5–6 weeks old — a genuine data gap rather than a sign nothing is happening; rely on GDO's own banding (above) over this ageing news item. [NOW Grenada, Aug 2026](https://nowgrenada.com/2026/08/ministry-of-health-urges-vigilance-amid-increase-in-dengue-cases/)

## 4. News — general scan (5 items)

Independent broad scan, capped at 5, for the last ~2 weeks (2026-09-14 to 2026-09-28); includes GDO-tracked countries outside this week's 10-country target list and non-endemic settings per the routine's instruction.

1. **Florida, United States, death confirmed 2026-09-18 (occurred 2026-09-04)** — An 80-year-old Hillsborough County woman died from dengue complications after a local mosquito bite — Florida's first confirmed dengue death of 2026 and the county's worst outbreak since the 1930s (134 local cases this summer; ~332 statewide, 147+ locally acquired, as of mid-September). Orange County (Orlando) separately confirmed a second locally-acquired case around 26 September, showing spread beyond Tampa. Non-endemic in GDO terms; continues the "dengue's US range is expanding" thread from prior weeks. [WTSP, 18 Sep](https://www.wtsp.com/article/news/health/dengue-fever-death-hillsborough-florida/67-17b51105-cc12-4eab-8046-52e7a30a823b) · [Newsweek, map of 2026 US cases](https://www.newsweek.com/map-shows-dengue-fever-cases-each-state-as-florida-records-first-2026-death-12466232)
2. **Bangladesh, as of 2026-09-17 — deaths accelerating sharply** — 58,400 cumulative cases and 176 deaths for the year; 79 deaths recorded in just the first 17 days of September, versus 43 for all of August and 36 in July — a marked acceleration in the fatality rate, not just a routine bulletin uptick. GDO-tracked (High cumulative severity, running well above ratio) but not among this week's 10 targeted countries. [Outbreak News Today, 17 Sep](https://outbreaknewstoday.substack.com/p/bangladesh-dengue-cases-top-70000) · [Deccan Herald](https://www.deccanherald.com/world/bangladesh-sees-worst-single-day-surge-in-dengue-cases-and-deaths-this-year-3738118)
3. **Americas region-wide, epi week 35 (through ~2026-09-25)** — PAHO's Grade-3 (highest-level) multi-country outbreak response now covers 1,658,783 suspected cases, 3,176 severe cases and 507 deaths region-wide — still down 57% versus 2025 and 64% versus the five-year average, but Brazil alone accounts for ~80% of regional cases, and Brazil, Colombia, Costa Rica, El Salvador, Mexico, Panama and Puerto Rico are all reporting simultaneous circulation of all four serotypes. Useful regional counter-narrative to this week's individual escalation stories. [PAHO/WHO, EW35 2026](https://www.paho.org/en/documents/dengue-epidemiological-situation-region-americas-epidemiological-week-35-2026)
4. **Sri Lanka, through late September 2026** — Cases have passed 100,000 with 74 deaths (up from >96,000 cases/72 deaths as of 4 September), running at roughly 2.5× Sri Lanka's 2025 pace; Western Province remains worst-affected. GDO-tracked and already Extremely High cumulative (96.8th percentile) and High current-season (87.7th) — not among this week's 10 targeted countries, but the scale here makes it worth flagging on its own. [Newswire.lk, 4 Sep](https://www.newswire.lk/2026/09/04/sri-lanka-dengue-cases-surpass-96000-as-deaths-reach-72/) · [Lanka Newspapers, 23 Sep](https://www.lankanewspapers.com/2026/09/23/dengue-crisis-deepens-sri-lanka-reports-alarming-case-numbers-as-of-late-september-2026)
5. **Philippines, Aurora province, January–September 2026 (reported 2026-09-23)** — Aurora province logged 2,172 dengue cases for the year, a 137% increase on the same period in 2025, with 7 deaths; children aged 1–10 made up nearly half of all infections (917 cases, 42%) — a sharp localised escalation even as the Philippines' national case count runs 33% down year-on-year. Continues the "national improvement can mask a worsening sub-region" theme from prior weeks' Cebu coverage. Not GDO-tracked. [Tribune.net.ph, 23 Sep](https://tribune.net.ph/2026/09/23/aurora-dengue-cases-surge-137-to-2172)

## 5. Trend since last update

No new data this week — the active snapshot, `latest_status.csv` and `movers.csv` are unchanged from the 2026-09-21 report (news-only week; see Header). See that report's Section 5 for the last full A/B/C mover breakdown.

## 6. Social-media candidate flags

Ranked short-list, for the researcher drafting Tuesday's posts.

1. **Sri Lanka — the region's clearest, largest-scale story this fortnight.** Cases have passed 100,000 with 74 deaths, running ~2.5× 2025's pace. GDO's own figures back this up independently: Extremely High cumulative severity (96.8th percentile) *and* High current-season standing (87.7th) — both elevated together, unlike this week's cooling movers (Guyana, Samoa). *No major caveat — GDO's standing read and the fresh press figures line up cleanly.*
2. **Panama — the "read GDO's ratio carefully" explainer, now with fresher numbers.** MINSA's newest figures (>8,000 cumulative cases, 495 added in the latest week) sit alongside a reported 27.3% year-on-year decrease versus 2025 — while GDO's own monthly ratio reads "running well above" its seasonal baseline. Good material for a post about why a seasonal-baseline ratio and a year-on-year press figure can point in different directions without contradicting each other. *Caveat: frame as methodology, not alarm — and don't conflate MINSA's 19 dengue deaths with an unrelated influenza-death figure circulating in some coverage.*
3. **Vietnam — still the standout GDO mover, and the news keeps confirming it.** A fresh OSAC alert (~18 Sep) reports Hanoi cases doubling week-on-week, on top of GDO's own current-season percentile jump (2.4 → 32.6, the largest swing in the active snapshot). *No major caveat — consistent second week running.*
4. **Florida, United States — the state's first dengue death of 2026.** An 80-year-old Hillsborough County resident died from a locally-acquired infection; the county's worst outbreak since the 1930s. Strong "dengue's reach is expanding" angle for a non-endemic audience. *Caveat: Florida isn't GDO-tracked — this is a general-scan item, not a GDO nowcast reading.*
5. **Bangladesh — deaths accelerating, not just cases.** 79 deaths in the first 17 days of September alone versus 43 for all of August is a fatality-rate story, distinct from (and arguably more striking than) a rising case count. GDO-tracked but outside this week's 10-country selection. *Caveat: as in prior weeks, GDO's own nowcast vintage sits well behind this surge — don't attribute the September press figures to GDO directly.*

## 7. Scientific literature findings

Lighter-effort pass; a handful of recent items across forecasting, climate, surveillance methods and vaccine policy.

- **Forecasting:** A hybrid discrete-wavelet-transform + SARMA + LSTM model for weekly dengue case forecasting (trained on 2012–2022 Quezon City, Philippines data) outperformed traditional SARMA and simple thresholding, and the authors propose it as a basis for dynamic (rather than fixed) epidemic alarm thresholds. *PLOS Neglected Tropical Diseases*, 9 Jul 2026. [PLOS NTD](https://journals.plos.org/plosntds/article?id=10.1371%2Fjournal.pntd.0014444)
- **Climate drivers:** A comment piece argues climate change, extreme weather and socioeconomic shifts are jointly driving dengue surges, and that building climate resilience requires better vector control, surveillance, climate-informed burden projections, and cross-sector (health/environment/climate) partnerships — directly relevant to several of this week's escalation stories (Sri Lanka, Florida, Bangladesh). *Nature Reviews Microbiology*, Sep 2026. [Nature](https://www.nature.com/articles/s41579-026-01329-4)
- **Surveillance methods:** A systematic review and meta-analysis of 10 wastewater-based dengue surveillance studies found a pooled DENV positivity rate of 24% (95% CI 20–28%), with solid-phase sample processing plus RT-dPCR the most sensitive detection approach and wastewater solids (rather than the liquid fraction) the most reliable matrix for RNA recovery. *Viruses* (MDPI), 30 Apr 2026. [DOI](https://doi.org/10.3390/v18050531)
- **Vaccine policy:** A survey of 18 advisory bodies across 17 countries found substantial divergence in Qdenga (TAK-003) travel-vaccination guidance — some restrict eligibility to travellers with documented prior dengue infection, others extend it to seronegative travellers or base eligibility purely on destination exposure risk — reflecting differing interpretations of the same trial evidence. *Journal of Travel Medicine*, 22 Jul 2026. [DOI](https://doi.org/10.1093/jtm/taag065)

## 8. Appendix

### 8.1 `movers.csv` (active snapshot, full table — unchanged from 2026-09-21 report)

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

1. OSAC, Vietnam Health Alert — Hanoi dengue cases doubling (~18 Sep) — https://osac.gov/Country/Vietnam/Content/Detail/Report/6fb8fff1-ca66-4489-8f98-226658445563
2. Dengue Visual Atlas, 78,000 cases of dengue in Vietnam in 2026, background — https://denguevisualatlas.com/en/78000-cases-of-dengue-in-vietnam-in-2026-20-more-than-the-previous-year/
3. DID Press Agency, Afghanistan dengue cases declined 41% in August (~27 Sep) — https://en.didpress.com/37994/
4. Malay Mail, dengue cases soar 66pc, deaths hit 62 in Malaysia (9 Sep) — https://www.malaymail.com/news/malaysia/2026/09/09/dengue-cases-soar-66pc-deaths-hit-62-in-malaysia-almost-double-2025-toll/234576
5. La 1ère, dengue: l'épidémie ralentit à Futuna mais progresse à Wallis, background — https://la1ere.franceinfo.fr/wallisfutuna/dengue-l-epidemie-ralentit-a-futuna-mais-progresse-a-wallis-1711747.html
6. Diario Crónica, reportan un caso de dengue y seis probables de chikungunya (22 Sep) — https://www.diariocronica.com.ar/noticias/2026/09/22/168238-reportan-un-caso-de-dengue-y-seis-probables-de-chikungunya
7. Wakat Séra, Burkina: une augmentation inhabituelle et rapide de cas de dengue à Ziniaré et Zorgho (10 Sep) — https://www.wakatsera.com/burkina-une-augmentation-inhabituelle-et-rapide-de-cas-de-dengue-a-ziniare-et-zorgho/
8. Mappr, Timor-Leste dengue outbreak map, background — https://www.mappr.co/dengue-outbreak-map/
9. WHO SEARO, Regional Epidemiological Bulletin, Sep 2026 (content unverified this pass) — https://cdn.who.int/media/docs/default-source/searo/whe/wherepib/2026_09_searo_epi_bulletin1.2.pdf
10. Infobae, Panamá supera los 8,000 casos de dengue tras sumar 495 en una semana (26 Sep) — https://www.infobae.com/panama/2026/09/26/panama-supera-los-8000-casos-de-dengue-tras-sumar-495-en-una-semana/
11. Infobae, Panamá registra 7,565 casos acumulados de dengue y baja las hospitalizaciones en 14.5% (16 Sep) — https://www.infobae.com/panama/2026/09/16/panama-registra-7565-casos-acumulados-de-dengue-y-baja-las-hospitalizaciones-en-145/
12. EcoTV Panamá, MINSA reporta disminución del 27.3% los casos dengue Panamá — https://www.ecotvpanama.com/nacionales/minsa-reporta-disminucion-del-273-los-casos-dengue-panama-n6093122
13. NOW Grenada, Ministry of Health urges vigilance amid increase in dengue cases (Aug 2026) — https://nowgrenada.com/2026/08/ministry-of-health-urges-vigilance-amid-increase-in-dengue-cases/
14. WTSP, Hillsborough County woman dies of dengue fever complications (18 Sep) — https://www.wtsp.com/article/news/health/dengue-fever-death-hillsborough-florida/67-17b51105-cc12-4eab-8046-52e7a30a823b
15. Newsweek, map shows dengue fever cases each state as Florida records first 2026 death — https://www.newsweek.com/map-shows-dengue-fever-cases-each-state-as-florida-records-first-2026-death-12466232
16. Outbreak News Today, Bangladesh dengue cases top 70,000 (17 Sep) — https://outbreaknewstoday.substack.com/p/bangladesh-dengue-cases-top-70000
17. Deccan Herald, Bangladesh sees worst single-day surge in dengue cases and deaths this year — https://www.deccanherald.com/world/bangladesh-sees-worst-single-day-surge-in-dengue-cases-and-deaths-this-year-3738118
18. PAHO/WHO, Dengue Epidemiological Situation, Region of the Americas, Epidemiological Week 35 2026 — https://www.paho.org/en/documents/dengue-epidemiological-situation-region-americas-epidemiological-week-35-2026
19. Newswire.lk, Sri Lanka dengue cases surpass 96,000 as deaths reach 72 (4 Sep) — https://www.newswire.lk/2026/09/04/sri-lanka-dengue-cases-surpass-96000-as-deaths-reach-72/
20. Lanka Newspapers, dengue crisis deepens: Sri Lanka reports alarming case numbers as of late September 2026 (23 Sep) — https://www.lankanewspapers.com/2026/09/23/dengue-crisis-deepens-sri-lanka-reports-alarming-case-numbers-as-of-late-september-2026
21. Tribune.net.ph, Aurora dengue cases surge 137% to 2,172 (23 Sep) — https://tribune.net.ph/2026/09/23/aurora-dengue-cases-surge-137-to-2172
22. PLOS Neglected Tropical Diseases, advancing outbreak detection: hybridizing machine learning with wavelets for weekly dengue case forecasting (9 Jul 2026) — https://journals.plos.org/plosntds/article?id=10.1371%2Fjournal.pntd.0014444
23. Nature Reviews Microbiology, impacts of climate change on dengue (Sep 2026) — https://www.nature.com/articles/s41579-026-01329-4
24. Viruses (MDPI), methodological approaches to dengue virus detection in wastewater: a systematic review and meta-analysis of positivity rate (30 Apr 2026) — https://doi.org/10.3390/v18050531
25. Journal of Travel Medicine, shared evidence, different recommendations: a comparative analysis of Qdenga (TAK-003) dengue vaccine guidance for travellers across countries (22 Jul 2026) — https://doi.org/10.1093/jtm/taag065
