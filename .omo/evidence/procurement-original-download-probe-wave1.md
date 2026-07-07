# Procurement original download probe wave 1

Created: 2026-07-08T01:45:00+09:00

Scope: P2 benchmark festivals and procurement/agency leads where public web evidence can connect festival planning to contractor/procurement structure.

Method:
- Search official domains first, then public procurement mirrors.
- Probe whether original attachments are directly downloadable with simple HTTP, referrer HTTP, or only visible through a source page.
- Classify each item by causal-use strength before making "why failed/succeeded" claims.

Key findings:
- Suwon SWCF 2020 procurement attachments require the official page as referrer but download as force-download originals. This is official original evidence for the event-agency/RFP structure.
- Bucheon KOMACON has official tender and official evaluation-result pages for 2025, including RFP/evaluation-result attachments. This is the strongest contractor-governance chain found in this wave.
- Incheon Pentaport 2026 G2B direct file access returned 403, but a full public PDF mirror is downloadable and a university notice documents ITO evaluation-committee recruitment. Treat as strong lead, not official original until ITO/G2B original page is captured.
- Cheorwon GCWCF evaluation result is official and web-readable, but curl HEAD followed a WAF/error redirect. Treat page text as official, attachment automation unresolved.

Next expansion:
- Capture direct KOMACON 2025 attachment URLs and headers.
- Search ITO/G2B pages for original Pentaport 2026 공모지침서 and evaluation-result notice.
- Search Suwon 2026 제63회 original G2B/Suwon page to replace the momo365 mirror.
- Add contractor names only when evaluation result, award result, contract disclosure, or settlement source supports them.
