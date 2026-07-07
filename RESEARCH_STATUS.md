# Research status

Updated: 2026-07-07.

## Pushed checkpoints
- `95daed5` initial dashboard checkpoint.
- `b4915f7` wave 1 source and synthesis integration.
- `5ea77d1` claim/evidence model.
- `e9cb252` scoring, access and relation schema model.
- `a2171fa` expanded case, procurement and coverage evidence.
- `ee3de90` HTML evidence navigation improvements.
- `99f5ab9` cause-first index.
- `TBD` collection-readiness model for normalized festival-year keys, source inventory and collection backlog.

## Evidence layers now present
- Official source map for festival master, tourism/performance, finance/cost, procurement and case evidence.
- Claim graph and evidence manifest to prevent unsupported causal claims.
- Access-feasibility model for API-key, attachment, dashboard and public-page limits.
- Scoring rubric for cause hypotheses.
- Relation graph schema for public stakeholder and contractor relationships.
- Case evidence for success, failure, mixed outcome, cancellation, climate/site failure, price risk, social-license risk and crowd-risk comparator records.
- Procurement evidence for host/supervisor, procurement agent, lead contractor package, subcontract restriction, bid cancellation/change, booth recruitment and selected vendor records.
- Coverage matrix explaining the 2017-2026 backbone and 2016 nationwide master-data gap.
- Cause-first index for climate/safety, price/booth, traffic/access, content/identity, budget/contract, social-license and data-gap exploration.
- Collection-readiness model for festival-year key normalization, source inventory and staged ingestion tasks.
- MCST annual download-pattern manifest for 2017-2026 candidate ZIP files.
- MCST GET probe confirms downloadable 2017-2026 annual ZIPs with byte sizes and SHA-256 hashes; raw binaries are not committed.
- MCST archive schema probe confirms 2017-2026 annual workbooks and records first-sheet aggregate festival counts before full row normalization.
- MCST 2017-2026 annual workbooks are now extracted into a normalized master-draft with 10,198 festival-year records. Staff names and phone numbers from public sheets are intentionally omitted.
- Lightweight MCST master summaries now provide year, province and festival-type aggregate indexes for dashboard use.
- MCST 2017-2021 legacy `period_raw` strings now have a non-destructive date overlay for 4,475 records. Exact ranges were parsed for 2,357 records and single-day dates for 98 records; ambiguous month/mid-month/tentative strings remain flagged for review.

## Current limitations
- The repository is not yet a complete national archive of every 2016-2026 Korean festival.
- 2016 nationwide master coverage remains unresolved from public sources found so far.
- Public Data Portal and NaraJangteo APIs may require service keys for automated bulk collection.
- Tourism DataLab values are trend/performance signals, not exact gate counts.
- Media-only records remain capped at lower confidence until official reports or notices are attached.
- RFP/procurement documents show planning responsibility and scope, not outcome causality by themselves.

## Next research waves
- Review ambiguous MCST 2017-2021 period strings that remain partial/unparsed after conservative overlay parsing.
- Backfill 2016 through local datasets, MCST selected-festival reports and local-government archives while marking coverage status.
- Join Local Finance 365 cost records to festival-year keys for large disclosed events.
- Expand NaraJangteo contract matching with notice number, agency, date, amount, method and supplier where public.
- Add case pages for top failure/risk clusters: crowding/access, price/merchant, weather/climate, budget inefficiency, content dilution and social-license conflict.
- Add visual relation graph rendering once enough high-confidence public relationships exist.
- Convert collection backlog into machine-executed ingestion when service keys or downloadable files are available.
## Checkpoint: MCST-to-finance/procurement match keys (2026-07-08T01:07:16+09:00)

- Built data/master/mcst-finance-procurement-match-keys.json and .csv for all 10198 MCST master-draft records.
- Join readiness: high 3672, medium 6430, low 96.
- Date windows available for 4030 records; budget values available for 9500 records.
- 2017-2021 overlay dates used for 2455 records.
- Added dashboard section #match-keys to explain how festival identity will be connected to budget, procurement, outsourcing, and result evidence.

## Checkpoint: MCST 2026-2027 benchmark cohort join (2026-07-08T01:23:57+09:00)

