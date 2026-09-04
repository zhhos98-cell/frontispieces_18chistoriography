# Full-repo density pass checkpoint — 2026-09-04

Status: **PAUSED FOR CONVERSATION HANDOFF — DO NOT RESTART FROM ZERO**

Purpose: record exactly where the article-density pass stopped. The user explicitly required a **true full-file traversal**, meaning every repository file must be opened and read for content, not merely filtered by tree/path/index records. The article remains source-locked and first-order `colour + book history`.

## Editing protocol already loaded

`AGENTS.md` was read from `main` and governs all subsequent work:

- source-locked historical expansion;
- surgical patching rather than paragraph regeneration;
- canonical draft only;
- chronology / actor clarity;
- complete event chains;
- no new second-order theory line;
- do not increase interpretive temperature merely for flow;
- distinguish event fact / source / historiography / inference;
- re-fetch current SHA before every write.

Canonical article draft:

`drafts/HLQ_COLOUR_BOOKHISTORY_ARTICLE_DRAFT_v5_SOURCE_INTEGRATED_2026-09-04.md`

Working branch:

`article-line-goettingen-nuremberg-return`

Branch head before this checkpoint:

`47b13e3b65affdebd6372093eb97d3e34e0890c0`

## Full-file traversal completed so far

### Root — COMPLETE

Every root text/state file was opened and read:

- `CLOSURE_STATE_2026-08-30.json`
- `CLOSURE_STATE_2026-08-31.json`
- `CURRENT_HANDOFF.md`
- `FINAL_CLOSURE_2026-08-30.md`
- `FINAL_CLOSURE_2026-08-31.md`
- `README.md`

Result: lifecycle/evidence guardrails only; no direct density insertion into the current HLQ article. Old Winckelmann/matrix-state lines remain closed and must not flow into this article merely because the repo is being traversed.

### `archive/` — COMPLETE

Every file in `archive/` and `archive/data_legacy_2026-08-30/` was opened and read, including all JSONL/CSV controls.

Result: mostly superseded/quarantined records and discovery trails. Historical correspondence/discovery records may explain how later controls were found but should not replace upgraded institutional/primary evidence. No direct article insertion should be made from legacy records unless the same fact is upgraded elsewhere in active controls.

### `data/` root — COMPLETE

Every file in `data/` root was opened and read, including the full Winckelmann/Winkelmann group.

Result:

- Winckelmann/Winkelmann lines are excluded from this article.
- Strong but out-of-scope `Evidenz`, genealogy-proof, anthropology, and methodological data should remain excluded.
- High-value first-order candidates found in active data include copy-level augmentation/colouring, production continuity, publisher distribution, reusable plate stock, and handbook/calendar recombination.

### `data/canonical/` — COMPLETE

Every canonical file was opened and read.

Result: canonical layer confirms that `colour as epistemic jurisdiction`, human variation, method-property, etc. belong to other frozen/closed branches and should not migrate into the HLQ article. The present article's strongest bounded contribution remains book/copy/host/decoder/rehosting/production history.

### `docs/` — PARTIAL, TRUE CONTENT PASS IN PROGRESS

Important: `docs/` has **not yet been completed**. Earlier in the pass some docs were read via blob/contents calls, then the user correctly required a true file-by-file content traversal. From that point forward, files are being opened directly with `fetch_file`.

Directly opened/read in the true content pass immediately before pause include:

- `COLOUR_METHOD_THIRD_SWEEP_ACTOR_LEVEL_JURISDICTIONS_2026-08-27.md`
- `COLOUR_METHOD_WILSON_WEB_SWEEP_LEGIBILITY_MATERIAL_CONSTRAINT_AND_EVIDENCE_REGIMES_2026-08-27.md`
- `COPY_AUGMENTATION_AS_PRIVATE_ARMORIAL_DATABASE_1747_1750_2026-08-26.md`
- `COPY_AUGMENTATION_WAPPENKALENDER_1747_2026-08-26.md`
- `ANNUAL_HANDBOOK_RECOMBINATION_GATTERER_1764_2026-08-26.md`

Earlier in this same conversation many additional active docs were also individually opened and read (not merely indexed), including the 2026-09-04 HLQ controls and several key production/copy notes, but the new conversation should **not assume `docs/` is complete** until every file in the docs tree has been individually opened once.

## High-value density candidates already found

These are candidates only. Do not patch them into the article until the full traversal is finished and competing candidates have been compared.

### 1. 1724 Wappenkalender as a denser annual object

The annual-history module control shows that annuals did not merely repeat genealogy/heraldry. Across 1724–32 they rotated substantial history modules (Bohemian, Austrian, French, Reich, peace-history, Danish, etc.). The 1724 object combined a colour-explanation plate, c.80 armorial images and c.100 genealogical tables with a historical module.

Potential use: enrich the first explanation of what a `Wappenkalender` actually was. Maximum 1–2 sentences; do not create a new section.

