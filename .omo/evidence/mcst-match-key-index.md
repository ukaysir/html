# MCST-to-finance/procurement match key index

Generated: 2026-07-08T01:07:16+09:00

## Purpose
This artifact converts the 10,198-row MCST regional festival master draft into practical search and join keys for the next evidence layer: local finance cost/budget data, bid notices, contract status, outsourced operator traces, and post-event result reports.

## Outputs
- data/master/mcst-finance-procurement-match-keys.json
- data/master/mcst-finance-procurement-match-keys.csv
- data/master/mcst-finance-procurement-match-keys.summary.json

## Counts
- Total records: 10198
- High-priority join candidates: 3672
- Medium-priority join candidates: 6430
- Low-priority join candidates: 96
- Date windows available: 4030
- Budget fields available: 9500
- 2017-2021 overlay dates used: 2455

## Year readiness
| Year | Records | High | Medium | Low | Date available | Budget available |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| 2017 | 733 | 454 | 279 | 0 | 456 | 725 |
| 2018 | 886 | 526 | 360 | 0 | 536 | 869 |
| 2019 | 884 | 223 | 578 | 83 | 547 | 325 |
| 2020 | 968 | 502 | 466 | 0 | 507 | 955 |
| 2021 | 1004 | 401 | 603 | 0 | 409 | 991 |
| 2022 | 944 | 0 | 944 | 0 | 0 | 923 |
| 2023 | 1129 | 0 | 1129 | 0 | 0 | 1090 |
| 2024 | 1170 | 0 | 1170 | 0 | 0 | 1164 |
| 2025 | 1214 | 769 | 434 | 11 | 775 | 1197 |
| 2026 | 1266 | 797 | 467 | 2 | 800 | 1261 |

## Interpretation rules
- High: normalized festival name, local government key, date window, and budget are all present.
- Medium: enough keys exist for public-source search, but at least one major dimension needs confirmation.
- Low: do not draw automated success/failure conclusions without another source.

## Why this matters
The user's core question is not simply which festivals existed, but why demand forecasting, outsourcing, procurement, budget, crowding, and satisfaction outcomes diverged. This index is the bridge from festival identity to public finance/procurement evidence.