- Extracted the official 27-name 2026-2027 cultural-tourism festival cohort from the MCST HWPX press attachment using public UplDownloadFile parameters visible in the official HTML.
- Joined the 27 official names to the 2026 MCST regional festival master: exact 23, fuzzy 2, unmatched 2.
- Updated data/mcst-cultural-tourism-benchmark-2026-2027.json, added .csv, refreshed mcst-cultural-tourism-benchmark-2026-2027.html, and added ULW instrumentation under .omo/ulw-research/20260708-mcst-benchmark-join/.

## Checkpoint: benchmark name-resolution layer (2026-07-08T01:27:22+09:00)

- Added data/mcst-cultural-tourism-benchmark-name-resolution.json and .csv to explain the four non-exact benchmark joins.
- Updated mcst-cultural-tourism-benchmark-2026-2027.html with a name-resolution table so human reviewers can understand why a selected festival may fail exact matching.

## Checkpoint: benchmark risk priority queue (2026-07-08T01:28:56+09:00)

- Built a priority queue for the 27 cultural-tourism benchmark festivals using join ambiguity, budget, previous visitor, and outsourcing signals.
- Added data/benchmark-risk-priority-queue.json, .csv, and enchmark-risk-priority-queue.html.

## Checkpoint: benchmark procurement search queue (2026-07-08T01:33:24+09:00)

- Built a P2 procurement/agency search queue for 7 benchmark festivals.
- Added evidence seeds for Bucheon, Incheon Pentaport, Cheorwon, Suwon, Bupyeong, Dongnae, and Eumseong where public search found initial leads.
- Added guardrail that bid notices are not fault findings until contracts/results/outcomes are joined.

## Checkpoint: procurement source strength (2026-07-08T01:35:18+09:00)

- Classified procurement/agency evidence seeds into official original, official event page, official evaluation result, mirror, and publicity-only source classes.
- Added data/procurement-source-strength-wave1.json, .csv, and procurement-source-strength-wave1.html.

## Checkpoint: procurement original download probe (2026-07-08T01:45:00+09:00)

- Probed official/mirror attachment accessibility for Suwon, Bucheon, Incheon Pentaport, Cheorwon, Bupyeong, and Dongnae benchmark cases.
- Added data/procurement-original-download-probe-wave1.json, .csv, procurement-original-download-probe-wave1.html, and evidence note.

## Checkpoint: governance causal chain (2026-07-08T01:58:00+09:00)

- Added a stricter Level A/B/C/D classification to avoid overclaiming contractor or procurement causality.
- Identified Incheon Pentaport 2019 as the first strong Level A causal-candidate case linking selection dispute, injunction attempt, agreement execution, lineup/communication criticism, and operating-organization structure.
- Added data/festival-governance-causal-chain-wave1.json, .csv, festival-governance-causal-chain-wave1.html, and evidence note.

## Checkpoint: Pentaport 2019 cause dossier (2026-07-08T02:08:00+09:00)

- Built a detailed dossier for Incheon Pentaport 2019 as the first Level A causal-candidate case.
- Separated confirmed governance structure, public selection dispute, court-result reporting, programming/communication critique, ticket-value critique, counter-evidence, and unresolved proof gaps.
- Added data/pentaport-2019-cause-dossier.json, .csv, pentaport-2019-cause-dossier.html, and evidence note.

## Checkpoint: Pentaport 2025 success dossier (2026-07-08T02:19:00+09:00)

- Built a success-side dossier for Incheon Pentaport 2025 using official Incheon visitor/economic/satisfaction data and public operating-detail reports.
- Separated success result, safety/heat response, programming, legacy content, local linkage, and unresolved contractor-attribution gaps.
- Added data/pentaport-2025-success-dossier.json, .csv, pentaport-2025-success-dossier.html, and evidence note.

## Checkpoint: Bucheon Comics 2025 governance dossier (2026-07-08T02:29:00+09:00)

- Built a Level B+ governance/outcome bridge dossier for Bucheon International Comics Festival 2025.
- Connected official KOMACON tender/evaluation pages, public 2025 participation scale, program structure, and 2027 cultural tourism festival selection while preserving contractor-attribution gaps.
- Added data/bucheon-comics-2025-governance-dossier.json, .csv, bucheon-comics-2025-governance-dossier.html, and evidence note.

