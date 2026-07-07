# MCST archive schema probe checkpoint

Date: 2026-07-08

Observed:
- Each MCST annual ZIP from 2017 through 2026 contains an XLSX regional festival workbook.
- 2017 and 2018 ZIPs also contain HWP culture-tourism-festival files.
- First worksheet rows provide annual aggregate counts and inclusion/exclusion notes.

Derived annual totals:
- 2017: 733
- 2018: 886
- 2019: 884
- 2020: 968
- 2021: 1004
- 2022: 944
- 2023: 1129
- 2024: 1170
- 2025: 1214
- 2026: 1266

Added:
- `data/mcst-archive-schema-probe.json`

Next:
- Normalize event-level rows while skipping title, aggregate and note rows.
