# Archive checkpoint — Round 2 user-supplied carriers

Date: 2026-08-27
Status: `active_checkpoint`

## Purpose

Preserve the current state immediately after the user supplied two complete carriers for Christoph Meiners, *Grundriss der Geschichte der Menschheit*, so the edition-collation round can survive conversation/tool failure.

## User-supplied files

1. `Full text of _Grundriss der Geschichte der Menschheit,_(1).html`
   - Internet Archive full-text carrier;
   - canonical IA item visible in the file: `grundrissdergesc00mein`;
   - title page OCR directly gives Lemgo, Meyersche Buchhandlung, **1785**;
   - this is the repo-controlled **1785 first edition**.

2. `Grundriss_der_Geschichte_der_Menschheit(1).epub`
   - complete Google Books EPUB supplied by the user;
   - OPF metadata directly gives title, author Christoph Meiners, publisher `im Verlage der Meyerschen Buchhandlung`, and Google identifier **`vBsFAAAAYAAJ`**;
   - this is the repo-controlled **1793 second-edition carrier**;
   - EPUB contains an explicit printed-page map, allowing direct extraction by printed page rather than scan-offset inference.

## Existing Round 2 restart packet

The archived Round 2 document had reduced the remaining work to exactly six printed-page targets:

### 1785 first edition
- pp.23–24
- p.39

### 1793 second edition
- p.23
- pp.59–60
- p.85

The three proposed checks were:

1. 1785 p.23 ↔ 1793 p.23: formulation history of the anti-single-body-part rule;
2. 1793 pp.59–60: exact scope and grammar of the Kant citation/race-definition module within Meiners's Stamm/Race/Varietät/Spielart hierarchy;
3. 1785 p.39 ↔ 1793 p.85: exact passage-level climate/`Abstammung` revision.

## Primary-direct correction 1 — the p.23/24 ↔ p.23 mapping fails

Direct inspection falsifies the inherited page-locus assumption.

### 1785 pp.23–24

These pages are in the ethnographic/descent sequence on northern Eurasian peoples. They discuss, among other material:

- Samoyeds, Ostiaks, Lapps, Finnic peoples and related groups;
- Tungusic-derived peoples;
- migration/population links toward North America;
- climatic harshness in Dauria and related regions.

They do **not** contain the later anti-isolated-body-part sentence attributed in specialist secondary discussion.

### 1793 p.23

This page is still in Meiners's methodological definition of `Geschichte der Menschheit`. It contrasts the new field with Universalhistorie: Universalhistorie follows chronological order, whereas the history of humankind juxtaposes nations, actions and events separated by time and space; Meiners then begins a formal definition of the science.

Therefore:

`1785 pp.23–24 ≠ textual antecedent of 1793 p.23 anti-body-part wording`.

Indeed, on this controlled 1793 carrier, **p.23 itself does not contain that anti-body-part wording**.

This is a consequential citation/page-mapping correction. The specialist quotation/page reference previously relied upon must be rechecked against its exact cited work/edition rather than propagated into the primary corpus.

Do not infer an OCR-offset problem: both user-supplied carriers expose explicit title/edition identity, and the 1793 EPUB has a printed-page map.

## Primary-direct result 2 — 1785 p.39 ↔ 1793 p.85

This comparison resolves a real passage-level revision more precisely than the earlier shorthand `climate → descent`.

### 1785 p.39

The first edition states, in OCR-normalised substance:

- bodily effects of climate are highly variable and apparently contradictory;
- diet and climate do not produce uniform effects in all lands and nations;
- `Abhärtung` is something different from bodily strength;
- `Abhärtung` is to some degree a consequence of exercise and way of life;
- **more importantly, it is an `Eigenthümlichkeit gewisser Stämme, Racen und Klimate`.**

The crucial first-edition structure is therefore:

`Abhärtung = partly acquired by practice/life + also an Eigenthümlichkeit of Stämme, Racen, and Klimate`.

### 1793 p.85

The second edition rewrites the distinction:

- `Härte ist etwas ganz anders, als Stärke`; one may exist without the other;
- `Abhärtung` is in a certain degree a consequence of exercise and way of life;
- **`Härte hingegen ist eine Eigenthümlichkeit gewisser Stämme, und Racen`.**

The revision does three things at once:

1. separates acquired/produced `Abhärtung` from `Härte` more sharply;
2. assigns `Härte` rather than `Abhärtung` to inherited/group-specific classificatory units;
3. removes **`Klimate`** from the `Eigenthümlichkeit` clause, leaving only `Stämme` and `Racen`.

This is primary-direct evidence for a local redistribution of explanatory weight toward lineage/classificatory group, but it is more exact to describe it as a **conceptual split plus deletion of climate from the hardness-as-property clause** than as a global substitution of descent for climate.

Safe formulation:

`1785: Abhärtung partly acquired, yet also property of Stämme/Racen/Klimate`
→ `1793: Abhärtung acquired; Härte instead property of Stämme/Racen`.

This supports the repo stop rule:

`specific climate deletion/reassignment ≠ disappearance of environmental causation elsewhere`.

## 1793 pp.59–60 — primary text now locally accessible

The page map places both target pages in `content-0048.xml`.

Direct OCR confirms on p.59:

`Alle Völker der Erde` form one `Geschlecht` / `Art (species)`, within which Meiners posits two distinct `Stämme`.

P.60 continues:

`in jedem Stamm mehrere Racen` → `in jeder Race unzählige Varietäten` → many `Spielarten` arising from mixture of people from different Stämme and Racen.

The anti-single-colour sentence is present immediately afterward: Meiners calls it strange to choose colour as the sole or principal mark by which similarity and difference of peoples are to be determined.

The p.60 note then states that Meiners wished `Stamm` and `Race` already had fixed meanings; others might reverse his usage, followed by the explicit reference to **Kant's essay in the November 1785 Berlinische Monatsschrift**.

Thus the primary grammar already strongly supports the modular reading:

`Meiners taxonomy first` + `terminological caveat about Stamm/Race` + `Kant reference in that caveat`.

The Kant citation is attached directly to terminology/definition at the Stamm/Race distinction; it does not interrupt or replace the larger hierarchy already stated in the main text.

A final exact transcription/normalisation check against the 1785 p.17 anti-single-colour passage remains in progress before Round 2 closure.

## Immediate next actions

1. recover and transcribe 1785 p.17 from the first-edition OCR;
2. collate its anti-single/principal-colour sentence against 1793 p.60;
3. inspect adjacent 1785 pp.38–39 and 1793 pp.84–85 to define the full boundaries of the hardness/climate rewrite;
4. repair `docs/RESEARCH_ROUND_2_OF_4_MEINERS_EDITION_HISTORY_CLOSURE_2026-08-27.md`, especially the now-falsified p.23 mapping;
5. close Round 2 if no additional primary ambiguity remains.

## Persistence rule for this session

Do not leave substantive intermediate results only in chat. Write repo checkpoints after each resolved page group or consequential correction, and leave a clean restart point before opening any new branch.