## Checkpoint: Suwon Hwaseong 2026 pre-event dossier (2026-07-08T02:39:00+09:00)

- Built a pre-event governance/crowd-risk dossier for the 63rd Suwon Hwaseong Cultural Festival.
- Upgraded the 2026 case from mirror-only tender lead to official Suwon evaluation-result disclosure with downloadable PDF attachment.
- Added data/suwon-hwaseong-2026-pre-event-dossier.json, .csv, suwon-hwaseong-2026-pre-event-dossier.html, and evidence note.

## Checkpoint: Cheorwon Ice Trekking 2026 safety/outcome dossier (2026-07-08T02:49:00+09:00)

- Built a winter/nature-dependent festival dossier for Cheorwon Hantangang Ice Trekking 2026.
- Connected 2026 visitor outcome, cultural-tourism-festival selection, official 2024 agency-evaluation disclosure, 2020 weather postponement precedent, and safety/course-operation risk factors.
- Added data/cheorwon-ice-2026-safety-outcome-dossier.json, .csv, cheorwon-ice-2026-safety-outcome-dossier.html, and evidence note.

## Checkpoint: case evidence matrix (2026-07-08T03:00:00+09:00)

- Added a dossier index/evidence matrix so the HTML can be read by cause type: procurement/contractor, demand/crowding, weather/safety, programming, local linkage, or pre-event monitoring.
- Added data/case-evidence-matrix-wave1.json, .csv, case-evidence-matrix-wave1.html, and evidence note.

## Checkpoint: Bupyeong/Dongnae procurement gap dossier (2026-07-08T03:12:00+09:00)

- Added a gap dossier for Bupyeong Pungmul Festival and Dongnae Eupseong Historical Festival.
- Marked both as cases with strong official event/cultural-tourism evidence but insufficient procurement/agency evidence for contractor causality.
- Added data/bupyeong-dongnae-gap-dossier.json, .csv, bupyeong-dongnae-gap-dossier.html, and evidence note.

## Checkpoint: festival failure/risk lead queue (2026-07-08T03:24:00+09:00)

- Added the first cross-case failure/risk lead queue for price/booth governance, night-market boundary gaps, sponsorship/host structure, demand-forecast thresholds, crowd safety, traffic and budget traceability.
- Separated final causality from leads: each record now states what evidence must be collected before blaming a contractor, subcontractor, booth operator or public host.
- Added data/festival-failure-risk-leads-wave1.json, .csv, festival-failure-risk-leads-wave1.html, and evidence note.

## Checkpoint: Yeongyang Sannamul price governance dossier (2026-07-08T03:36:00+09:00)

- Built a detailed dossier for the 2023 Yeongyang Sannamul old-snack price controversy and the 2024/2026 corrective governance trail.
- Classified the case as B+ for public responsibility and corrective-policy chain, but only C for broker/seat-fee mechanics until primary allocation/contract records are found.
- Added data/yeongyang-sannamul-price-governance-dossier.json, .csv, yeongyang-sannamul-price-governance-dossier.html, and evidence note.

## Checkpoint: Hongcheon Ice night-market price dossier (2026-07-08T03:48:00+09:00)

- Built a boundary-control dossier for the 2024 Hongcheon River Ice Festival night-market price controversy.
- Separated official in-venue vendors selected by foundation bidding and pre-agreed menu/prices from the nearby/night-market operator lead.
- Added data/hongcheon-ice-nightmarket-price-dossier.json, .csv, hongcheon-ice-nightmarket-price-dossier.html, and evidence note.

## Checkpoint: Incheon crowd forecast threshold dossier (2026-07-08T04:02:00+09:00)

- Built a demand-forecast and safety-threshold dossier for Yaksasa Mountain Temple Concert and Yeongjong Fireworks Festa.
- Connected case evidence to MOIS local-festival safety thresholds and Incheon City's four-stage crowd-safety model.
- Added data/incheon-crowd-forecast-threshold-dossier.json, .csv, incheon-crowd-forecast-threshold-dossier.html, and evidence note.

