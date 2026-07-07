# Korean Festival Cause Dashboard

Public-source-only research dashboard for tracing why Korean festivals succeed or fail.

Open `index.html` to view the dashboard.

See `RESEARCH_STATUS.md` for checkpoint status, completed evidence layers and remaining gaps.

## Scope
- 2016-2026 Korean festivals.
- Demand forecast, visitor performance, budget, contracts, agencies, public subcontract/booth traces and operational risk evidence.
- Agent-only public-source workflow: no phone calls, emails, interviews, information disclosure requests, paid/login-only sources or access-control bypass.

## Current status
This repository is a pushed research checkpoint. It contains:
- A standalone HTML investigation dashboard.
- Source maps for festival master, tourism, finance, procurement, contract and case evidence.
- Claim/evidence graph files to prevent unsupported causal claims.
- Access-feasibility and scoring models for the next collection waves.

The dataset is not yet a complete national raw-data archive. The dashboard explicitly keeps coverage and access limitations visible.

## GitHub Pages
The repo is structurally ready for GitHub Pages because `index.html` is at the repository root.

Pages was checked as not enabled during the research run. To publish, use:
- Source: `Deploy from a branch`
- Branch: `main`
- Folder: `/(root)`
- Expected URL after activation: `https://ukaysir.github.io/html/`

## Key data files
- `data/festival-source-map.json`
- `data/festival-cases.json`
- `data/evidence-manifest.json`
- `data/claim-graph.json`
- `data/schema.json`
- `data/scoring-rubric.json`
- `data/relation-graph-schema.json`
- `data/access-feasibility.json`
- `data/festival-case-evidence-wave3.json`
- `data/procurement-evidence-wave3.json`
- `data/source-coverage-matrix.json`
- `data/cause-index.json`
- `data/normalized-key-spec.json`
- `data/collection-backlog.json`
- `data/master-source-inventory.json`
- `data/mcst-download-manifest.json`
- `data/mcst-download-probe.json`
- `data/mcst-archive-schema-probe.json`
- `data/master/mcst-region-festivals-2017-2026.master-draft.json`
- `data/master/mcst-region-festivals-2017-2026.master-draft.csv`
- `data/master/mcst-region-festivals-2017-2026.summary.json`
- `data/master/mcst-region-festivals-2017-2026.summary-expanded.json`
- `data/master/mcst-region-festivals-2017-2026.lite-index.json`
- `data/master/mcst-legacy-period-overlays-2017-2021.json`
- `data/master/mcst-legacy-period-overlays-2017-2021.csv`
- `data/master/mcst-legacy-period-overlays-2017-2021.summary.json`
## Latest matching artifacts

- data/master/mcst-finance-procurement-match-keys.json: 10,198 MCST festival rows converted into finance/procurement search and join keys.
- data/master/mcst-finance-procurement-match-keys.csv: spreadsheet-friendly version for filtering by year, local government, budget band, and join priority.
- data/master/mcst-finance-procurement-match-keys.summary.json: year-level readiness counts for the dashboard.


## MCST benchmark cohort

- data/mcst-cultural-tourism-benchmark-2026-2027.json: official 2026-2027 cultural-tourism festival cohort extracted from the MCST HWPX press attachment and joined to the 2026 MCST master.
- data/mcst-cultural-tourism-benchmark-2026-2027.csv: spreadsheet-friendly benchmark join table.
- mcst-cultural-tourism-benchmark-2026-2027.html: human-readable benchmark cohort page.

## Benchmark priority queue

- data/benchmark-risk-priority-queue.json: investigation priority queue for the 2026-2027 cultural-tourism benchmark cohort.
- enchmark-risk-priority-queue.html: human-readable page showing which benchmark festivals should be traced first for budget/procurement/crowding/satisfaction causes.

## Benchmark procurement queue

- data/benchmark-procurement-search-queue.json: procurement/agency search queue for P2 benchmark festivals.
- enchmark-procurement-search-queue.html: human-readable query plan and evidence-seed page for contractor/procurement tracing.

## Procurement source strength

- data/procurement-source-strength-wave1.json: source-strength classification for procurement/agency leads.
- procurement-source-strength-wave1.html: human-readable distinction between official originals, official event pages, mirrors, and publicity-only leads.

