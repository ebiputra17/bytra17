# bytra17

Portfolio website of Ebi Putra (Data Analyst & Data Engineer).
Live: https://ebiputra17.github.io/bytra17/

Static site: edit `index.html`, push to `main`, GitHub Pages redeploys automatically.

## Bytra Power BI Portal

`portal/` is a static demo of the Bytra app (Laravel + Vue + AdminLTE): https://ebiputra17.github.io/bytra17/portal/

It copies the app's look: login page, then an AdminLTE layout with the Group Report → Dashboard Group → Dashboard bar,
plus read-only Master Report, User & Role and About pages. Demo account: `demo` / `demo`.
The login is a simulation only (a static page cannot protect anything), so everything shown must be dummy or public data.

Reports are listed in the `REPORTS` array at the bottom of `portal/index.html`. To add one, copy an entry and fill it in:

- `group`, `subgroup`: shown in the Group Report and Dashboard Group dropdowns.

- `embedUrl`: a Power BI **Publish to web** link (`https://app.powerbi.com/view?r=...`).
  When it is set, the live interactive report is shown. When it is empty, the screenshots and recording are shown.
  Publish to web makes the report public, so only use it for reports with dummy or public data.
- `video`, `images`: paths relative to `portal/`, for example `../assets/work/...`.