## Checkpoint: Daejeon Zero O'Clock mixed verdict dossier (2026-07-08T04:16:00+09:00)

- Built a mixed verdict dossier for Daejeon Zero O'Clock Festival.
- Preserved official success signals, including visitor count, economic effect and 3-no festival claims, while separating traffic, budget, local-identity and merchant-impact counter-evidence.
- Added data/daejeon-zero-clock-mixed-verdict-dossier.json, .csv, daejeon-zero-clock-mixed-verdict-dossier.html, and evidence note.

## Checkpoint: why-cause router wave 2 (2026-07-08T04:24:00+09:00)

- Added a human-readable causal router so reviewers can start from questions like contractor/procurement, price/booth, demand/crowd, weather/safety and mixed-verdict rather than raw festival names.
- Linked current dossiers to the appropriate causal question and stated the evidence rule needed before making a strong causal claim.
- Added data/why-cause-router-wave2.json, .csv, why-cause-router-wave2.html, and evidence note.

## Checkpoint: Jinhae Gunhangje prevention benchmark (2026-07-08T04:34:00+09:00)

- Built a prevention benchmark dossier for Jinhae Gunhangje, combining 2023 scale/outcome, 2025 price/booth controls, and 2026 one-strike price plus safety inspection controls.
- Separated price, booth-transfer, crowd-capacity, traffic and emergency-response controls into a reusable large-festival model.
- Added data/jinhae-gunhangje-price-safety-prevention-dossier.json, .csv, jinhae-gunhangje-price-safety-prevention-dossier.html, evidence note, and why-cause router links.

## Checkpoint: budget waste causality model (2026-07-08T04:45:00+09:00)

- Added a budget-waste evidence model so high budget is not automatically treated as waste.
- Defined risk flags for high net cost with weak outcomes, unverified headline economic effects, contract scope mismatch, externalized inconvenience and booth/price leakage.
- Added data/budget-waste-causality-model-wave1.json, .csv, budget-waste-causality-model-wave1.html, and evidence note.

## Checkpoint: case evidence matrix wave 2 (2026-07-08T05:00:00+09:00)

- Added a human-first matrix that re-indexes current dossiers by question: contractor/procurement, price/booth, demand/crowd, budget waste, safety/weather, success contrast and procurement gap.
- Added explicit guardrails for when a case can and cannot be blamed on a contractor, subcontractor, booth operator or public host.
- Added data/case-evidence-matrix-wave2.json, .csv, case-evidence-matrix-wave2.html, and evidence note.

## Checkpoint: Hwacheon Sancheoneo weather/recovery dossier (2026-07-08T05:15:00+09:00)

- Added a weather-dependent winter festival dossier comparing the 2020 warm-winter/COVID/ASF crisis with 2025-2026 safety, visitor, economic-effect and local-capture success signals.
- Classified the case as B+ for weather/safety/success-model evidence and C for budget-recovery until Local Finance 365 cost-accounting rows are joined.
- Added data/hwacheon-sancheoneo-weather-recovery-dossier.json, .csv, hwacheon-sancheoneo-weather-recovery-dossier.html, evidence note, and case-matrix links.

## Checkpoint: budget recovery comparator wave 1 (2026-07-08T05:30:00+09:00)

- Added a budget-recovery lead queue comparing reported 2024 gross execution, admission/own revenue, recovery rate and investigation priority.
- Separated high-spend/high-recovery benchmark leads from low-recovery and zero-revenue review leads while preserving the guardrail that media numeric leads need Local Finance 365 verification.
- Added data/budget-recovery-comparator-wave1.json, .csv, budget-recovery-comparator-wave1.html, and evidence note.

## Checkpoint: Andong Maskdance mixed budget/identity dossier (2026-07-08T05:45:00+09:00)

- Added a mixed dossier for Andong International Maskdance Festival separating 2024 visitor/global-content success signals from low direct-recovery and economic-effect methodology review needs.
- Preserved the distinction between cultural public value, direct revenue recovery, visitor-counting methodology, citywide capacity and contractor causality.
- Added data/andong-maskdance-mixed-budget-identity-dossier.json, .csv, andong-maskdance-mixed-budget-identity-dossier.html, evidence note, and case-matrix links.