## Procurement original download probe

- data/procurement-original-download-probe-wave1.json: official attachment download and source-upgrade probe for P2 benchmark festivals.
- procurement-original-download-probe-wave1.html: human-readable map of official original, evaluation result, mirror-only, blocked, and event-only evidence.

## Governance causal chain

- data/festival-governance-causal-chain-wave1.json: separates causal candidates from procurement-only or outcome-only evidence.
- festival-governance-causal-chain-wave1.html: human-readable chain from incident/success outcome to organizer, contractor, or evaluation structure.

## Pentaport 2019 cause dossier

- data/pentaport-2019-cause-dossier.json: first detailed Level A causal-candidate dossier linking governance, operator selection, and public experience criticism.
- pentaport-2019-cause-dossier.html: human-readable "why did this become a problem?" dossier with evidence strength and open proof gaps.

## Pentaport 2025 success dossier

- data/pentaport-2025-success-dossier.json: success-side dossier connecting visitor count, satisfaction, heat/safety operations, programming, and local linkage.
- pentaport-2025-success-dossier.html: human-readable "why did this work?" contrast case while preserving contractor-attribution gaps.

## Bucheon Comics 2025 governance dossier

- data/bucheon-comics-2025-governance-dossier.json: official tender/evaluation chain plus outcome and cultural-tourism-selection signals.
- bucheon-comics-2025-governance-dossier.html: human-readable bridge from procurement evidence to success hypotheses without contractor overclaiming.

## Suwon Hwaseong 2026 pre-event dossier

- data/suwon-hwaseong-2026-pre-event-dossier.json: official evaluation disclosure, tender/RFP leads, and pre-event crowd/food/foreign-visitor risk variables.
- suwon-hwaseong-2026-pre-event-dossier.html: human-readable checklist for what to monitor before and after the October 2026 festival.

## Cheorwon Ice Trekking 2026 safety/outcome dossier

- data/cheorwon-ice-2026-safety-outcome-dossier.json: winter festival outcome, cultural-tourism-selection, weather/safety risk, and agency-evaluation leads.
- cheorwon-ice-2026-safety-outcome-dossier.html: human-readable dossier explaining why this case must be analyzed through weather, safety, course operation, and regional linkage.

## Hwacheon Sancheoneo weather/recovery dossier

- data/hwacheon-sancheoneo-weather-recovery-dossier.json: weather-dependent winter festival model comparing the 2020 crisis with 2025-2026 recovery/success signals.
- hwacheon-sancheoneo-weather-recovery-dossier.html: human-readable explanation of why this is a conditional ice-capacity, safety, local-capture and cost-recovery case rather than a proven contractor-failure case.

## Case evidence matrix

- data/case-evidence-matrix-wave2.json: current dossier matrix by human question, cause type, evidence level, procurement link, outcome link and next evidence needed.
- case-evidence-matrix-wave2.html: human-readable "why did this fail/succeed?" comparison table for contractor, price/booth, crowd, budget, safety and success-control questions.
- data/case-evidence-matrix-wave1.json: current dossier index by evidence level, procurement link, outcome link, and risk axes.
- case-evidence-matrix-wave1.html: human-readable matrix for deciding whether a case is contractor/procurement, demand/crowding, safety/weather, or pre-event monitoring.

## Bupyeong/Dongnae procurement gap dossier

- data/bupyeong-dongnae-gap-dossier.json: official event/cultural-tourism evidence and missing procurement/agency evidence for Bupyeong and Dongnae.
- bupyeong-dongnae-gap-dossier.html: human-readable gap map showing why contractor causality is not yet supportable for these cases.

## Festival failure/risk lead queue

- data/festival-failure-risk-leads-wave1.json: first lead queue for price/booth control, demand forecast, crowd safety, traffic and budget traceability risks.
- festival-failure-risk-leads-wave1.html: human-readable "why did this go wrong?" queue separating symptoms, operating boundaries, documents to collect and causal guardrails.

## Yeongyang Sannamul price governance dossier

