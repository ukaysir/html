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
