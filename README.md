# Oskar's Daily Brief
Static site (GitHub Pages, main branch root). No build step.

## Add a brief
1. Copy `template.html` to `briefs/YYYY-MM-DD.html`. Fill `{{DATE}}`, `{{DATE_LONG}}` (e.g. "Monday, October 12, 2026"), `{{HEADLINE}}`.
2. Hero: fill 3-4 top story cards (`{{Sn_*}}`): `CLASS` is the area class, `LABEL` the chip text, `HEADLINE`, `WHY` (one line why it matters), `URL`, `SOURCE`. Delete unused cards.
3. Area classes and chip labels (fixed colors): `ai` AI, `macro` Macro, `sea` Red Sea, `sci` Science, `data` "Data & Cloud" (Data engineering & AI cloud: Polars, DuckDB, chDB, ClickHouse plus Cloudflare, AWS, Tailscale, GCP, Azure, Vercel, Fly.io, Modal, Databricks, Snowflake). Extra sections: `channels`, `people`, `potentials`.
4. Replace each `{{..._ITEMS}}` with `<li>` bullets (source links inline). Empty area: replace the `<ul>` with `<p class="empty">Quiet day.</p>`. `{{NOTES}}` for unavailable sources (or remove).
5. In `index.html`, add a card right under `<!-- ARCHIVE: newest first -->`:
   `<a class="bcard" href="briefs/YYYY-MM-DD.html"><div class="d">DATE_LONG</div><div class="h">HEADLINE</div></a>`
6. No em-dashes. Commit and push to `main`.

## Sources
Core X follows added 2026-10-12 (verified active): @KentonVarda (Kenton Varda, Cloudflare Workers), @rough__sea (Ryan Dahl, Deno/Cloudflare), @ceo_clickhouse (Aaron Katz, ClickHouse CEO), @fabknowledge (Doug O'Laughlin, semis), @simonw (Simon Willison, AI/data tooling), @mustafasuleyman (Mustafa Suleyman, Microsoft AI).
Plus all handles listed in the routine prompt.