- data/yeongyang-sannamul-price-governance-dossier.json: detailed price/booth governance chain for the 2023 Yeongyang old-snack controversy and later corrective measures.
- yeongyang-sannamul-price-governance-dossier.html: human-readable answer to whether the issue was vendor behavior, operating structure, broker/seat-fee mechanics, or a proven subcontractor problem.

## Hongcheon Ice night-market price dossier

- data/hongcheon-ice-nightmarket-price-dossier.json: boundary-control dossier for the 2024 Hongcheon River Ice Festival night-market price controversy.
- hongcheon-ice-nightmarket-price-dossier.html: human-readable split between official festival vendors, nearby/night-market sellers, consignment/operator leads and missing contract proof.

## Incheon crowd forecast threshold dossier

- data/incheon-crowd-forecast-threshold-dossier.json: demand-forecast and safety-threshold dossier for Yaksasa Mountain Temple Concert and Yeongjong Fireworks Festa.
- incheon-crowd-forecast-threshold-dossier.html: human-readable model linking expected attendance, 1,000-person planning threshold, site bottlenecks, late deployment and traffic dissatisfaction.

## Daejeon Zero O'Clock mixed verdict dossier

- data/daejeon-zero-clock-mixed-verdict-dossier.json: mixed success/failure dossier separating official visitors/economic effect/3-no festival claims from traffic, budget and merchant-impact counter-evidence.
- daejeon-zero-clock-mixed-verdict-dossier.html: human-readable "success or failure?" page that preserves both official outcome signals and civic inconvenience risks.

## Why-cause router

- data/why-cause-router-wave2.json: human-readable routing layer from causal questions to the most relevant dossiers.
- why-cause-router-wave2.html: "왜 망했지?" navigation page for contractor/procurement, price/booth, demand/crowd, weather/safety and mixed-verdict questions.

## Jinhae Gunhangje price/safety prevention dossier

- data/jinhae-gunhangje-price-safety-prevention-dossier.json: prevention benchmark for large-festival price control, booth-transfer control, crowd capacity, traffic and emergency response.
- jinhae-gunhangje-price-safety-prevention-dossier.html: human-readable model for how a 300만+ visitor festival attempts to prevent price and crowd-risk failures.

## Budget waste causality model

- data/budget-waste-causality-model-wave1.json: evidence model for deciding when a festival has budget-waste risk without equating high budget with waste.
- budget-waste-causality-model-wave1.html: human-readable scoring flow using net cost, revenue, visitor/satisfaction evidence, local spend, external costs and contract accountability.

## Budget recovery comparator

- data/budget-recovery-comparator-wave1.json: lead queue comparing reported 2024 festival cost, own revenue, recovery rate and budget-waste investigation priority.
- budget-recovery-comparator-wave1.html: human-readable comparator that separates high-spend/high-recovery benchmarks from low-recovery or zero-revenue review leads.

## Andong Maskdance mixed budget/identity dossier

- data/andong-maskdance-mixed-budget-identity-dossier.json: mixed dossier separating visitor/global-content success signals from low direct-recovery and economic-effect methodology risks.
- andong-maskdance-mixed-budget-identity-dossier.html: human-readable "success or budget risk?" page for Andong International Maskdance Festival.

## Jinju Namgang Lantern price/social-license dossier

- data/jinju-lantern-price-social-license-dossier.json: mixed dossier on paid-entry controversy, free-entry/paid-experience model, global-festival growth and booth-price governance.
- jinju-lantern-price-social-license-dossier.html: human-readable page showing why a successful global festival can still carry price, booth, resident-inconvenience and social-license risks.

## Boryeong Mud success/local-capture dossier

- data/boryeong-mud-success-local-capture-dossier.json: success benchmark for paid experiential content, local voucher return, foreign demand, stay/spend and marketing-attribution caveats.
- boryeong-mud-success-local-capture-dossier.html: human-readable comparator for why a high-cost festival may avoid budget-waste classification when direct paid conversion and local-capture evidence are strong.

## Hampyeong Butterfly success/price-boundary dossier

- data/hampyeong-butterfly-success-price-boundary-dossier.json: mixed success dossier separating paid ecological content, coupon/local-capture structure, budget-recovery lead, 2023 nearby night-market price controversy and stage-procurement attribution limits.
- hampyeong-butterfly-success-price-boundary-dossier.html: human-readable explanation of why Hampyeong is a success benchmark with a price-boundary risk rather than a proven subcontractor-failure case.