### 2. Copy-level augmentation, 1747

A 1912 catalogue describes a 1747 Wappenkalender owned by `A. W. von Arnstedt` in which more than 100 additional named eighteenth-century heraldic copper engravings had been cut out and lightly mounted on versos of the existing plates.

Potential use: strong copy-history control showing a Wappenkalender could become an expandable armorial reference object after publication.

Evidence guard: historical physical-copy catalogue description; present location unresolved.

### 3. Luxury coloured/augmented 1750 copy

A 1750 copy associated through its binding with Maria Josepha of Saxony is described with:

- engraved colour explanation;
- 108 armorial plates;
- plates coloured and heightened with gold and silver;
- additional coloured coats of arms pasted onto blank pages.

Potential use: very strong first-order evidence separating publisher-issued apparatus from copy-specific finishing and later augmentation.

Guard: provenance does not prove Maria Josepha personally ordered every intervention.

### 4. 1762 Gatterer *Handbuch* reader augmentation

The active copy-use controls preserve a 1762 Gatterer *Handbuch* copy with hand-drawn/coloured heraldic additions and source indications.

Potential use: brings reader-made colour/armorial augmentation directly into the Gatterer succession, rather than leaving copy augmentation only in the Köhler annuals.

Needs re-read of the exact active control before prose insertion.

### 5. 1764 `Fortgesetzter Wappen-Calender ... oder jährliches Handbuch`

The exact title explicitly recombines:

`Wappen-Calender` + `jährliches Handbuch`

and states that it contains rulers' genealogies and arms, correct armorial description, and an outline of heraldry.

Potential use: excellent chronological/format bridge between 1759 `Handbuch` and 1771/72 cumulative `Wappenbuch`. It materially shows the publication identity itself being recombined, without needing abstract `version governance` language.

### 6. Publisher/plate-stock continuity

Active controls show that Weigel/Tyroff/Raspe publication history includes retained/reused copper stock. A 1766 publisher statement includes the literal formulation `Die Kupfer waren also schon da` in a relevant reusable-plate context.

Potential use: one concrete production-history sentence, if the precise object/actor context remains directly relevant after re-reading the control. Do not generalise all plate continuity from this single case.

### 7. 1775 Raspe cumulative Wappenbuch gift/distribution

The Raspe control preserves evidence of publisher gift/distribution of the cumulative Wappenbuch in 1775.

Potential use: shows the cumulative Wappenbuch as an actively distributed object after the 1771/72 format transition, rather than only a title-state/bibliographical rehosting.

Needs exact source wording re-read before insertion.

### 8. Gatterer 1773/74 heraldic hatching system

Prior-art/control files establish that Gierl already describes Gatterer's 1773 Table I as combining Wappentopographie with black-and-white representation of tinctures. The 1774 p.12 passage then evaluates Rink's extra hatching signs via old `Wappenbriefe` and explicitly directs the reader to Köhler's programme on the history of hachures.

Potential use: strengthens Fig.8 / return section, but **do not alter Fig.8 or make a 1773→1774 plate comparison until the P0 direct page/plate comparison is actually closed**, per the user's new memo.

## Strong materials explicitly excluded despite density

The following were encountered and read but should not flow into this article merely because they are rich:

- human bodily colour / anthropology / race lines;
- Zimmermann, Meiners, Blumenbach, Girtanner;
- broad `colour as method`, `epistemic jurisdiction`, `distributed/stratified phenotype` arguments;
- full Gatterer `Evidenz` system;
- Linnaeismus/diplomatic-table measurement line unless used only in a tiny contextual note and absolutely necessary;
- Winckelmann/Winkelmann project;
- broad Leibniz/Reimmann source-routing material;
- Clio/frontispiece ontology and matrix-state work.

## Next conversation: exact restart point

1. Re-fetch branch head and current canonical draft SHA.
2. Re-fetch `docs` tree.
3. Continue **true file-by-file `fetch_file` reading** through every remaining `docs/` file. Do not treat the tree listing itself as traversal.
4. Then individually open every file in:
   - `drafts/`
   - `schema/`
5. Only when every repository file has actually been read should the density patch be assembled.
6. Build one candidate table internally with:
   - source file;
   - exact historical fact;
   - evidence status;
   - target paragraph in canonical draft;
   - whether it increases first-order density or creates a second-order detour.
7. Patch only the strongest candidates in one controlled batch.
8. Re-read the full canonical draft after patching to check chronology, actor clarity, name density, and whether any insertion raises interpretive temperature.

## Current article principle

Keep the article literal:

- colour can be named without being printed;
- encoded by letters or hatching;
- supplied through a monochrome key;
- added by hand;
- lost at copy level;
- augmented by owners;
- rehosted in later formats;
- applied to historical tables.

Do not convert this into a theory of `knowledge production` or a generalized claim that colour/relations/epistemic operators were `made`.