## Checkpoint: Jinju Namgang Lantern price/social-license dossier (2026-07-08T06:00:00+09:00)

- Added a mixed price/social-license dossier for Jinju Namgang Lantern Festival covering 2016 paid-entry conflict, 2026 free-entry/paid-experience model, 2025 outcome signals and 2025 food-truck price controversy.
- Separated global-festival success signals from booth-price governance, resident inconvenience, crowding and unsupported subcontractor causality claims.
- Added data/jinju-lantern-price-social-license-dossier.json, .csv, jinju-lantern-price-social-license-dossier.html, evidence note, and case-matrix links.

## Checkpoint: Boryeong Mud success/local-capture dossier (2026-07-08T06:15:00+09:00)

- Added a success benchmark dossier for Boryeong Mud Festival covering paid mud-experience zones, local voucher return, foreign visitors, night/performance content, stay/spend signals and marketing-attribution caveats.
- Classified Boryeong as a budget-waste control case: high spend is not waste when paid conversion and local-capture evidence are strong, but contractor attribution remains unproven.
- Added data/boryeong-mud-success-local-capture-dossier.json, .csv, boryeong-mud-success-local-capture-dossier.html, evidence note, and case-matrix links.

## Checkpoint: Hampyeong Butterfly success/price-boundary dossier (2026-07-08T06:30:00+09:00)

- Added a mixed success/price-boundary dossier for Hampyeong Butterfly Festival covering paid ecological content, coupon/local-capture structure, 2024 cost-recovery lead, 2026 outcome signals and the 2023 nearby night-market price controversy.
- Classified the case as B+ success, B price-boundary and C contractor attribution: stage procurement exists, but the current evidence does not support blaming a contractor/subcontractor for price controversy or crediting one for total success.
- Added data/hampyeong-butterfly-success-price-boundary-dossier.json, .csv, hampyeong-butterfly-success-price-boundary-dossier.html, evidence note, and case-matrix links.

## Checkpoint: Bonghwa Sweetfish budget/accounting gap dossier (2026-07-08T06:45:00+09:00)

- Added a budget/accounting gap dossier for Bonghwa Sweetfish Festival covering paid experience fees, Bonghwa Love gift-certificate refunds, 2024 high-cost/zero-revenue lead, 2025 festival-revenue donation and 2026 event-agency/booth procurement layers.
- Classified 2023 cancellation as a natural-disaster/safety recovery case caused by heavy rain and Naeseongcheon flooding, not demand-forecast or contractor failure.
- Added data/bonghwa-sweetfish-budget-accounting-gap-dossier.json, .csv, bonghwa-sweetfish-budget-accounting-gap-dossier.html, evidence note, and case-matrix links.

## Checkpoint: Sangju World Hat free-access budget-risk dossier (2026-07-08T07:00:00+09:00)

- Added a free-access budget-risk dossier for Sangju World Hat Festival covering the 2024 city-funded/zero-revenue lead, explicit paid-content weakness explanation, 2025 content-maturation attempts and reported visitor/stay/economic-effect improvement.
- Classified the case as B+ for direct cause of revenue weakness, B for outcome leads and C for contractor attribution because no public evidence yet ties a specific agency or subcontractor to the revenue model problem.
- Added data/sangju-hat-free-access-budget-risk-dossier.json, .csv, sangju-hat-free-access-budget-risk-dossier.html, evidence note, and case-matrix links.

## Checkpoint: Mungyeong Teabowl cultural-value/budget-recovery dossier (2026-07-08T07:15:00+09:00)

- Added a cultural-value/budget-recovery dossier for Mungyeong Teabowl Festival covering free-entry/paid-experience structure, 2024 low direct-recovery lead, 2025 pass/voucher/tourism-discount redesign and 2026 experiential/smart-operation improvements.
- Separated cultural public value from direct revenue recovery: low admission recovery is a budget-risk lead, but not a failure verdict without local-spend, satisfaction, artist-sales and evaluation-method evidence.
- Added data/mungyeong-teabowl-cultural-value-budget-recovery-dossier.json, .csv, mungyeong-teabowl-cultural-value-budget-recovery-dossier.html, evidence note, and case-matrix links.

