# Local carrier checkpoint — Meiners Round 2

Date: 2026-08-27
Status: `active_checkpoint`

## Purpose

Crash-safe restart point for the resumed Round 2 edition collation. This checkpoint records verified carrier state plus completed local-page inspections. Locator conflicts are preserved rather than silently harmonised.

## Newly supplied local carriers

### 1785 first edition

User supplied:

- `Full text of _Grundriss der Geschichte der Menschheit,_(1).html`

Verified properties:

- saved Internet Archive full-text carrier;
- canonical IA item: `grundrissdergesc00mein`;
- same 1785 first-edition IA carrier already mapped in the repo.

Carrier status:

`1785 full local text carrier = AVAILABLE`

### 1793 second edition

User supplied:

- `Grundriss_der_Geschichte_der_Menschheit(1).epub`

Direct EPUB metadata verifies:

- title: `Grundriss der Geschichte der Menschheit`;
- author: Christoph Meiners;
- publisher: `im Verlage der Meyerschen Buchhandlung`;
- Google Books ID: `vBsFAAAAYAAJ`;
- preface explicitly dates itself `Göttingen am 6ten März 1793`;
- title OCR reads `Zweyte sehr verbesserte Ausgabe`.

This is the 1793 second-edition carrier required by Round 2 and corresponds to the repo-mapped Google/IA family.

Carrier status:

`1793 full local EPUB/image-text carrier = AVAILABLE`

## Research-state change

Previous archived state:

`Round 2 = PAUSED because the public carriers were known but single-page automated retrieval was blocked.`

Current state:

`Round 2 = RESUMED because both edition carriers are now locally available.`

The old access-layer blockage is no longer the operative constraint.

## Completed local inspection: 1793 pp.59–60

This target is now primary-direct from the user-supplied EPUB.

### p.59

The paragraph begins:

`Alle Völker der Erde machen zwar nur ein einziges Geschlecht, oder eine einzige Art (species) von Geschöpfen aus; allein in diesem einzigen Menschengeschlecht muß man zwen ganz verschiedene Stämme ...`

The sentence continues onto p.60.

### p.60

The hierarchy is directly present:

`ein einziges Geschlecht / species`
→ `zwei ganz verschiedene Stämme`
→ `in jedem Stamm mehrere Racen`
→ `in jeder Race unzählige Varietäten`
→ `Spielarten` produced by mixture across different Stämme and Racen.

Immediately after that hierarchy Meiners repeats the anti-single-colour rule:

`Sonderbar scheint es mir, daß man die Farbe zum einzigen oder vornehmsten Merkmahle wählte, nach welchem man die Aehnlichkeit und Verschiedenheit von Völkern zu bestimmen habe.`

The note attached to `Racen` says, in OCR-normalised substance:

`Ich wünschte, daß die Wörter Stamm und Race schon eine bestimmte Bedeutung gehabt hätten. Vielleicht würden viele da, wo ich Stamm setze, lieber Race, und umgekehrt gebraucht haben. S. Kants Abh. im Novemb. der Berl. Monatsschrift vom Jahr 1785.`

The Google OCR misreads `Kants` as `Rants`; the bibliographic phrase nevertheless identifies Kant's November 1785 *Berlinische Monatsschrift* essay unambiguously.

Primary-direct consequence:

`1793 Kant uptake = local terminological/definitional comparison attached to the Stamm/Race distinction, inside a pre-existing Meiners hierarchy.`

This directly supports the repo's selective/module-uptake model and rules out treating the citation itself as wholesale Kantianization.

Status:

`1793 pp.59–60 = PRIMARY-DIRECT CLOSED`

## Locator conflict 1: 1793 p.23

Direct inspection of Google page anchor `GBS.PA23` in the 1793 carrier shows a methodological passage contrasting `Geschichte der Menschheit` with Universalhistorie. It states that the former can juxtapose nations, actions and events separated by time and space, then begins a definition of the new science.

The directly inspected p.23 does **not** contain the skull / isolated-body-part formulation expected from the current specialist-page locator in the Round 2 log.

Therefore:

`1793 p.23 body-part locator = CONFLICTING WITH LOCAL PRIMARY CARRIER`

Do not promote the modern p.23 locator to primary-direct. Search the 1793 full carrier for the actual body-part/skull formulation before deciding whether this is a citation error, pagination mismatch, or wording/OCR problem.

## Locator conflict 2: 1793 p.85

Direct inspection of `GBS.PA85` shows a passage on bodily strength, diet, hardening, and the different effects of climate and food. It does not contain the expected passage-level revision foregrounding `Abstammung`.

The immediately preceding p.84 does explicitly say that the effects of climate on the human body are highly indeterminate/contradictory and that neither food nor climate produces uniform effects across countries and nations. But p.85 itself is not the currently expected descent-revision passage.

Therefore:

`1793 p.85 Abstammung locator = CONFLICTING WITH LOCAL PRIMARY CARRIER`

Do not silently reconcile this with the Bernasconi-derived locator. Search the full 1793 carrier for the actual revised wording and then compare with 1785.

## Exact remaining work

1. Extract 1785 pp.23–24 and determine what those pages actually contain.
2. Search both editions for the skull / isolated-body-part formulation; establish its true page locus and formulation history.
3. Extract 1785 p.39.
4. Search the 1793 carrier for the `Abstammung` / climate revision and establish its true page locus.
5. Collate the first-edition wording against the actual second-edition locus.
6. Correct the main Round 2 log rather than forcing the old six-page packet if the secondary locators prove wrong.
7. Close Round 2 only after these locator conflicts are resolved or bounded explicitly.

## Stop rules retained

- `citation ≠ adoption`;
- `module adoption ≠ system replacement`;
- `highest causal weight ≠ causal exclusivity`;
- `specific climate deletion ≠ disappearance of environmental causation`;
- `secondary page locator ≠ primary page identity`;
- `same printed page number across editions ≠ same wording`;
- `anti-single-colour criterion ≠ anti-single-body-part formulation`;
- preserve locator conflicts as evidence problems; do not normalize them away.
