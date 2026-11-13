# bytra17

Portfolio website of Ebi Putra (Data Analyst & Data Engineer).
Live: https://ebiputra17.github.io/bytra17/

Static site: edit `index.html`, push to `main`, GitHub Pages redeploys automatically.

## Bytra Power BI Portal

`portal/` is a static Power BI portal: https://ebiputra17.github.io/bytra17/portal/

Reports are listed in the `REPORTS` array at the bottom of `portal/index.html`. To add one, copy an entry and fill it in:

- `embedUrl`: a Power BI **Publish to web** link (`https://app.powerbi.com/view?r=...`).
  When it is set, the live interactive report is shown. When it is empty, the screenshots and recording are shown.
  Publish to web makes the report public, so only use it for reports with dummy or public data.
- `video`, `images`: paths relative to `portal/`, for example `../assets/work/...`.
