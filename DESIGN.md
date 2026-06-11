# Design

## Concept

**«Проверено» — the graded page.** The site is a manuscript worked over by
an exacting proofreader. The product's own output is the design system:
red correction marks, monospace schema tags, §-references in the margin.

## Color

Strategy: **Committed** — red carries the surface; everything else is ink
on paper. Named reference: teacher's red pen on white exercise paper.

| token | light | dark | role |
|---|---|---|---|
| `--bg` | `oklch(0.99 0 0)` ≈ #fcfcfc | `oklch(0.17 0.005 80)` ≈ #16140f | paper. True neutral — never cream |
| `--ink` | #181512 | #ece8e2 | body text |
| `--ink-soft` | #43403c | #b6b1aa | secondary text (≥4.5:1 kept) |
| `--muted` | #6e6a64 | #8d8780 | captions, timestamps |
| `--red` | #b3261e | #ff7b72 | the pen: marks, links, rules, bands |
| `--red-ink` | #8c1d17 | #ff8f87 | red on tinted surfaces |
| `--red-wash` | `color-mix(red 6%, bg)` | `color-mix(red 12%, bg)` | annotation backgrounds |
| `--rule` | #e4e1dc | #353129 | hairlines |

Red band (`.band`): solid `--red`, white text (≈5.7:1).

## Typography

- **Literata** (variable; latin+cyrillic) — body AND display. Bookish,
  contemporary, real Cyrillic. Display: weight 600–700, tight opsz.
- **PT Mono** — tags, dates, nav, code. ParaType is the Russian state
  type commission's foundry; mono is the product's native register
  (CLI tags), not costume.
- No third family. Contrast axis: serif ↔ mono.
- Body 18px/1.6, max 65ch. Display clamp ceiling 4.2rem.

## Marks system (the brand's own grammar)

- `del` — red strikethrough (animated draw on load; static when
  reduced-motion).
- `ins` — red, raised above the line with a caret `‸` at the insertion
  point, like a handwritten interline correction.
- `.tag` — PT Mono, red-wash background pill, the real synterr subtype.
- `.para-ref` — §-reference in PT Mono (e.g. `§152`), the citation grammar
  borrowed from Rozental. Used as the section-marker system on the
  homepage offerings ledger — a deliberate, named brand system, used in
  ONE place, not on every heading.

## Layout

- Content widths: prose 42rem, wide 66rem.
- No cards, no three-up grids. The offerings are a ledger: asymmetric
  rows with §-markers, generous row spacing, hairline separators.
- One full-width red band per page maximum (the featured-paper statement).
- Header: wordmark + PT Mono nav, double hairline rule below (editorial).
- Footer: single hairline, mono.

## Motion

One orchestrated load sequence in the hero only: strike draws (320ms
ease-out-quart, 250ms delay), then the inserted word and caret fade/rise
(240ms). Everything visible by default; animation only adds the drawing.
`prefers-reduced-motion`: no animation, marks fully rendered.

## Banned on this site

Cream/parchment backgrounds · uppercase tracked kickers · side-stripe
borders · → link arrows · icon card grids · gradient text · glassmorphism.
