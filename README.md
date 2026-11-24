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
- Ten claim rows, seven accounts. The payoff is late, not absent.
- H5 is the exploratory service-value path DICI → AIRI_S → service outcomes → ROA. H6 is MADI × DICI (N=7, not testable). H6b is AIRI_G × DICI.
- No causal claim. Replication is partial, not full.

## Provenance and limits

- Values are embedded from the v4 public package's result JSONs; the page performs no runtime `fetch`, and this repository ships no separate `claims.json`. The source paths are named in each Evidence row.
- H2: thesis §3.5 reports +0.211 pre-extension and +0.0009 for a 32-firm extension; the released-panel recomputation is +0.0841. These are different AIRI scales and must not be merged.
- H6b: the thesis/Python point is +4.9894; the package's stage3 JSON is +4.9785. The page displays +4.9894 and retains +4.9785 as a stage3 cross-check. The package README's Table 3 label needs correction.
- H7: γ .1464 (thesis), .0993 (released panel) and .1119 (Python grid) belong to different AIRI scales; attenuation percentages are not comparable across them.
- H9: the package reports four dynamic multipliers at t0–t3; the thesis prose calls the cumulative "three-period". The page displays the four-term package series and cum +24.81 through t3; do not sum only t0–t2.
- MADI coding sheets are an illustrative 0/1/2 reconstruction, not original keystroke-level coding.
- Firm names are anonymised; the public artifact carries no author name.
- The page is a public-facing research narrative, not the thesis document or a full replication package.

## Build status

The v4.2 page was audited at 1280×720 on 25 November 2026: 13/13 routes, 0 JS errors, 0 console errors, no canvas overflow. The deployed file is byte-identical to local SHA-256 `1e5beca6443953317c291e292bfe6a855faa4acd64e48437b517e83345349982` (2,628,784 bytes) at commit `3e72b6f`.

Interaction audit: 41/41 declared Evidence rows open with non-empty content — Q1–Q8 (8), Claims Ledger H1a–H9 plus H6b (10), Conventions (9), Replication (7), Explore (7). Each Q1–Q8 has its own READING and Source line; H6b keeps its dedicated six-value p-ladder drawer. No page has duplicate answers. Q1–Q8 `data-r`/`data-src`, the ten Ledger row `data-r`, and the original H6b drawer are preserved from commit `3fbc100`.

v4.2 corrections: Story 06 H8 denominator corrected from 27 to 32 firms; Controls drawer CFO denominator corrected to net operating cash flow / total assets; H6b stage3 +4.9785 labelled as a cross-check rather than "legacy must not be used"; Q/ledger active state follows the clicked row; inline favicon removes the `/favicon.ico` 404.

## Deployment

The page is served from this repository's own GitHub Pages endpoint, not from a sub-path of the profile site.

`https://kaito-ayano.github.io/The-Late-Payoff/`

The workflow publishes the committed `index.html` as the Pages artifact. The repository remains the public project record and source note; it does not ship the thesis document or the replication package.
