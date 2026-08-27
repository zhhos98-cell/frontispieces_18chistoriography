# Archive checkpoint — Round 2 user-supplied carriers

Date: 2026-08-27
Status: `active_checkpoint`

## Purpose

Preserve the current state immediately after the user supplied two complete carriers for Christoph Meiners, *Grundriss der Geschichte der Menschheit*, so the edition-collation round can survive conversation/tool failure.

## User-supplied files

1. `Full text of _Grundriss der Geschichte der Menschheit,_(1).html`
   - Internet Archive full-text carrier;
   - canonical IA item visible in the file: `grundrissdergesc00mein`;
   - this matches the repo-controlled **1785 first-edition** carrier.

2. `Grundriss_der_Geschichte_der_Menschheit(1).epub`
   - complete EPUB supplied by the user;
   - preliminary carrier identification associates it with Google Books `vBsFAAAAYAAJ`, already recorded in the repo as an **1793 second-edition** carrier;
   - local metadata/content inspection remains the immediate verification step before promotion to primary-direct edition control.

## Existing Round 2 restart packet

The archived Round 2 document had reduced the remaining work to exactly six printed-page targets:

### 1785 first edition
- pp.23–24
- p.39

### 1793 second edition
- p.23
- pp.59–60
- p.85

The three bounded checks are:

1. 1785 p.23 ↔ 1793 p.23: formulation history of the anti-single-body-part rule;
2. 1793 pp.59–60: exact scope and grammar of the Kant citation/race-definition module within Meiners's Stamm/Race/Varietät/Spielart hierarchy;
3. 1785 p.39 ↔ 1793 p.85: exact passage-level climate/`Abstammung` revision.

## New state after upload

The previous retrieval-layer blockage is potentially removed: complete local carriers are now available rather than remote single-page access only.

The 1785 HTML directly exposes IA identifier `grundrissdergesc00mein`, matching the first-edition carrier map.

A caution already established in the repo remains important: the 1785 anti-single/principal-colour criterion is securely associated with p.17, while the modern-secondary pp.23–24 locus may concern a different bodily-evidence discussion. The p.23/24 ↔ 1793 p.23 task must therefore be literal formulation collation, not assumed sentence identity.

## Immediate next actions

1. Parse both supplied carriers locally and recover printed-page boundaries.
2. Extract the six target pages verbatim, retaining OCR uncertainty.
3. Collate 1785 pp.23–24 against 1793 p.23.
4. Reconstruct 1793 pp.59–60 and identify the exact Kant citation/definition and grammatical relation to Meiners's existing hierarchy.
5. Collate 1785 p.39 against 1793 p.85.
6. Update `docs/RESEARCH_ROUND_2_OF_4_MEINERS_EDITION_HISTORY_CLOSURE_2026-08-27.md` with primary-direct results and close Round 2 if all three checks resolve.

## Persistence rule for this session

Do not leave substantive intermediate results only in chat. Write repo checkpoints after each resolved page group or consequential correction, and leave a clean restart point before opening any new branch.