## Checkpoint: Cheongsong Apple metric-opacity success dossier (2026-07-08T07:30:00+09:00)

- Added a success/control dossier for Cheongsong Apple Festival covering participatory content, hybrid online expansion, price-fixed sales, wildfire recovery narrative, satisfaction/economic-effect reporting and 2025/2026 stage-performance procurement context.
- Classified the case as B+ success, B metric-opacity and C contractor attribution: economic-effect formulas and online/offline visitor definitions must be audited before using the numbers for demand forecasting or budget-waste decisions.
- Added data/cheongsong-apple-metric-opacity-success-dossier.json, .csv, cheongsong-apple-metric-opacity-success-dossier.html, evidence note, case-matrix links and why-cause router links.

## Checkpoint: Yeongdeok Snow Crab price/brand-control dossier (2026-07-08T07:45:00+09:00)

- Added a price-governance prevention dossier for Yeongdeok Snow Crab Festival covering live-commodity price volatility, stakeholder agreement, market-price display, booth price labels, complaint systems, citizen monitoring, crab experience/tasting supply expansion and smart queueing.
- Classified the case as B+ price governance, B outcome lead and C contractor attribution: public evidence supports a price/brand-control model, not a hidden agency or subcontractor causality claim.
- Added data/yeongdeok-snowcrab-price-brand-control-dossier.json, .csv, yeongdeok-snowcrab-price-brand-control-dossier.html, evidence note, case-matrix links and why-cause router links.

## Checkpoint: Gwangyang Maehwa traffic/demand redesign dossier (2026-07-08T08:00:00+09:00)

- Added a demand/crowd/traffic redesign dossier for Gwangyang Maehwa Festival covering historic road/parking limits, 2024 car-free/shuttle/real-time traffic controls, 2026 parking and shuttle capacity, accumulated-temperature bloom prediction, paid-entry/local-voucher refund and satisfaction/outcome leads.
- Classified the case as B+ demand/traffic redesign, B+ outcome and C contractor attribution: public evidence supports a capacity-matching model, not a hidden agency or subcontractor causality claim.
- Added data/gwangyang-maehwa-traffic-demand-redesign-dossier.json, .csv, gwangyang-maehwa-traffic-demand-redesign-dossier.html, evidence note, case-matrix links and why-cause router links.

## Checkpoint: Jeju Fire content/social-license transition dossier (2026-07-08T08:15:00+09:00)

- Added a content/social-license transition dossier for Jeju Fire Festival covering oreum-burning controversy, climate/wildfire/ecological concerns, 2023 deliberation, 2024 non-held redesign year, 2025 virtual-fire wind interruption and 2026 hybrid recovery leads.
- Classified the case as B+ content/social-license, B weather shock/recovery lead and C contractor attribution: the evidence supports a flagship-content legitimacy problem, not a hidden agency or subcontractor causality claim.
- Added data/jeju-fire-content-social-license-transition-dossier.json, .csv, jeju-fire-content-social-license-transition-dossier.html, evidence note, case-matrix links and why-cause router route.

## Checkpoint: Namwon Chunhyang price-recovery dossier (2026-07-08T08:30:00+09:00)

- Added a price-governance recovery dossier for Namwon Chunhyang Festival covering the 2023 high-price/low-portion controversy, 2024 direct booth rental, price/weight labels, KRW 10k menu cap, expulsion/admin/criminal action, Theborn/Baek Jong-won food trust mechanism, outside-merchant enforcement and 2025/2026 visitor recovery leads.
- Classified the case as B+ price recovery, B procurement context and C contractor attribution: the KRW 250m promotion/marketing tender is real context, but not food-price causality without RFP scope and booth-operation evidence.
- Added data/namwon-chunhyang-price-recovery-dossier.json, .csv, namwon-chunhyang-price-recovery-dossier.html, evidence note, case-matrix links and why-cause router links.

## Checkpoint: Sejong Nakhwa crowd/traffic stabilization dossier (2026-07-08T08:45:00+09:00)

