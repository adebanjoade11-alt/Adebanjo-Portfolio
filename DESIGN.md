# Design

Visual system for `portfolio-v2/` (the new portfolio). The older `site/` keeps its own dark "field record" look and is not governed by this file.

## World

An engineer's drawing set. Three ideas combined at the owner's request:

1. **Feeder diagram**: a single-line electrical diagram is the organising graphic. The hero is a drawn 33 kV busbar feeding three loads (Networks & O&M, Construction, IT & systems), and a vertical feeder line runs down the page on desktop with a circuit-breaker symbol (square with a cross) at the head of every section.
2. **Infrastructure prospectus**: editorial type, generous measure, the owner's own site photographs set large with plain captions.
3. **Programme schedule**: the career drawn as a Gantt chart (bars for roles, diamonds for milestones) and an S-curve for the solar PV capital project, labelled as an illustrative shape.

## Tokens

| Token | Value | Use |
|---|---|---|
| `--paper` | `#f4f1ea` | page (drafting paper) |
| `--paper-2` / `--paper-3` | `#ebe6da` / `#e2dccd` | header cells, chips, image wells |
| `--ink` | `#13213a` | text, linework, contact band |
| `--ink-2` | `#46526b` | secondary text (6.9:1 on paper) |
| `--rule` | `#cdc5b3` | hairlines |
| `--red` / `--yellow` / `--blue` | `#b3302a` / `#d99a1e` / `#2856a3` | phase colours: networks / construction / IT and study. Yellow is never used for text on paper. |

## Type

- Display: Archivo (variable width; condensed 72–90% for headings).
- Reading: Source Serif 4.
- Data: IBM Plex Mono, only for dates, measurements, labels in diagrams and the schedule.

## Rules

- Graphics are authored SVG geometry (diagrams, charts), never imitation pictures. Illustrative charts say so in the caption.
- One animation: the hero diagram energises (lines draw in, then current flows). Off under reduced motion.
- No eyebrow labels above headings; the breaker symbol does that job.
- Photos: `img/<name>-t.webp` thumbnails, `img/<name>.webp` full size. Camera watermarks are cropped out of the files themselves, not hidden with CSS.
