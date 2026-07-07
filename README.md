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