## Bonghwa Sweetfish budget/accounting gap dossier

- data/bonghwa-sweetfish-budget-accounting-gap-dossier.json: budget-accounting gap dossier separating paid experience/voucher structure, 2024 zero-revenue fiscal lead, 2025 revenue donation signal, 2023 flood cancellation and 2026 agency/booth procurement layers.
- bonghwa-sweetfish-budget-accounting-gap-dossier.html: human-readable explanation of why Bonghwa Sweetfish Festival should be treated as an accounting/reconciliation and natural-shock case before calling it waste or contractor failure.

## Sangju World Hat free-access budget-risk dossier

- data/sangju-hat-free-access-budget-risk-dossier.json: free-access budget-risk dossier separating 2024 zero-revenue/free-entry explanation, paid-content weakness, 2025 content-maturation efforts, outcome leads and contractor-attribution guardrails.
- sangju-hat-free-access-budget-risk-dossier.html: human-readable explanation of why Sangju World Hat Festival is a free-access public-value vs direct-revenue case rather than a proven contractor-failure case.

## Mungyeong Teabowl cultural-value/budget-recovery dossier

- data/mungyeong-teabowl-cultural-value-budget-recovery-dossier.json: cultural public-value and budget-recovery dossier separating free-entry/paid-experience structure, 2024 low recovery lead, 2025 pass/voucher/tourism-discount redesign, and agency-procurement context.
- mungyeong-teabowl-cultural-value-budget-recovery-dossier.html: human-readable explanation of why Mungyeong Teabowl Festival has budget-recovery risk without being reducible to failure or contractor causality.

## Cheongsong Apple metric-opacity success dossier

- data/cheongsong-apple-metric-opacity-success-dossier.json: success/control dossier separating offline visitors, online visits, direct/indirect economic effects, satisfaction, sales and procurement context.
- cheongsong-apple-metric-opacity-success-dossier.html: human-readable explanation of why Cheongsong Apple Festival is a success case with metric-transparency risk rather than a failure or contractor-causality case.

## Yeongdeok Snow Crab price/brand-control dossier

- data/yeongdeok-snowcrab-price-brand-control-dossier.json: price-governance prevention dossier separating live-commodity price volatility, market-price disclosure, booth labels, citizen monitors, complaint systems, supply expansion and contractor-attribution limits.
- yeongdeok-snowcrab-price-brand-control-dossier.html: human-readable explanation of why Yeongdeok Snow Crab Festival is a brand-protection and price-control benchmark rather than a proven subcontractor case.

## Gwangyang Maehwa traffic/demand redesign dossier

- data/gwangyang-maehwa-traffic-demand-redesign-dossier.json: demand/crowd/traffic dossier separating bloom timing, parking capacity, shuttle design, real-time traffic information, paid-entry/local-voucher loop, satisfaction and contractor-attribution limits.
- gwangyang-maehwa-traffic-demand-redesign-dossier.html: human-readable explanation of why Gwangyang Maehwa Festival is a traffic-capacity redesign case rather than a simple crowding failure or subcontractor case.

## Jeju Fire content/social-license transition dossier

- data/jeju-fire-content-social-license-transition-dossier.json: content-identity and social-license dossier separating oreum-burning controversy, deliberation, weather interruption, digital/hybrid redesign, recovery metrics and contractor-attribution limits.
- jeju-fire-content-social-license-transition-dossier.html: human-readable explanation of why Jeju Fire Festival is a flagship-content risk and social-license transition case rather than a simple contractor or demand-forecast case.

## Namwon Chunhyang price-recovery dossier

- data/namwon-chunhyang-price-recovery-dossier.json: price-governance recovery dossier separating 2023 food-price controversy, direct booth control, price/weight labels, enforcement, outside-merchant boundary, Theborn/Baek Jong-won cooperation, marketing-procurement context and visitor recovery leads.
- namwon-chunhyang-price-recovery-dossier.html: human-readable explanation of why Chunhyang Festival's food-price recovery is a booth-governance case rather than a simple subcontractor or marketing-agency case.

