# GDO Internal News Report — 2026-11-16

*Source: Global Dengue Observatory (accessed 2026-11-16).*

Snapshot folder: `snapshots/2026_11_09` (news-only week — unchanged since the
2026-11-04 render; next render expected 2026-11-18). Upstream data vintage:
`Output/2026_11_04` from `DENV_global_observatory`, commit
`1d039b61e627d5ffacb39b390774056bce303acb`. 85 countries/territories tracked.

---

## 1. This week's snapshot

No new GDO render has happened since last week's report, so the underlying
numbers below are identical to the 2026-11-09 pull. Across the 85 tracked
countries, the current-season severity picture splits:

| Current-season severity | Countries |
|---|---|
| Extremely High | 5 |
| High | 10 |
| Normal | 27 |
| Low | 30 |
| Extremely Low | 7 |
| Unknown | 6 |

(Cumulative-season severity, a slightly different cut, runs 10 Extremely
High / 13 High / 28 Normal / 23 Low / 5 Extremely Low / 6 Unknown.)

The five countries sitting at **Extremely High** on the current-season read
are Cuba (100th percentile), Kenya (100th), Cambodia (99.9th), Sudan (95.9th)
and Peru (95.7th). Regionally, the tracked set is heavily Caribbean (21
countries) and Pacific Islands (15), with South America (13), Sub-Saharan
Africa (10), East & Southeast Asia (9), North & Central America (8) and South
Asia (8) also represented; Europe/Middle East/North Africa has just one
tracked country (Sudan) in this dataset.

---

## 2. News — targeted (countries flagged by the active snapshot's data move)

The active `movers.csv` (unchanged from last week, since no new pull has
happened) flags 16 country-rows that moved category at the last data
refresh: A = severity-band change, B = monthly-ratio-descriptor change, C =
large current-season-percentile swing. That's more than 10, so per the
targeting rule we prioritised the 6 A/B band-crossings, then filled the
remaining 4 slots with the largest C percentile swings (Peru, Fiji,
Afghanistan, Sudan). The other 5 C movers (Australia, United States,
Mauritania, Senegal, Viet Nam) didn't get a dedicated write-up this week;
they're in the full table in the appendix. News below is a fresh search as
of today, not a repeat of last week's pass.