- Added a night-spectacle crowd/traffic dossier for Sejong Nakhwa Festival covering the 2023 first-year parking/traffic bottleneck, 2024 parking/traffic/safety controls, 2024 evaluation gaps, 2025 outside-visitor/economic-effect leads and 2026 no-accident 100k-crowd lead.
- Classified the case as B+ traffic/safety stabilization, B outcome and C contractor attribution: public evidence supports capacity planning and public safety/traffic coordination, not hidden subcontractor causality.
- Added data/sejong-nakhwa-crowd-traffic-stabilization-dossier.json, .csv, sejong-nakhwa-crowd-traffic-stabilization-dossier.html, evidence note, case-matrix links and why-cause router links.

## Checkpoint: Inje Icefish climate/water-level cancellation dossier (2026-07-08T09:00:00+09:00)

- Added a winter-site failure dossier for Inje Icefish Festival covering 2019 person-counting/economic-effect baseline, 2023 demand/effect lead, 2024-2026 cancellations, Soyang Dam water-level threshold, insufficient freezing, site submersion, safety risk and four-season tourism adaptation leads.
- Classified the case as B+ climate/water-level, B+ demand history and C contractor attribution: public evidence supports physical site-condition failure, not demand disappearance or hidden subcontractor causality.
- Added data/inje-icefish-climate-waterlevel-cancellation-dossier.json, .csv, inje-icefish-climate-waterlevel-cancellation-dossier.html, evidence note, case-matrix links and why-cause router links.

## Checkpoint: 2026-07-08T09:15:00+09:00
- Added 무안연꽃축제 heat/shuttle/procurement dossier.
- New files: .omo/evidence/muan-lotus-heat-shuttle-procurement-dossier.md, data/muan-lotus-heat-shuttle-procurement-dossier.json, data/muan-lotus-heat-shuttle-procurement-dossier.csv, $slug.html.
- Updated case evidence matrix to 27 festival records and added season_heat_comfort_records.
- Added why-router path for season/heat/bloom/comfort failures and corrected the demand/crowd row links to point to 광양매화축제 and 세종낙화축제 instead of price-row cases.
- Evidence status: B+. Public sources support the seasonal redesign, price-control measures, disaster scale-down, and procurement structure. They do not yet prove contractor fault or final budget efficiency.

## Checkpoint: 2026-07-08T09:45:00+09:00
- Added 부산불꽃축제 crowd/ticket/procurement dossier.
- New files: .omo/evidence/busan-fireworks-crowd-ticket-procurement-dossier.md, data/busan-fireworks-crowd-ticket-procurement-dossier.json, data/busan-fireworks-crowd-ticket-procurement-dossier.csv, $slug.html.
- Updated case evidence matrix to 28 festival records and added mega_crowd_firework_records.
- Added why-router coverage for budget/outsourcing governance and linked 부산불꽃축제 into the demand/crowd route.
- Evidence status: A-. Strong public-source support for attendance variation, safety controls, paid-seat prices, and fragmented procurement notices. Budget figures from KNN are treated as media claims requiring official budget/settlement confirmation.

## Checkpoint: 2026-07-08T10:15:00+09:00
- Added 화천산천어축제 climate/economy/governance dossier.
- New files: .omo/evidence/hwacheon-sancheoneo-climate-economy-governance-dossier.md, data/hwacheon-sancheoneo-climate-economy-governance-dossier.json, data/hwacheon-sancheoneo-climate-economy-governance-dossier.csv, $slug.html.
- Updated case evidence matrix to 29 festival records and added winter_climate_success_records.
- Added why-router coverage for winter ice/climate failure mode and linked 화천산천어축제 into budget/outsourcing governance.
- Evidence status: A-. Strong public-source support for attendance, economic-effect report, climate disruption history, animal-welfare controversy, and recurring procurement signals. Full budget efficiency still needs official settlement and contract data.

## Checkpoint: 2026-07-08T10:45:00+09:00
- Added 진주남강유등축제 paid-access governance dossier.
- New files: .omo/evidence/jinju-yudeung-paid-access-governance-dossier.md, data/jinju-yudeung-paid-access-governance-dossier.json, data/jinju-yudeung-paid-access-governance-dossier.csv, $slug.html.
- Updated case evidence matrix to 30 festival records and added paid_access_social_license_records.
- Added why-router coverage for paid-access/social-license failures and linked 진주남강유등축제 into budget/outsourcing governance.
- Evidence status: A-. Strong public-source support for the 2016 paid-entry/screening-wall controversy, 2025 attendance/economic-effect claims, 2026 global-festival funding, and 2024-2025 procurement signals. Full fiscal efficiency requires settlement and contract award data.

