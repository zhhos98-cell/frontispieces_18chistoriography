# Local carrier checkpoint — Meiners Round 2

Date: 2026-08-27
Status: `active_checkpoint`

## Purpose

Crash-safe restart point for the resumed Round 2 edition collation. This checkpoint records only verified carrier state and the immediate next tasks. Treat page-level interpretive conclusions below as provisional until each target leaf has been directly collated and then promoted into the main Round 2 log.

## Newly supplied local carriers

### 1785 first edition

User supplied:

- `Full text of _Grundriss der Geschichte der Menschheit,_(1).html`

Verified properties:

- saved Internet Archive full-text carrier;
- canonical IA item: `grundrissdergesc00mein`;
- this is the same 1785 first-edition IA carrier already mapped in the repo.

Carrier status:

`1785 full local text carrier = AVAILABLE`

### 1793 second edition

User supplied:

- `Grundriss_der_Geschichte_der_Menschheit(1).epub`

Verified mapping from the EPUB carrier / prior repo carrier map:

- Google Books ID: `vBsFAAAAYAAJ`;
- corresponding IA family already mapped as `grundrissderges01meingoog`;
- this is the 1793 second-edition carrier required by Round 2.

Carrier status:

`1793 full local EPUB/image-text carrier = AVAILABLE`

## Research-state change

Previous archived state:

`Round 2 = PAUSED because the public carriers were known but single-page automated retrieval was blocked.`

Current state:

`Round 2 = RESUMED because both edition carriers are now locally available.`

The old access-layer blockage is therefore no longer the operative constraint.

## Exact restart packet retained

Collate only the bounded Round 2 targets:

### 1785 first edition

- pp.23–24;
- p.39.

### 1793 second edition

- p.23;
- pp.59–60;
- p.85.

Round 2 questions remain:

1. 1785 pp.23–24 ↔ 1793 p.23: formulation history of the anti-single-body-part rule.
2. 1793 pp.59–60: literal scope and grammatical location of the Kantian race-definition module inside Meiners's existing taxonomy.
3. 1785 p.39 ↔ 1793 p.85: exact climate/`Abstammung` revision.

## Provisional warning from first-pass retrieval

The 1785 local carrier makes it possible to distinguish the already controlled p.17 anti-single/principal-colour criterion from the still-pending pp.23–24 body-part/skull formulation. Do not collapse these loci. The p.23–24 task must be settled from the primary text rather than inferred from modern page citations.

## Immediate next actions

1. Reconstruct printed-page mapping for the 1793 EPUB.
2. Extract and inspect 1793 p.23.
3. Extract and inspect 1793 pp.59–60.
4. Extract and inspect 1793 p.85.
5. Extract 1785 pp.23–24 and p.39 from the local IA full-text carrier.
6. Collate the three bounded questions.
7. Update `docs/RESEARCH_ROUND_2_OF_4_MEINERS_EDITION_HISTORY_CLOSURE_2026-08-27.md` and archive a final Round 2 closure checkpoint.

## Stop rules retained

- `citation ≠ adoption`;
- `module adoption ≠ system replacement`;
- `highest causal weight ≠ causal exclusivity`;
- `specific climate deletion ≠ disappearance of environmental causation`;
- `same printed page number across editions ≠ same wording`;
- `anti-single-colour criterion ≠ anti-single-body-part formulation`;
- do not reopen broad comparator searches during this bounded collation.