### Bolivia (A: severity band)
GDO: cumulative severity has reached "Rare bad event — unusually high cases
to date" (percentile 99.5), up from "Above average" at the last pull.
Current-season read remains comparatively mild — Normal band, 47th
percentile — with a monthly ratio of 2.48, running well above the seasonal
baseline (1,499 observed cases against an expected ~604). Estimated season
total: 101,738 cases.
*Caveat: latest observed month is September 2026 — a ~2.5-month gap, at the
outer edge of GDO's 1–2 month nowcast sweet spot.*
News context: PAHO's regional situation report through epidemiological week
39 (to 23 October) shows Bolivia's case count up 25% versus the preceding
four-week period — one of the larger regional increases, alongside Peru
(+41%). A 1 October PAHO item notes Bolivia has stood up two national
laboratory networks to strengthen arbovirus surveillance. Separate reporting
describes a rising case count in an Amazonian department. No
November-specific national total surfaced, consistent with GDO's own
~2.5-month-old observed data.
Sources: [PAHO — dengue situation report, epi week 39](https://www.paho.org/sites/default/files/2026/10/2026-cde-dengue-sitrep-americas-epi-week-39-oct.pdf); [Prensa Latina — Bolivia registra incremento de dengue en departamento amazónico](https://www.prensa-latina.cu/?p=880846); [PAHO — Bolivia articula dos redes nacionales de laboratorios](https://www.paho.org/es/noticias/1-10-2026-bolivia-articula-dos-redes-nacionales-laboratorios-para-fortalecer-vigilancia-0).

### Honduras (A: severity band)
GDO: cumulative severity moved from "Below average" to "Average — typical
case load" (percentile 25.2). Current-season read: Low, 20th percentile;
monthly ratio 0.25, running well below the seasonal baseline (1,166 observed
cases against an expected ~4,658). Estimated season total: 13,985.
*Caveat: latest observed month is September 2026 (~2.5-month gap) — outside
the tightest nowcast window.*
News context: Honduras's health secretariat (Sesal) put the 2026 cumulative
total at 13,939 cases as of 10 November, with 944 new cases in the latest
epidemiological week alone — a 32.2% rise on the prior week. Of that total,
3,407 cases carry warning signs and 263 are classified severe; one outlet
projects the year could close near 19,300 cases if the recent weekly pace
holds. Five deaths from severe dengue are reported for 2026, with another
under investigation. PAHO/Sesal data place Honduras second in Central
America for case counts this year, even though the national count had been
running below the five-year average earlier in 2026.
Sources: [La Tribuna — Honduras supera los 12 mil casos de dengue en lo que va de 2026](https://www.latribuna.hn/2026/11/02/honduras-supera-los-12-mil-casos-de-dengue-en-lo-que-va-de-2026/); [La Prensa — dengue en Honduras, reportan 944 nuevos contagios en una semana](https://www.laprensa.hn/honduras/dengue-honduras-reportan-944-nuevos-contagios-semana-LH32603594); [La Tribuna — Honduras reporta cinco muertes por dengue grave en 2026](https://www.latribuna.hn/2026/10/13/honduras-reporta-cinco-muertes-por-dengue-grave-en-2026-e-investiga-otro-fallecimiento/).

### Mexico (A: severity band)
GDO: cumulative severity stepped down from "Average" to "Below average"
(percentile 21.8, Low band). Current-season read also Low (15.1th
percentile); monthly ratio 0.13 — running well below baseline (4,198
observed cases against an expected ~33,002). Estimated season total: 73,654.
*Latest observed month is October 2026 — within GDO's nowcast sweet spot,
one of the fresher reads this week.*
News context: a KJZZ report dated 10 November names Sonora as the Mexican
state with the most dengue cases this year (over 2,000 cases in 2026, more
than 100 in the two weeks before publication in Hermosillo alone) — a
persistent, border-adjacent hotspot even as the national picture eases.
Separately, Yucatán media reported on 9 November that a "dangerous serotype"
had been confirmed circulating across 26 municipalities. One undated
Excélsior report cites a national total of 4,152 cases; given the dating
uncertainty, that figure should be treated cautiously rather than as a
current count. The pattern — a mild national trend with a sharp, localised
exception — is consistent with GDO's cumulative read (nationally below
average) alongside the Sonora hotspot.
Sources: [KJZZ — Sonora has Mexico's highest 2026 dengue cases](https://www.kjzz.org/fronteras-desk/2026-11-10/just-across-the-border-from-arizona-sonora-has-mexicos-highest-2026-dengue-cases); [Diario de Yucatán — boom de dengue en Yucatán, confirman serotipo peligroso en 26 municipios](https://www.yucatan.com.mx/merida/2026/11/09/boom-de-dengue-en-yucatan-confirman-un-peligroso-serotipo-en-26-municipios.html).

### Brazil (B: monthly-ratio descriptor)
GDO: the monthly-ratio descriptor has flipped from "running well above" to
"running well below" (ratio 0.66; cumulative percentile 42, Normal band).
Current-season read: Low, 7.6th percentile. 26,999 observed cases against an
expected ~40,791 for the month. Estimated season total: 1,083,015 — by far
the largest in this week's list, reflecting Brazil's scale.
*Latest observed month is October 2026 — within the nowcast sweet spot. A
swing from well-above to well-below in one pull is a large directional
change for a country this size; worth flagging rather than over-reading as
a single clean trend.*
News context: Brazilian outlets reported on 11 November that the Instituto
Todos pela Saúde counted more than 374,000 cases and 371 deaths from January
through October 2026 — a far milder year than 2025, consistent with GDO's
"well below" read. The same reporting flagged a rise in DENV-2/3 serotype
share (from roughly 14% in 2025 to about 30% in 2026), raising reinfection
concerns heading into next season. Looking ahead, an IMDC expert projection
published 6 November estimates up to 860,000 probable cases for 2027,
expecting a pattern similar to 2025–2026 despite a possible strong El Niño,
with a peak around April.
Sources: [Agência Brasil via acessa.com — especialistas alertam para risco de reinfecção da dengue](https://www.acessa.com/noticias/2026/11/amp/343964-especialistas-alertam-para-risco-de-reinfeccao-da-dengue.html); [Diário de Pernambuco — dengue pode chegar a 860 mil casos prováveis em 2027](https://www.diariodepernambuco.com.br/brasil/2026/11/11728512-dengue-pais-pode-chegar-a-860-mil-casos-provaveis-da-doenca-em-2027.html).

### Colombia (B: monthly-ratio descriptor)
GDO: descriptor moved from "tracking near" to "running slightly below"
(ratio 0.87; cumulative percentile 62, Normal). Current-season read also
Normal, 51st percentile. 6,149 observed cases against an expected ~7,078.
Estimated season total: 112,504.
*Latest observed month is October 2026 — within the nowcast sweet spot.*
News context: Noticias RCN, citing Colombia's Instituto Nacional de Salud,
reported 97,894 cumulative cases and 65 confirmed deaths for 2026 (three
more under investigation) as of week 43 (around 6 November) — approaching
100,000 for the year, with Barranquilla/Atlántico the most heavily affected
area (7,000+ cases). This cumulative year-to-date total doesn't contradict
GDO's "slightly below" monthly read: the two describe different timeframes
(full-year running total versus the latest single month's ratio to
baseline). Separately, Colombia's meteorological agency (IDEAM) officially
declared El Niño on 8 October, putting the probability it remains strong to
very strong through Q1 2027 at 83% — a forward-looking risk flag worth
watching into the new year.
Sources: [Noticias RCN — Colombia se acerca a los 100.000 casos de dengue en 2026](https://www.noticiasrcn.com/salud-y-bienestar/dengue-colombia-casos-muertes-recomendaciones-1079432); [Diario del Sur — El Niño aumenta la alerta por dengue en Colombia](https://diariodelsur.com.co/noticias/el-nino-aumenta-la-alerta-por-dengue-y-expertos-piden-prevenir-antes-del-verano).

### Guyana (B: monthly-ratio descriptor)
GDO: descriptor has intensified from "running slightly above" to "running
well above" (ratio 4.83; cumulative percentile 99.2, "Rare bad event").
Current-season read: Low, 5.9th percentile — a sign the current season
hasn't yet caught up to the cumulative picture. 4,977 observed cases against
an expected ~1,031. Estimated season total: 94,175.
*Caveat: latest observed month is September 2026 (~2.5-month gap). This move
remains thinly corroborated by fresh reporting.*
News context: Guyana-specific November reporting was again hard to isolate
from older/republished figures and from French Guiana (a different
territory with similarly-worded search results). A Nation News item dated
22 April 2026 cites 2,169 confirmed cases and 11 deaths year-to-date with a
technical working group activated — but near-identical figures also appear
in 2023 Kaieteur News coverage, so that date/figure pairing should be read
with caution rather than relied on as a 2026 data point. The clearest
regional signal is PAHO's mid-September note that Caribbean subregion cases
were rising as part of a roughly 1.69 million-case regional total, with all
four dengue serotypes circulating in the Americas this year. As last week,
this GDO move stays largely uncorroborated by country-specific news — worth
another look once clearer reporting surfaces.
Source: [Caribbean National Weekly, via PAHO — PAHO urges Caribbean to prepare for possible rise in dengue, chikungunya](https://www.caribbeannationalweekly.com/posts/paho-urges-caribbean-to-prepare-for-possible-rise-in-dengue-chikungunya).

### Peru (C: current-season percentile swing)
GDO: current-season percentile stands at 95.7 (Extremely High), up from
49.1 at the last pull — the largest percentile swing in this week's data.
Monthly ratio 5.40, running well above baseline (11,651 observed cases
against an expected ~2,156). Cumulative percentile 99.9 ("Rare bad event").
Estimated season total: 428,297.
*Latest observed month is October 2026 — within the nowcast sweet spot, and
the baseline (~2,156 cases/month expected) isn't tiny, so the ratio reflects
a genuine surge rather than a small-denominator artefact.*
News context: Forbes Perú (6 November) reports 82,554 cases through 24
October — 153% above the same point in 2025 — alongside 91 confirmed dengue
deaths this year, a toll the Ministry of Health links to unusually high
El Niño-driven temperatures. A Latin Times figure for a few days earlier
(78,912 cases through 23 October, +122% on 2025) differs slightly, likely
reflecting different cut-off dates; both point the same direction. Peru's
national epidemiology centre (CDC Perú) has warned that the 2026–2027 El
Niño could drive a second wave via flooding and heavy rain. A 9 November
regional report cites a 700% year-on-year increase in one area (La
Esperanza/Trujillo/El Porvenir), though the underlying measure isn't
specified — flagged for context, not as a verified figure.
Sources: [Forbes Perú — Perú registra 91 muertes por dengue en 2026 y los casos crecen un 153% frente a 2025](https://forbes.pe/actualidad/2026-11-06/peru-registra-91-muertes-por-dengue-en-2026-y-los-casos-crecen-un-153-frente-a-2025/); [Latin Times — Peru dengue cases, El Niño second wave](https://www.latintimes.com/peru-dengue-cases-el-nino-second-wave-600565).

### Fiji (C: current-season percentile swing)
GDO: current-season percentile has risen to 36.3 (still Normal band), from
1.5 at the last pull. Monthly ratio 0.56 — running well below baseline (199
observed cases against an expected ~359). Cumulative percentile 59, Normal.
Estimated season total: 7,222.
*Caveat: latest observed month is August 2026 — a 3-month-plus gap, outside
GDO's nowcast sweet spot. The prior reading (1.5th percentile) was near the
floor, so a large proportional jump off a near-zero base looks dramatic even
though the destination — "Normal" — is unremarkable.*
News context: no Fiji-specific November 2026 case count surfaced in this
pass; the clearest documented figures were a 2025-season total (11,599
confirmed cases, per an IFRC health-security brief) and a Fijivillage report
of 1,090 confirmed cases for a Central Division outbreak, dated March 2026
but matching a March 2025 figure in another source — flagged as unverified
rather than relied upon. Fiji's health officials have previously said case
numbers tend to rise with the November–April rains, which fits the
direction of this GDO move even without a fresh corroborating count. For
regional contrast (a different territory, not in this dataset), New
Caledonia has logged 640+ probable/confirmed cases in 2026 and is under a
DENV-1 red alert.
Source: [Fiji Global News — New Caledonia faces dengue epidemic as DENV-1 red alert drives intensified vector control](https://fijiglobalnews.com/new-caledonia-faces-dengue-epidemic-as-denv-1-red-alert-drives-intensified-vector-control/).

### Afghanistan (C: current-season percentile swing)
GDO: current-season percentile has risen to 76.1 (High), from 45.3 at the
last pull. Monthly ratio 1.02 — tracking near baseline (272 observed cases
against an expected ~265). Cumulative percentile 82.4, "Above average".
Estimated season total: 6,758.
*Caveat: latest observed month is August 2026 (~3-month gap) — outside the
nowcast sweet spot, and the baseline here (~265 cases/month) is modest, so
the percentile climb should be read cautiously.*
News context: as last week, no Afghanistan-specific dengue reporting dated
to November 2026 surfaced. The WHO/EMRO and news results returned are
explicitly dated November–December 2025 (Nangarhar province: 1,000+
suspected cases that month, +7.7% on the prior week; national total 2,357
suspected cases, +21.9% on October; year-to-date 4,384 cases from six
provinces as of 8 November 2025; cases then fell 85.6% in December 2025).
Those figures describe last year's season, not this one, and are included
here only as seasonal/contextual background — not as evidence of a current
2026 surge. Flagging this gap explicitly, since GDO's own Afghanistan read
is itself ~3 months stale this week.
Source: [Tribune India — WHO reports significant rise in suspected dengue cases in eastern Afghanistan](https://www.tribuneindia.com/news/world/who-reports-significant-rise-in-suspected-dengue-cases-in-eastern-afghanistan) (2025 reporting, included for seasonal context only).

### Sudan (C: current-season percentile swing)
GDO: current-season percentile has risen to 95.9 (Extremely High), from
72.6 at the last pull. Monthly ratio 1.52, running well above baseline
(2,636 observed cases against an expected ~1,735). Cumulative percentile
94.5, "Above average". Estimated season total: 45,861.
*Caveat: latest observed month is September 2026 (~2.5-month gap). Sudan's
ongoing conflict is a known confounder for surveillance completeness — treat
this percentile as a plausible floor rather than a precise read, since
disrupted health infrastructure is more likely to mean under-counting than
over-counting.*
News context: Sudan Tribune carried several November 2026 datelined items
(2, 3, 7 and 10 November), though case-count detail did not surface fully in
this search pass. One report of uncertain date describes a decline in
Sennar state, with 3,259 infections and 16 deaths recorded since July.
WHO's August 2026 Sudan Health Spotlight put the cumulative national count
at 85,782 cases and 180 deaths across weeks 31/2024–34/2026, with Blue Nile
accounting for roughly 91% of August cases alone. North Darfur's Tawila
displacement camp had logged 500+ cases by mid-October. The throughline,
unchanged from last week, is conflict-damaged health infrastructure
compounding an already severe season.
Sources: [Sudan Tribune — 10 November 2026](https://sudantribune.com/article/315148); [WHO EMRO — Sudan Health Spotlight, August 2026](https://www.emro.who.int/images/stories/sudan/Sudan-Health-Spotlight-August-2026.pdf); [Darfur24 — dengue cases in Tawila, North Darfur](https://darfur24.com/?p=69150).

---

## 3. News — general scan

Independent broad scan, capped at 5 items, explicitly including
non-endemic/no-GDO-data geographies.

- **Bangladesh** — WHO's South-East Asia bulletin reports 6,063 patients
  hospitalised with dengue as of 8 November, with 3 more deaths in the prior
  24 hours; October was the deadliest month of the year, and one quoted
  entomologist expects no significant easing before December. (GDO itself
  has Bangladesh at High/84.95th-percentile current-season, "running well
  above" — see §5.)
  [Source](https://arynews.tv/bangladesh-death-toll-from-dengue-rises-unlikely-to-ease-before-december).
- **Americas (PAHO)** — PAHO situation reporting continues to track a large,
  multi-country dengue year across the region (1,845,488 suspected cases by
  epidemiological week 40, cumulative incidence 283 per 100,000). Figures on
  the regional emergency level varied across sources in this search and
  weren't independently confirmed — treat the specific case total as PAHO's
  reported figure, not GDO's.
  [Source](https://www.paho.org/sites/default/files/2026/10/2026-cde-dengue-sitrep-americas-epi-week-40-oct.pdf).
- **India** — TravelHealthPro, citing WHO data, puts India's 2026 cumulative
  case count at 70,140 as of 19 October — a non-targeted country this week,
  but a large absolute burden worth tracking.
  [Source](https://travelhealthpro.org.uk/updates.php?base=5021).
- **United States (Hawaii, non-endemic)** — Hawaii's Department of Health
  confirmed an 11th travel-related dengue case on 5 November; no local
  transmission reported.
  [Source](https://www.hawaiinewsnow.com/2026/11/05/dept-health-confirms-11th-travel-related-dengue-case-hawaii/).
- **Europe (imported and limited local cases, non-endemic)** — Spain's
  national Aedes-borne disease surveillance report counted 232 cases with a
  known exposure country through week 39 (to 27 September), 35% of them
  (81 cases) imported from the Maldives, with Cuba-linked cases reappearing
  from week 27. France identified 261 imported cases between 1 May and 26
  July, alongside two locally-acquired cases in the Tarn and Hérault
  départements as of 20 July; Italy has also reported a small number of
  locally-acquired cases this year. Risk of onward spread in mainland Europe
  after a traveller-imported case is still considered low given current
  conditions.
  [Source](https://www.mesvaccins.net/web/news/23998-plusieurs-pays-europeens-signalent-une-augmentation-du-nombre-de-cas-de-dengue-importes-lies-a-des-voyages-aux-maldives).

---

## 4. Trend since last update

No new GDO data this week. This is a **news-only week**: the active
snapshot (`snapshots/2026_11_09`, vintage 2026-11-04) is unchanged from last
week's report, so there are no fresh category A/B/C moves to report against
it — the next render is expected 2026-11-18. The movers file behind §2 is
identical to the one used in last week's report and is reproduced in full in
the appendix for reference.

---

## 5. Social-media candidate flags

Ranked short-list, with caveats carried over from §2.

1. **Peru** — Extremely High current-season band (95.7th percentile), the
   largest percentile swing of any tracked country this pull, corroborated
   by fresh reporting of a 153% year-on-year case rise and 91 deaths, plus
   an official CDC Perú alert naming El Niño as a second-wave risk. *Caveat:
   among the more reliable reads this week — within the 1–2 month nowcast
   window, not a small-baseline artefact — good candidate to lead with.*
2. **Bangladesh** — High band (84.95th percentile, "running well above"),
   corroborated by WHO's report of record October hospitalisations and
   continuing deaths into November. *Caveat: GDO's own Bangladesh read is
   ~2.5 months old (observed September); the October/November figures come
   from WHO/press reporting, not from the GDO file itself — keep that
   sourcing distinction clear in any post.*
3. **Sudan** — Extremely High band (95.9th percentile), set against a
   conflict-disrupted health system and fresh November Sudan Tribune
   coverage. *Caveat: likely an under-count given surveillance disruption —
   frame as "at least this severe," not a precise figure; observed month is
   ~2.5 months stale.*
4. **Bolivia** — cumulative severity at "Rare bad event" (99.5th
   percentile), corroborated by PAHO's report of a 25% four-week case rise
   and new investment in laboratory surveillance. *Caveat: current-season
   read is still Normal (47th percentile) — don't overstate immediacy;
   observed month is ~2.5 months stale.*
5. **Honduras** — crossed into the "Average" severity band (A mover), with
   the cleanest, most recent news corroboration of the week (Sesal data
   through 10 November, +32.2% week-over-week, on pace for a record year).
   *Caveat: GDO's own current-season read is still Low (20th percentile) —
   the news trend is sharper than GDO's current-season classification
   suggests; a genuine within-year acceleration, not yet a top-band severity
   story.*

---

## 6. Scientific literature findings

Light pass, dengue forecasting/surveillance/climate/vaccine-policy methods:

- A Bayesian spatio-temporal nowcasting framework (Xiao & Moraga, EGU 2026
  abstract) uses a flexible reporting-delay structure, implemented in
  `inlabru` for speed, and beat a baseline model in 22 of 26 Brazilian
  states in a 2025 validation exercise.
  [Source](https://meetingorganizer.copernicus.org/EGU26/EGU26-4713.html?pdf).
- Tran et al. (medRxiv, July 2026) applied NobBS, a Bayesian nowcasting
  method, to the 2024 Puerto Rico dengue outbreak; it accurately captured
  the epidemic trajectory and generally outperformed a baseline, though
  reporting anomalies and more variable reporting delays reduced
  performance and raised uncertainty in some periods.
  [Source](https://www.networkscienceinstitute.org/publications/lessons-learned-from-real-time-nowcasting-the-2024-dengue-outbreak-in-puerto-rico).
- A large multi-country analysis in Lancet Planetary Health (2026) across
  21 countries and 1,237 locations (2000–2019) found strong associations
  between ENSO and dengue risk, with the share attributable to
  human-caused climate change varying by geography.
  [Source](https://econpapers.repec.org/RePEc:plo:pgph00:0006405).
- PAHO published updated Americas dengue-vaccine recommendations in
  November 2026, backing Takeda's TAK-003 (Qdenga) and advising it be given
  separately from other vaccines (especially live-attenuated ones) for
  cleaner safety monitoring; PAHO is awaiting consolidated
  safety/pharmacovigilance evidence on Brazil's Butantan-DV vaccine, which
  Brazil suspended in June 2026 pending a safety investigation.
  [Source](https://www.paho.org/sites/default/files/2026/11/recommendations-use-dengue-vaccine-region-americas-2026.pdf).
- A 2026 commentary (citing a Nature Communications analysis of 57
  countries) estimates El Niño-linked temperature changes explain roughly
  63% of year-to-year variation in dengue cases, with about a 48% case
  increase per 1°C rise in a key Pacific temperature index. *Caveat: this
  is a secondary citation via commentary rather than the primary paper —
  worth confirming against the original source before using externally.*
  [Source](https://codeblue.galencentre.org/?p=74912).

---

## 7. Appendix

### 7.1 Full movers table (`snapshots/2026_11_09/movers.csv`, unchanged from last week)

| iso3 | country | region | category | field | prior value | current value | delta |
|---|---|---|---|---|---|---|---|
| BOL | Bolivia | South America | A | severity_interpretation | Above average - more cases than typical at this point | Rare bad event - unusually high cases to date | — |
| HND | Honduras | North & Central America | A | severity_interpretation | Below average - fewer cases than typical at this point | Average - typical case load at this point | — |
| MEX | Mexico | North & Central America | A | severity_interpretation | Average - typical case load at this point | Below average - fewer cases than typical at this point | — |
| BRA | Brazil | South America | B | monthly_ratio_descriptor | running well above | running well below | — |
| COL | Colombia | South America | B | monthly_ratio_descriptor | tracking near | running slightly below | — |
| GUY | Guyana | South America | B | monthly_ratio_descriptor | running slightly above | running well above | — |
| PER | Peru | South America | C | current_season_percentile | 49.1 | 95.7 | +46.57 |
| BOL | Bolivia | South America | C | current_season_percentile | 7 | 47 | +40.07 |
| FJI | Fiji | Pacific Islands | C | current_season_percentile | 1.5 | 36.3 | +34.81 |
| AFG | Afghanistan | South Asia | C | current_season_percentile | 45.3 | 76.1 | +30.78 |
| SDN | Sudan | Europe, Middle East & North Africa | C | current_season_percentile | 72.6 | 95.9 | +23.36 |
| AUS | Australia | Pacific Islands | C | current_season_percentile | 0 | 21.9 | +21.94 |
| USA | United States Of America | North & Central America | C | current_season_percentile | 58.5 | 78.5 | +20.07 |
| MRT | Mauritania | Sub-Saharan Africa | C | current_season_percentile | 72.5 | 91.7 | +19.20 |
| SEN | Senegal | Sub-Saharan Africa | C | current_season_percentile | 62.1 | 80.6 | +18.55 |
| VNM | Viet Nam | East & Southeast Asia | C | current_season_percentile | 49 | 65 | +15.95 |

### 7.2 Consolidated citation list

**Targeted news (§2):**
- [PAHO — dengue situation report, epi week 39](https://www.paho.org/sites/default/files/2026/10/2026-cde-dengue-sitrep-americas-epi-week-39-oct.pdf)
- [Prensa Latina — Bolivia registra incremento de dengue en departamento amazónico](https://www.prensa-latina.cu/?p=880846)
- [PAHO — Bolivia articula dos redes nacionales de laboratorios](https://www.paho.org/es/noticias/1-10-2026-bolivia-articula-dos-redes-nacionales-laboratorios-para-fortalecer-vigilancia-0)
- [La Tribuna — Honduras supera los 12 mil casos de dengue en lo que va de 2026](https://www.latribuna.hn/2026/11/02/honduras-supera-los-12-mil-casos-de-dengue-en-lo-que-va-de-2026/)
- [La Prensa — dengue en Honduras, reportan 944 nuevos contagios en una semana](https://www.laprensa.hn/honduras/dengue-honduras-reportan-944-nuevos-contagios-semana-LH32603594)
- [La Tribuna — Honduras reporta cinco muertes por dengue grave en 2026](https://www.latribuna.hn/2026/10/13/honduras-reporta-cinco-muertes-por-dengue-grave-en-2026-e-investiga-otro-fallecimiento/)
- [KJZZ — Sonora has Mexico's highest 2026 dengue cases](https://www.kjzz.org/fronteras-desk/2026-11-10/just-across-the-border-from-arizona-sonora-has-mexicos-highest-2026-dengue-cases)
- [Diario de Yucatán — boom de dengue en Yucatán, confirman serotipo peligroso en 26 municipios](https://www.yucatan.com.mx/merida/2026/11/09/boom-de-dengue-en-yucatan-confirman-un-peligroso-serotipo-en-26-municipios.html)
- [Agência Brasil via acessa.com — especialistas alertam para risco de reinfecção da dengue](https://www.acessa.com/noticias/2026/11/amp/343964-especialistas-alertam-para-risco-de-reinfeccao-da-dengue.html)
- [Diário de Pernambuco — dengue pode chegar a 860 mil casos prováveis em 2027](https://www.diariodepernambuco.com.br/brasil/2026/11/11728512-dengue-pais-pode-chegar-a-860-mil-casos-provaveis-da-doenca-em-2027.html)
- [Noticias RCN — Colombia se acerca a los 100.000 casos de dengue en 2026](https://www.noticiasrcn.com/salud-y-bienestar/dengue-colombia-casos-muertes-recomendaciones-1079432)
- [Diario del Sur — El Niño aumenta la alerta por dengue en Colombia](https://diariodelsur.com.co/noticias/el-nino-aumenta-la-alerta-por-dengue-y-expertos-piden-prevenir-antes-del-verano)
- [Caribbean National Weekly, via PAHO — PAHO urges Caribbean to prepare for possible rise in dengue, chikungunya](https://www.caribbeannationalweekly.com/posts/paho-urges-caribbean-to-prepare-for-possible-rise-in-dengue-chikungunya)
- [Forbes Perú — Perú registra 91 muertes por dengue en 2026 y los casos crecen un 153% frente a 2025](https://forbes.pe/actualidad/2026-11-06/peru-registra-91-muertes-por-dengue-en-2026-y-los-casos-crecen-un-153-frente-a-2025/)
- [Latin Times — Peru dengue cases, El Niño second wave](https://www.latintimes.com/peru-dengue-cases-el-nino-second-wave-600565)
- [Fiji Global News — New Caledonia faces dengue epidemic as DENV-1 red alert drives intensified vector control](https://fijiglobalnews.com/new-caledonia-faces-dengue-epidemic-as-denv-1-red-alert-drives-intensified-vector-control/)
- [Tribune India — WHO reports significant rise in suspected dengue cases in eastern Afghanistan (2025 reporting)](https://www.tribuneindia.com/news/world/who-reports-significant-rise-in-suspected-dengue-cases-in-eastern-afghanistan)
- [Sudan Tribune — 10 November 2026](https://sudantribune.com/article/315148)
- [WHO EMRO — Sudan Health Spotlight, August 2026](https://www.emro.who.int/images/stories/sudan/Sudan-Health-Spotlight-August-2026.pdf)
- [Darfur24 — dengue cases in Tawila, North Darfur](https://darfur24.com/?p=69150)

**General scan (§3):**
- [ARY News — Bangladesh death toll from dengue rises, unlikely to ease before December](https://arynews.tv/bangladesh-death-toll-from-dengue-rises-unlikely-to-ease-before-december)
- [PAHO — dengue situation report, epi week 40](https://www.paho.org/sites/default/files/2026/10/2026-cde-dengue-sitrep-americas-epi-week-40-oct.pdf)
- [TravelHealthPro — India dengue outbreak update](https://travelhealthpro.org.uk/updates.php?base=5021)
- [Hawaii News Now — Dept. of Health confirms 11th travel-related dengue case in Hawaii](https://www.hawaiinewsnow.com/2026/11/05/dept-health-confirms-11th-travel-related-dengue-case-hawaii/)
- [Mesvaccins.net — plusieurs pays européens signalent une augmentation du nombre de cas de dengue importés, liés à des voyages aux Maldives](https://www.mesvaccins.net/web/news/23998-plusieurs-pays-europeens-signalent-une-augmentation-du-nombre-de-cas-de-dengue-importes-lies-a-des-voyages-aux-maldives)

**Scientific literature (§6):**
- [EGU26 abstract — Xiao & Moraga, Bayesian spatio-temporal nowcasting](https://meetingorganizer.copernicus.org/EGU26/EGU26-4713.html?pdf)
- [Network Science Institute — lessons learned from real-time nowcasting, Puerto Rico 2024](https://www.networkscienceinstitute.org/publications/lessons-learned-from-real-time-nowcasting-the-2024-dengue-outbreak-in-puerto-rico)
- [EconPapers/Lancet Planetary Health — ENSO and dengue risk across 21 countries](https://econpapers.repec.org/RePEc:plo:pgph00:0006405)
- [PAHO — recommendations for the use of dengue vaccine in the Region of the Americas, 2026](https://www.paho.org/sites/default/files/2026/11/recommendations-use-dengue-vaccine-region-americas-2026.pdf)
- [CodeBlue — the 2026 El Niño phenomenon and its impact on dengue outbreaks](https://codeblue.galencentre.org/?p=74912)