## Checkpoint: 2026-07-08T11:15:00+09:00
- Added 보령머드축제 global/paid-experience governance dossier.
- New files: .omo/evidence/boryeong-mud-global-paid-experience-governance-dossier.md, data/boryeong-mud-global-paid-experience-governance-dossier.json, data/boryeong-mud-global-paid-experience-governance-dossier.csv, $slug.html.
- Updated case evidence matrix to 31 festival records and added paid_experience_global_records.
- Added why-router coverage for paid-experience/local-capture and linked 보령머드축제 into budget/outsourcing governance and season/heat comfort routes.
- Evidence status: A-. Strong public-source support for official schedule/pricing, 2024 attendance and paid-experience figures, 2020 pandemic substitution, 2026 global-festival funding, and 2026 liability-insurance procurement. Full budget efficiency still needs settlement, paid-zone sales, voucher usage, and insurance/incident logs.

## Checkpoint: 
- Added goal expansion requested by the user: final common-pattern synthesis across all festival cases.
- Added DESIGN.md before redesign work and introduced one shared Toss-like minimal style in ssets/toss-report-theme.css.
- Linked the shared Pretendard-based theme into every top-level HTML file for consistent typography and page structure.
- Added estival-common-patterns-synthesis.html summarizing success patterns, failure/risk patterns, and a festival-by-festival pattern map.

## Checkpoint: 2026-07-08T11:45:00+09:00
- Added 서울세계불꽃축제 crowd/public-private governance dossier.
- New files: .omo/evidence/seoul-fireworks-crowd-public-private-governance-dossier.md, data/seoul-fireworks-crowd-public-private-governance-dossier.json, data/seoul-fireworks-crowd-public-private-governance-dossier.csv, $slug.html.
- Updated case evidence matrix to 32 festival records and added public_private_megacity_records.
- Added why-router coverage for public/private mega-event responsibility and linked 서울세계불꽃축제 into demand/crowd and budget/outsourcing governance routes.
- Updated common-pattern synthesis count and festival pattern map.
- Evidence status: A-. Strong public-source support for 100만 인파, police/Seoul/Hanwha safety operations, traffic controls, toilet/trash/medical capacity, and resident externality claims. Exact public cost allocation still requires official budget/settlement data.

## Checkpoint: 춘천마임축제 2020-2026
- Added case id: chuncheon-mime-2020-2026.
- Evidence: official organizer/KTO pages, COVID cancellation, 2023/2024 evaluation metrics, traffic-space improvement, budget cut record, 2026 closure and honor festival designation.
- Planning implication: collect space agreements, budget stability, time-band crowding, and transport capacity in addition to visitor totals.


## Checkpoint: 대전빵축제 2023-2026
- Added case id: daejeon-bread-2023-2026.
- Evidence: 2023 expert critique, 2024 crowd/queue reports, 2025 official schedule and closure metrics, 2026 operation outsourcing bid result.
- Planning implication: collect queue time, booth supply, sell-out time, traffic, and agency KPI data, not just visitor totals.


## Checkpoint: 자라섬재즈페스티벌 2018-2026
- Added case id: jarasum-jazz-2018-2026.
- Evidence: official 2026 site, 2025 lineup/attendance milestone, 2024 ticket data, 2020 online pivot, 2018 subsidy/budget reporting, 2023 agreement/revenue controversy reporting.
- Planning implication: collect paid ticket conversion, subsidy/sponsor/ticket revenue split, local stay spending, and contingency policy data.


## Checkpoint: 강릉커피축제 2020-2026
- Added case id: gangneung-coffee-2020-2026.
- Evidence: official festival site, 2025 performance metrics, 2024 parking bottleneck, 2020 cancellation, 2021 delay, long-run evaluation, 2023 outsourcing award.
- Planning implication: collect parking/shuttle capacity, district-level cafe sales, visitor stay spending, and outsourced operation KPIs alongside visitor totals.

