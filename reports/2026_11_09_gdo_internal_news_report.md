# GDO Internal News Report — 2026-11-09

*Source: Global Dengue Observatory (accessed 2026-11-09).*

Snapshot folder: `snapshots/2026_11_09` (pull week — new render). Upstream data
vintage: `Output/2026_11_04` from `DENV_global_observatory`, commit
`1d039b61e627d5ffacb39b390774056bce303acb`. Prior snapshot for comparison:
`snapshots/2026_10_19` (vintage `2026-10-18`). 85 countries/territories
tracked.

---

## 1. This week's snapshot

Across the 85 tracked countries, the current-season severity picture splits:

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
are Cuba (100th percentile), Kenya (100th), Cambodia (99.9th), Peru (95.7th)
and Sudan (95.9th). Worth flagging: Cuba and Kenya aren't new to this list —
neither shows up in this week's movers file, which means they were already
at this level last pull and have simply stayed there. Peru and Sudan, by
contrast, are new arrivals this week (more in §2 below).

Regionally, the tracked set is heavily Caribbean (21 countries) and Pacific
Islands (15), with South America (13), Sub-Saharan Africa (10), East &
Southeast Asia (9), North & Central America (8) and South Asia (8) all
represented; Europe/Middle East/North Africa has just one tracked country
(Sudan) in this dataset.

---

## 2. News — targeted (countries flagged by this week's data move)

16 country-rows moved category this week (A = severity-band change, B =
monthly-ratio-descriptor change, C = large current-season-percentile swing).
That's more than 10, so per the targeting rule we prioritised the 6 A/B
band-crossings, then filled the remaining 4 slots with the largest C
percentile swings (Peru, Fiji, Afghanistan, Sudan — ranked by swing size).
The other 5 C movers (Australia, United States, Mauritania, Senegal, Viet
Nam) didn't make the cut for a dedicated write-up this week; they're in the
full table in the appendix.

