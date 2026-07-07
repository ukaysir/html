# MCST download-pattern checkpoint

Date: 2026-07-08

Observed from the public MCST regional festival page:
- `fnDown()` builds `{year}_festival.zip`.
- It calls `file_download(strFileNM, strSavedFileNM, 'PORTAL.DOCUMENT.UPLOAD')`.
- `file_download` resolves to `/servlets/eduport/front/upload/UplDownloadFile` with `pFileName`, `pRealName`, `pPath` and `pFlag`.

Added:
- `data/mcst-download-manifest.json`

Caution:
- This checkpoint records the download pattern only. Each annual ZIP still needs HTTP status, content type, size and checksum before it should be treated as ingested master data.
