# MEGA.dev S01E03 — what it shows

Local replay of a challenge already accepted by the course on 2026-10-28. This repository preserves the supplied knowledge base, a signed review page, and the static rendered site. It does not claim a new course solve.

## Review

- [Signed review source](src/routes/kb/incidents/4471-review/+page.svx)
- [Rendered review HTML](build/kb/incidents/4471-review.html)
- [Original incident](src/routes/kb/incidents/4471/+page.svx)
- [Export conventions](README-export.md)

The original CauseTable component renders 412 unique reports: 379 parser and 33 hint. The five desk-noted symptom reports remain within parser; the investigation count overlaps, rather than adding five reports.

## Tickets and desk update

- [#1 Parser — 379 reports](https://github.com/jwilk123/mega-s01e03-replay/issues/1): engineering reports fixed.
- [#2 Hint — 33 reports](https://github.com/jwilk123/mega-s01e03-replay/issues/2): won't fix because booking-v3 was retired.
- [#3 Investigation — five overlapping reports](https://github.com/jwilk123/mega-s01e03-replay/issues/3): unresolved symptoms; no proved root cause.

The live challenge update says #4471 closed 05 October. The kb export predates that update. Accepted decision record 0001 is preserved unchanged.

## Build and view

Requires Node.js and npm. From the repository root:

```sh
npm ci
npm run build
npm run preview -- --port 4173
```

Open http://127.0.0.1:4173/kb/incidents/4471-review. The `build/` directory contains the complete static site. Serve it locally to see the desk's rendered view; GitHub's code view displays the HTML source.

The page computes counts with the original components and carries the course-issued frontmatter signature and RenderStamp. Dependency folders, package caches and private session logs are excluded.
