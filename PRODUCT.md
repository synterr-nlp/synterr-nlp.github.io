# Product

## Register

brand

## Users

GEC/NLP researchers, reviewers following the BEA 2026 paper link, and
potential users of synterr (Russian-NLP practitioners). They arrive
skeptical, scan fast, and judge rigor from the first viewport. Secondary:
collaborators and students sent here as the project's front door.

## Product Purpose

The public face of synterr-nlp: open Russian GEC research — rule-grounded
synthetic error generation, per-rule diagnostics, reproducible pipelines.
The site must make one impression: these people are exacting. Success =
a visitor reads the hero, understands the per-rule thesis in ten seconds,
and clicks through to the paper or the code.

## Brand Personality

Exacting, red-penned, bilingual. The voice of a careful proofreader:
confident corrections, no hedging, receipts attached. Copy is already
strong ("evaluated honestly", "What Aggregate Scores Hide") — design must
match its nerve.

## Anti-references

- The 2025–26 "tasteful AI academic" template: cream/parchment background,
  one muted accent, tiny uppercase tracked kickers over every section,
  three rule-separated text columns, → arrows on links. (This is what the
  previous design was; it was called slop. Never return.)
- SaaS landing grammar: hero metrics, gradient text, icon card grids.
- Generic "lab website" sterility with no domain identity.

## Design Principles

1. **The artifact is the identity.** GEC is proofreading; the design system
   is built from the product's own output — correction marks (del/ins),
   schema tags, Rozental §-references, dependency arcs. Nothing decorative
   that the tool couldn't have produced.
2. **The red pen is earned.** Red is not an accent, it is the actor: it
   strikes, inserts, annotates. Use it like a proofreader, not a painter.
3. **Show a correction before claiming correctness.** The hero demonstrates
   the product on a real Russian sentence before any copy asserts anything.
4. **Russian is content, not flavor.** Cyrillic examples are real synterr
   output with real tags; never lorem-Russian.
5. **Honest receipts.** Every claim links to data (per-rule tables,
   provenance, checksums). Design makes the receipts visible, not buried.

## Accessibility & Inclusion

WCAG AA. Body text ≥4.5:1 in both themes. Dark/light themes maintained.
All correction-mark animation behind prefers-reduced-motion with a static
default that is fully legible (marks visible without animation). Semantic
del/ins markup so corrections read correctly in screen readers. lang="ru"
on Russian content.
