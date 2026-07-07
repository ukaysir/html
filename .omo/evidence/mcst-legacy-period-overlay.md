# MCST legacy period overlay checkpoint

Date: 2026-07-08

Added:
- `data/master/mcst-legacy-period-overlays-2017-2021.json`
- `data/master/mcst-legacy-period-overlays-2017-2021.csv`
- `data/master/mcst-legacy-period-overlays-2017-2021.summary.json`

Scope:
- 2017-2021 MCST master draft rows where dates were originally stored as raw legacy period strings.

Result:
- Total overlay records: 4,475
- Exact day-level ranges parsed: 2,357
- Single exact dates parsed: 98
- Partial/unparsed and still requiring review: 2,020

Guardrail:
- The overlay does not overwrite master data.
- Ambiguous strings such as month-only, mid-month, tentative, seasonal and multiple-period formats remain low-confidence review items.
