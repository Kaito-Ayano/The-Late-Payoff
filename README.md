# The Late Payoff

A separate project page for an English data-story on digital-intelligent investment and financial performance in China's listed logistics firms, 2016–2024.

**Standalone project page:** https://kaito-ayano.github.io/The-Late-Payoff/

The page has two modes:

- **Story** — the narrative argument, from the panel to the ledger.
- **Evidence** — the auditable claim ledger, conventions, replication route and firm map.

The public artifact is a single self-contained HTML file: 1280×720 stage, font files embedded, no runtime `fetch`, no external assets. It is committed as `index.html` in this repository.

## What the page says

- 32 firms: 27 A-share and 5 HK; 229 A-share firm-years, 2016–2024.
- HK is a separate strip; 2025 is an empty column, not a zero.
- Ten tests, seven accounts. The payoff is late, not absent.
- No causal claim. Replication is partial, not full.

## Provenance and limits

- Values are read from the frozen `claims.json` under `TLP-DATA-v1`.
- Firm names are anonymised; the public artifact carries no author name.
- The page is a public-facing research narrative, not the thesis document or a full replication package.

## Build status

The local build was audited at 1280×720: 13/13 routes, 0 JS errors, no canvas overflow, and no author name in the HTML.

## Deployment

The page is served from this repository's own GitHub Pages endpoint, not from a sub-path of the profile site.

`https://kaito-ayano.github.io/The-Late-Payoff/`

The workflow publishes the committed `index.html` as the Pages artifact. The repository remains the public project record and source note; it does not ship the thesis document or the replication package.