### Bolivia (A: severity band)
GDO: cumulative severity has jumped to "Rare bad event — unusually high
cases to date" (percentile 99.5), up from "Above average" last pull.
Current-season read is milder — Normal, 47th percentile — with a monthly
ratio of 2.48, i.e. running well above the seasonal baseline (1,499 observed
cases against an expected ~604). Estimated season total: 101,738 cases.
*Caveat: latest observed month is September 2026 — a ~2-month gap, at the
outer edge of GDO's 1–2 month nowcast sweet spot.*
News context: mid-2026 reporting described a growing Santa Cruz outbreak
(2,700+ cases by late July) that prompted Argentina's northern border
provinces to step up surveillance, and Bolivian health authorities flagged
a rise in cases relative to 2025. Bolivia's main transmission season in the
lowland east typically runs December–March, so November marks the start of
the riskier window — consistent with the cumulative severity reading, even
if no November-specific case count was found in this search.
Sources: [VOA — Bolivia alerta aumento de casos de dengue](https://www.vozdeamerica.com/a/bolivia-alerta-aumento-casos-dengue/6963792.html); [TodoJujuy — dengue en Bolivia y la frontera con Argentina](https://www.todojujuy.com/jujuy/alerta-dengue-bolivia-que-pasa-las-fronteras-que-conectan-jujuy-y-salta-n286384).

### Honduras (A: severity band)
GDO: cumulative severity has moved from "Below average" to "Average —
typical case load" (percentile 25.2, right at the Low/Normal boundary).
Current-season read: Low, 20th percentile; monthly ratio 0.25 — running
well below the seasonal baseline (1,166 observed cases vs. an expected
~4,658). Estimated season total: 13,985.
*Caveat: latest observed month is September 2026 (~2-month gap) — outside
the tightest nowcast window.*
News context: Honduran health-ministry data reported via local outlets put
the 2026 cumulative count at ~12,995 cases through week 43 (adding ~714 in
that week alone), with four dengue deaths confirmed this year. One outlet
projected the year could close near 19,300 cases if the recent weekly pace
holds, and cites PAHO data placing Honduras second in Central America for
case counts this year — even though case numbers earlier in 2026 had been
running well below 2025.
Sources: [El Heraldo — casi 13,000 casos de dengue en 2026](https://www.elheraldo.hn/honduras/salud-registra-casi-13-000-casos-dengue-en-lo-que-va-del-2026-honduras-DH32532089); [La Tribuna — cinco muertes por dengue grave](https://www.latribuna.hn/2026/10/13/honduras-reporta-cinco-muertes-por-dengue-grave-en-2026-e-investiga-otro-fallecimiento/).

### Mexico (A: severity band)
GDO: cumulative severity has stepped down from "Average" to "Below average"
(percentile 21.8, Low band). Current-season read is also Low (15.1th
percentile); monthly ratio 0.13 — running well below baseline (4,198
observed cases vs. an expected ~33,000). Estimated season total: 73,654.
*This is one of the fresher reads this week — latest observed month is
October 2026, close to GDO's 1–2 month sweet spot.*
News context: national reporting (dates not fully confirmed in this search)
puts the 2026 cumulative total in the low thousands with Sonora leading the
state tally, alongside Mexico's health secretary describing a marked
year-on-year decline through mid-2026. Campeche was a local exception,
doubling to 42 cases by late September. No November-specific national total
surfaced in this pass, consistent with the GDO read of a season running
well below its seasonal norm.
Sources: [Excelsior — México acumula casos de dengue en 2026](https://www.excelsior.com.mx/nacional/dengue-mexico-2026); [Por Esto — dengue se duplica en Campeche](https://www.poresto.com/campeche/2026/9/21/dengue-se-duplica-en-campeche-2026-ya-acumula-42-casos.html).

### Brazil (B: monthly-ratio descriptor)
GDO: the monthly-ratio descriptor has flipped from "running well above" to
"running well below" (ratio 0.66; cumulative percentile 42, Normal band).
Current-season read: Low, 7.6th percentile. 26,999 observed cases against an
expected ~40,791 for the month. Estimated season total: 1,083,015 — by far
the largest in this week's list, reflecting Brazil's scale.
*Latest observed month is October 2026 — within the nowcast sweet spot. The
swing from well-above to well-below in one pull is a big directional
change for a country this size; worth flagging rather than over-reading as
a single clean trend, since large-population countries can show reporting
lags that smooth out over subsequent pulls.*
News context: Brazil's Ministry of Health reported a sharp year-on-year
drop in the first third of 2026 (roughly 227,500 probable cases to
mid-April, versus 916,400 over the same period in 2025 — about a 75% fall).
A later, less certain figure put the national 2026 total near 1.5 million
cases and 400 deaths by mid-August. Separately, an InfoDengue-Mosqlimate
modelling study had projected around 1.8 million cases for 2026 nationally,
with the heaviest load expected in São Paulo and Minas Gerais.
Sources: [Carta Capital — queda de casos de dengue no Brasil](https://www.cartacapital.com.br/?p=599680); [Brasil61 — Brasil deve registrar 1,8 milhão de casos de dengue em 2026](https://brasil61.com/n/dengue-2026-brasil-deve-registrar-1-8-milhao-de-casos-com-pico-em-sp-e-mg-bras2616149).

### Colombia (B: monthly-ratio descriptor)
GDO: descriptor moved from "tracking near" to "running slightly below"
(ratio 0.87; cumulative percentile 62, Normal). Current-season read is also
Normal, 51st percentile. 6,149 observed cases against an expected ~7,078.
Estimated season total: 112,504.
*Latest observed month is October 2026 — within the nowcast sweet spot.*
News context: Colombia's Instituto Nacional de Salud reported, as of week
43 (around 6 November), 97,894 cumulative dengue cases and 65 confirmed
deaths for 2026 (plus three deaths still under investigation) — approaching
100,000 for the year. An October update had put the running total at
91,419 cases with 192 municipalities above their expected epidemiological
threshold. Barranquilla/Atlántico and Cesar remain the most heavily
affected areas.
Sources: [Noticias RCN — Colombia se acerca a los 100.000 casos de dengue en 2026](https://www.noticiasrcn.com/salud-y-bienestar/dengue-colombia-casos-muertes-recomendaciones-1079432); [Consultorsalud — mapa territorial de casos de dengue](https://consultorsalud.com/dengue-en-colombia-2026-mapa-territorial-casos/).

### Guyana (B: monthly-ratio descriptor)
GDO: descriptor has intensified from "running slightly above" to "running
well above" (ratio 4.83; cumulative percentile 99.2, "Rare bad event").
Current-season read: Low, 5.9th percentile — a sign the current season
hasn't yet caught up to the cumulative picture. 4,977 observed cases against
an expected ~1,031. Estimated season total: 94,175.
*Caveat: latest observed month is September 2026 (~2-month gap). News
coverage for Guyana specifically (as opposed to French Guiana, a separate
territory that dominates search results under similar terms) was thin in
this pass, so this move is currently GDO-only and not yet corroborated by
fresh reporting — worth another look next week.*
News context: the clearest recent Guyana-specific signal found was from
January 2026, reporting an upsurge in Region Six (East Berbice-Corentyne)
tied to persistent rainfall and vector-breeding conditions — consistent
with the rainy-season driver, but not itself evidence for the current spike.
Source: [iNews Guyana — Region Six dengue upsurge](https://groundnews.lakegeneva.lib.wi.us/article/reg-6-records-surge-in-dengue-cases-amid-rainy-season-rho) (via syndication).

### Peru (C: current-season percentile swing)
GDO: current-season percentile has jumped to 95.7 (Extremely High), from
49.1 at the last pull — the largest percentile swing of any country this
week. Monthly ratio 5.40, running well above baseline (11,651 observed
cases vs. an expected ~2,156). Cumulative percentile is 99.9 ("Rare bad
event"). Estimated season total: 428,297.
*Latest observed month is October 2026 — within the nowcast sweet spot, so
this is one of the more trustworthy reads this week. The baseline (~2,156
cases/month expected) isn't tiny, so the 5.4× ratio reflects a real surge
rather than a small-denominator artefact.*
News context: Peru's national count reached 78,912 cases through 23
October (122% above the same point in 2025), with 72 confirmed deaths and
13 more under investigation. On 21 October, CDC Peru issued an
epidemiological alert warning that the 2026–2027 El Niño phenomenon could
drive a second wave via flooding and heavy rainfall. The health ministry
has pushed its vaccination campaign past 135,000 doses, with 400,000 more
secured for the rest of the year.
Sources: [Azertag — Peru extends health emergency, 73,000+ cases](https://azertag.az/en/xeber/peru_extends_health_emergency_after_registering_73000_cases_of_dengue_fever-2618045); [LatinTimes — Peru dengue cases, El Niño second wave](https://www.latintimes.com/peru-dengue-cases-el-nino-second-wave-600565).

### Fiji (C: current-season percentile swing)
GDO: current-season percentile has risen to 36.3 (still Normal band), from
just 1.5 at the last pull. Monthly ratio 0.56 — running well below baseline
(199 observed cases vs. an expected ~359). Cumulative percentile: 59,
Normal. Estimated season total: 7,222.
*Caveat: latest observed month is August 2026 — a 3-month-plus gap, outside
GDO's nowcast sweet spot, so treat this as indicative rather than current.
Also note the prior reading (1.5th percentile) was right at the floor, so a
large proportional jump off a near-zero base looks dramatic even though the
destination — "Normal" — is unremarkable.*
News context: no Fiji-specific November 2026 reporting surfaced; the
clearest documented Fijian outbreak in the search results was from the 2025
season (8,708 cases nationally, May 2025). Fiji's Ministry of Health has
previously flagged that cases typically rise from November through April
with the rains, which fits the direction of this move even without
corroborating current news. For contrast, neighbouring New Caledonia
(a different territory, not in this dataset) is in an active epidemic
phase with 640+ cases since late March 2026.
Source: [Fiji Global News — New Caledonia dengue epidemic, regional context](https://fijiglobalnews.com/new-caledonia-faces-dengue-epidemic-as-denv-1-red-alert-drives-intensified-vector-control/).

### Afghanistan (C: current-season percentile swing)
GDO: current-season percentile has risen to 76.1 (High), from 45.3 at the
last pull. Monthly ratio 1.02 — tracking near baseline (272 observed cases
vs. an expected ~265). Cumulative percentile: 82.4, "Above average".
Estimated season total: 6,758.
*Caveat: latest observed month is August 2026 (~3-month gap) — outside the
nowcast sweet spot, and the baseline here (~265 cases/month) is modest, so
the percentile climb should be read with some caution.*
News context: no Afghanistan-specific dengue reporting from November 2026
turned up in this search — every relevant result dated to November 2025.
For seasonal/contextual background only (not current evidence): WHO
reported a sharp November 2025 rise in Nangarhar province (1,000+ suspected
cases that month, +8% on October) and a national total of 2,357 cases and
3 deaths that November (+21.9% on October), followed by an 85.6% drop in
December. Flagging this gap explicitly rather than implying it describes
2026.
Source: [Tribune India — WHO reports rise in suspected dengue cases in eastern Afghanistan](https://www.tribuneindia.com/news/world/who-reports-significant-rise-in-suspected-dengue-cases-in-eastern-afghanistan) (2025 reporting, included for seasonal context only).

### Sudan (C: current-season percentile swing)
GDO: current-season percentile has risen to 95.9 (Extremely High), from
72.6 at the last pull. Monthly ratio 1.52, running well above baseline
(2,636 observed cases vs. an expected ~1,735). Cumulative percentile: 94.5,
"Above average". Estimated season total: 45,861.
*Caveat: latest observed month is September 2026 (~2-month gap). Sudan's
ongoing conflict is a known confounder for surveillance completeness —
treat this percentile as a plausible floor rather than a precise read,
since disrupted health infrastructure likely means under-counting rather
than over-counting.*
News context: Sudan Tribune carried fresh items dated 2–3 November 2026,
though without detail surfaced in this search pass. Earlier in the year:
a Blue Nile outbreak (reported July) was linked to 39 deaths and 300+
(later 350) confirmed infections, prompting calls for temporary
inter-state travel limits; North Darfur's Tawila displacement camp
reported 500+ cases by mid-October amid urgent aid appeals; and Khartoum
Bahri reported 1,296 dengue cases in August amid a broader surge that also
included malaria, typhoid and cholera. The throughline across all of these
is conflict-damaged health infrastructure compounding an already severe
season.
Sources: [AllAfrica — Sudan health minister urges vaccination as dengue, malaria spread](https://allafrica.com/stories/202604300005.html); [Darfur24 — dengue cases in Tawila, North Darfur](https://darfur24.com/?p=69150).

---

## 3. News — general scan

Independent broad scan, capped at 5 items, explicitly including
non-endemic/no-GDO-data geographies.

- **Bangladesh** — still climbing: 2,333 new hospital admissions on 8
  November alone, the highest single-day count this year; 461 deaths so far
  in 2026 make it the third-deadliest year since national surveillance began
  in 2000. One expert source expects a turn by mid-November.
  [Source](https://outbreaknewstoday.substack.com/p/bangladesh-dengue-fever-update).
- **Sri Lanka** — 107,829 cases and 81 deaths reported for 2026 as of
  midnight 8 November; a nationwide Dengue Prevention Week is running
  through 14 November across 74 at-risk Medical Officer of Health
  divisions.
  [Source](https://lankanewsweb.net/archives/296483/sri-lankas-dengue-toll-exceeds-107000-health-authorities-step-up-prevention-efforts).
- **Philippines** — Quezon City has logged 7,340 cases from 1 January to 5
  November; Sorsogon's cumulative count (data through early October) stood
  at 3,326 and rising.
  [Source](https://tribune.net.ph/2026/11/08/dengue-cases-in-sorsogon-rise-to-over-3000).
- **United States (Florida)** — the state's largest locally-acquired dengue
  outbreak in decades: 39 new locally-acquired cases in the last week of
  October alone, bringing the total to 524 across 12 counties, concentrated
  in the Tampa Bay area.
  [Source](https://outbreaknewstoday.substack.com/p/dengue-in-florida-locally-acquired-e1e).
- **Europe (imported cases, non-endemic)** — France's enhanced surveillance
  bulletin counted 206 imported dengue cases between 1 May and 5 July 2026,
  with no locally-acquired cases identified in mainland France at that
  point; separately, several European countries reported a rise in imported
  cases linked to travel to the Maldives (46+ cases across at least four
  countries), after the Maldives itself logged 631 confirmed cases in
  January 2026 — well above the same month in the two preceding years.
  [Source](https://www.mesvaccins.net/web/news/23998-plusieurs-pays-europeens-signalent-une-augmentation-du-nombre-de-cas-de-dengue-importes-lies-a-des-voyages-aux-maldives).

---

## 4. Trend since last update

Short summary of this week's 16 category moves (A = severity band, B =
monthly-ratio descriptor, C = large current-season-percentile swing; full
detail in the appendix).

| Category | Count | Countries |
|---|---|---|
| A — severity band change | 3 | Bolivia (↑ to Rare bad event), Honduras (↑ to Normal), Mexico (↓ to Below average) |
| B — monthly-ratio descriptor change | 3 | Brazil (well above → well below), Colombia (tracking near → slightly below), Guyana (slightly above → well above) |
| C — current-season percentile swing | 10 | Peru, Bolivia, Fiji, Afghanistan, Sudan, Australia, United States, Mauritania, Senegal, Viet Nam (all ↑) |

- Net direction this week: skewed toward worsening — 2 of 3 A-moves and 2 of
  3 B-moves point up in severity/ratio; all 10 C-moves are increases.
- Steepest single move: Peru, current-season percentile +46.6 points
  (49.1 → 95.7).
- No country moved down into the C list (i.e., no large current-season
  percentile *drops* this week).

---

## 5. Social-media candidate flags

Ranked short-list, with caveats carried over from §2.

1. **Peru** — current-season percentile jumped to 95.7 (Extremely High),
   with a fresh national case count (78,912 through 23 Oct, +122% on 2025)
   and an official CDC Peru alert naming El Niño as a risk for a second
   wave. *Caveat: among the more reliable reads this week (within the
   1–2 month nowcast window; not a small-baseline artefact) — good
   candidate to lead with.*
2. **Sudan** — current-season percentile at 95.9 (Extremely High), set
   against a conflict-disrupted health system and a string of regional
   outbreak reports (Blue Nile, North Darfur). *Caveat: likely an
   under-count given surveillance disruption — frame as "at least this
   severe," not a precise figure.*
3. **Bolivia** — cumulative severity at "Rare bad event" (99.5th
   percentile) just as the main transmission season (Dec–March) is about to
   begin, with a live Santa Cruz outbreak already drawing a cross-border
   response from Argentina. *Caveat: current-season read is still Normal —
   be careful not to overstate immediacy.*
4. **Guyana** — monthly ratio intensified to "running well above" (4.8×),
   cumulative percentile 99.2. *Caveat: GDO-only signal this week — no
   fresh Guyana-specific news corroboration found; worth flagging as "one
   to watch" rather than leading with it.*
5. **Afghanistan** — current-season percentile climbed to 76 (High).
   *Caveat: weakest candidate of the five — no 2026 news corroboration
   found (only 2025 WHO data), observed month is 3 months stale, and the
   baseline is modest. Consider holding this one back unless fresher
   reporting turns up.*

---

## 6. Scientific literature findings

Light pass, dengue forecasting/surveillance/climate methods:

- A 2026 Yale MPH thesis tests whether well-surveilled, climate-similar
  countries can proxy for nowcasting in data-poor settings; the
  Dominican Republic and Haiti emerged as the strongest such pair in the
  Caribbean. [Source](https://elischolar.library.yale.edu/ysphtdl/2621/).
- A One Health paper (dated October 2026) on ensemble forecasting for
  Brazil and Panama reports error reductions of roughly 20% and 36%
  respectively versus the best single-model alternative.
  [Source](https://www.pnnl.gov/publications/environmental-and-epidemiological-drivers-dengue-forecasting-across-heterogeneous).
- Singapore-based researchers describe an early-warning approach combining
  climate data with circulating-serotype shifts (as a proxy for population
  immunity), reporting improved outbreak prediction up to two months ahead,
  with risk highest under El Niño conditions.
  [Source](https://www.eurekalert.org/news-releases/1110126).
- In Vietnam, the DART machine-learning system is reported to generate
  district-level forecasts up to 12 weeks ahead, and the open-source
  E-Dengue tool is being integrated into routine national surveillance with
  a cluster-randomised trial planned.
- A PLOS Digital Health study on Brazil found that models incorporating
  physicians' search-engine behaviour consistently outperformed other
  approaches across most regions under realistic reporting delays.
  [Source](https://econpapers.repec.org/RePEc:plo:pdig00:0001206).

---

## 7. Appendix

### 7.1 Full movers table (`snapshots/2026_11_09/movers.csv`)

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
- [VOA — Bolivia alerta aumento de casos de dengue](https://www.vozdeamerica.com/a/bolivia-alerta-aumento-casos-dengue/6963792.html)
- [TodoJujuy — dengue en Bolivia y la frontera con Argentina](https://www.todojujuy.com/jujuy/alerta-dengue-bolivia-que-pasa-las-fronteras-que-conectan-jujuy-y-salta-n286384)
- [El Heraldo — casi 13,000 casos de dengue en 2026 (Honduras)](https://www.elheraldo.hn/honduras/salud-registra-casi-13-000-casos-dengue-en-lo-que-va-del-2026-honduras-DH32532089)
- [La Tribuna — Honduras, cinco muertes por dengue grave](https://www.latribuna.hn/2026/10/13/honduras-reporta-cinco-muertes-por-dengue-grave-en-2026-e-investiga-otro-fallecimiento/)
- [Excelsior — México acumula casos de dengue en 2026](https://www.excelsior.com.mx/nacional/dengue-mexico-2026)
- [Por Esto — dengue se duplica en Campeche](https://www.poresto.com/campeche/2026/9/21/dengue-se-duplica-en-campeche-2026-ya-acumula-42-casos.html)
- [Carta Capital — queda de casos de dengue no Brasil](https://www.cartacapital.com.br/?p=599680)
- [Brasil61 — projeção de 1,8 milhão de casos de dengue em 2026](https://brasil61.com/n/dengue-2026-brasil-deve-registrar-1-8-milhao-de-casos-com-pico-em-sp-e-mg-bras2616149)
- [Noticias RCN — Colombia se acerca a los 100.000 casos de dengue en 2026](https://www.noticiasrcn.com/salud-y-bienestar/dengue-colombia-casos-muertes-recomendaciones-1079432)
- [Consultorsalud — mapa territorial de casos de dengue en Colombia](https://consultorsalud.com/dengue-en-colombia-2026-mapa-territorial-casos/)
- [iNews Guyana (via syndication) — Region Six dengue upsurge](https://groundnews.lakegeneva.lib.wi.us/article/reg-6-records-surge-in-dengue-cases-amid-rainy-season-rho)
- [Azertag — Peru extends health emergency after 73,000+ dengue cases](https://azertag.az/en/xeber/peru_extends_health_emergency_after_registering_73000_cases_of_dengue_fever-2618045)
- [LatinTimes — Peru dengue cases, El Niño second wave](https://www.latintimes.com/peru-dengue-cases-el-nino-second-wave-600565)
- [Fiji Global News — New Caledonia dengue epidemic (regional context)](https://fijiglobalnews.com/new-caledonia-faces-dengue-epidemic-as-denv-1-red-alert-drives-intensified-vector-control/)
- [Tribune India — WHO reports rise in suspected dengue cases in eastern Afghanistan (Nov 2025)](https://www.tribuneindia.com/news/world/who-reports-significant-rise-in-suspected-dengue-cases-in-eastern-afghanistan)
- [AllAfrica — Sudan health minister urges vaccination as dengue, malaria spread](https://allafrica.com/stories/202604300005.html)
- [Darfur24 — dengue cases in Tawila, North Darfur](https://darfur24.com/?p=69150)

**General scan (§3):**
- [Outbreak News Today — Bangladesh dengue fever update](https://outbreaknewstoday.substack.com/p/bangladesh-dengue-fever-update)
- [Lanka News Web — Sri Lanka's dengue toll exceeds 107,000](https://lankanewsweb.net/archives/296483/sri-lankas-dengue-toll-exceeds-107000-health-authorities-step-up-prevention-efforts)
- [Tribune (Philippines) — dengue cases in Sorsogon rise to over 3,000](https://tribune.net.ph/2026/11/08/dengue-cases-in-sorsogon-rise-to-over-3000)
- [Outbreak News Today — dengue in Florida, locally acquired cases top 500](https://outbreaknewstoday.substack.com/p/dengue-in-florida-locally-acquired-e1e)
- [Mesvaccins.net — rise in imported dengue cases in Europe linked to travel to the Maldives](https://www.mesvaccins.net/web/news/23998-plusieurs-pays-europeens-signalent-une-augmentation-du-nombre-de-cas-de-dengue-importes-lies-a-des-voyages-aux-maldives)

**Scientific literature (§6):**
- [Yale ysphtdl — Nowcasting dengue cases in poor-surveillance nations](https://elischolar.library.yale.edu/ysphtdl/2621/)
- [PNNL — environmental and epidemiological drivers of dengue forecasting](https://www.pnnl.gov/publications/environmental-and-epidemiological-drivers-dengue-forecasting-across-heterogeneous)
- [EurekAlert — first worldwide dengue early-warning system](https://www.eurekalert.org/news-releases/1110126)
- [EconPapers/PLOS Digital Health — search-behaviour signals for dengue forecasting in Brazil](https://econpapers.repec.org/RePEc:plo:pdig00:0001206)
