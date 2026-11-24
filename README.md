# The Late Payoff

A separate project page for an English data-story on digital-intelligent investment and financial performance in China's listed logistics firms, 2016–2025.

**Standalone project page:** https://kaito-ayano.github.io/The-Late-Payoff/

The page has two modes:

- **Story** — the narrative argument, from the panel to the ledger.
- **Evidence** — the auditable claim ledger, conventions, replication route and firm map.

The public artifact is a single self-contained HTML file: 1280×720 stage, font files embedded, no runtime `fetch`, no external assets. It is committed as `index.html` in this repository.

## What the page says

- 32 firms: 27 A-share and 5 HK; 309 firm-years in the 32×10 frame; 229 A-share firm-years with a constructible DICI; 7 MADI observations.
- HK is a separate strip (2017–2025; six calendar gaps; 2016 has no HK row); 2025 has rows but no DICI/AIRI, not zero.
- Ten claims, seven accounts. The payoff is late, not absent.
- H5 is the exploratory service-value path DICI → AIRI_S → service outcomes → ROA. H6 is MADI × DICI (N=7, not testable). H6b is AIRI_G × DICI.
- No causal claim. Replication is partial, not full.

## Provenance and limits

- Values are embedded from the v4 public package's result JSONs; the page performs no runtime `fetch`, and this repository ships no separate `claims.json`. The source paths are named in each Evidence row.
- H2: thesis §3.5 reports +0.211 pre-extension and +0.0009 for a 32-firm extension; the released-panel recomputation is +0.0841. These are different AIRI scales and must not be merged.
- H6b: the thesis/Python point is +4.9894; the package's stage3 JSON is +4.9785. The page displays +4.9894 and retains +4.9785 as a cross-check. The package README's Table 3 label needs correction.
- H7: γ .1464 (thesis), .0993 (released panel) and .1119 (Python grid) belong to different AIRI scales; attenuation percentages are not comparable across them.
- MADI coding sheets are an illustrative 0/1/2 reconstruction, not original keystroke-level coding.
- Firm names are anonymised; the public artifact carries no author name.
- The page is a public-facing research narrative, not the thesis document or a full replication package.

## Build status

The build was audited at 1280×720: 13/13 routes, 0 JS errors, no canvas overflow, and no author name in the HTML.

Interaction audit (25 November 2026): Q1–Q8 each open with their own READING and Source lines; all 10 Claims Ledger rows (H1a–H9 plus H6b) open a drawer, with H6b keeping its dedicated six-value p-ladder drawer; all 9 Conventions terms, 7 Replication routes and 7 Explore segments open a source drawer. The H5 ledger label is aligned with the thesis hypothesis (service-value path, not MADI → ROA). The combined target count is 41, all exercised at 1280×720.

## Deployment

The page is served from this repository's own GitHub Pages endpoint, not from a sub-path of the profile site.

`https://kaito-ayano.github.io/The-Late-Payoff/`

The workflow publishes the committed `index.html` as the Pages artifact. The repository remains the public project record and source note; it does not ship the thesis document or the replication package.