## Sejong Nakhwa crowd/traffic stabilization dossier

- data/sejong-nakhwa-crowd-traffic-stabilization-dossier.json: night-spectacle crowd dossier separating first-year traffic/parking bottleneck, parking/traffic controls, safety/fire controls, evaluation gaps, visitor/economic-effect leads and contractor-attribution limits.
- sejong-nakhwa-crowd-traffic-stabilization-dossier.html: human-readable explanation of why Sejong Nakhwa Festival is a crowd-peak and traffic-capacity stabilization case rather than a simple subcontractor case.

## Inje Icefish climate/water-level cancellation dossier

- data/inje-icefish-climate-waterlevel-cancellation-dossier.json: winter-site failure dossier separating historical demand/economic effect, Soyang Dam water-level threshold, insufficient freezing, safety cancellation, dam-governance constraints and four-season adaptation leads.
- inje-icefish-climate-waterlevel-cancellation-dossier.html: human-readable explanation of why Inje Icefish Festival is a climate/water-level site failure rather than a demand or subcontractor failure.

### Muan Lotus Festival heat/shuttle/procurement dossier
- Added muan-lotus-heat-shuttle-procurement-dossier.html and structured JSON/CSV data for 무안연꽃축제 2023-2026.
- Classifies the case as summer heat, bloom timing, visitor fatigue, price trust, disaster scale-down, and outsourcing/procurement context rather than a proven failure.
- Captures the 2026 schedule reduction and cooling/night-program redesign, 2024 price-control measures, 2023 heavy-rain scale-down, and 2026 event-agency RFP mirror.

### Busan Fireworks crowd/ticket/procurement dossier
- Added usan-fireworks-crowd-ticket-procurement-dossier.html and structured JSON/CSV data for 부산불꽃축제 2022-2026.
- Classifies the case as a mixed A- case: strong mega-crowd safety operations plus unresolved budget/procurement transparency risk.
- Captures 2022 post-Itaewon safety controls, 2023 rain-driven attendance drop, 2024 paid-seat and 103만 attendance signals, 2025 117만 outcome and emergency/complaint load, and 2025 fragmented service procurement notices.

### Hwacheon Sancheoneo climate/economy/governance dossier
- Added hwacheon-sancheoneo-climate-economy-governance-dossier.html and structured JSON/CSV data for 화천산천어축제 2020-2027.
- Classifies the case as a successful but high-dependency winter model: engineered ice safety, local economic linkage, animal-welfare social-license pressure, and recurring procurement governance.
- Captures 2020 abnormal-warm/winter-rain disruption, 2021-2022 COVID cancellations, 2023 restart, 2026 159만 attendance and 1,018억 direct economic effect, and foundation-led tender signals.

### Jinju Yudeung paid-access governance dossier
- Added jinju-yudeung-paid-access-governance-dossier.html and structured JSON/CSV data for 진주남강유등축제 2015-2026.
- Classifies the case as a paid-access/social-license recovery case: full paid entry and screening-wall backlash, then free-entry/paid-experience recovery and global-festival growth funding.
- Captures 2016 paid-access controversy, 2025 172만 attendance and 2,400억 regional effect, 2026 global-festival selection, and fragmented lighting/sound/security/food/vendor procurement.

### Boryeong Mud global/paid-experience governance dossier
- Added oryeong-mud-global-paid-experience-governance-dossier.html and structured JSON/CSV data for 보령머드축제 2020-2026.
- Classifies the case as a global experiential festival with paid-zone demand control, local voucher recirculation, heat/contact safety, pandemic substitution history, and insurance/procurement governance.
- Captures 2024 165만 attendance and 3.99만 paid-experience users, 2026 global-festival funding, official paid-zone prices, and the 2026 liability-insurance procurement structure.

### Unified Toss-style design and common-pattern synthesis
- Added DESIGN.md as the shared design-system contract.
- Added ssets/toss-report-theme.css and linked it from every top-level HTML file to force Pretendard and one Toss-like minimal dashboard style across the report.
- Added estival-common-patterns-synthesis.html as the final synthesis page comparing success and failure patterns across all festival cases.
