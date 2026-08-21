# Frontispieces and Eighteenth-Century Historiography

A provenance-first corpus for tracking engraved frontispieces, their reissue across publication formats, and the wider Nuremberg print networks in which historical, genealogical, heraldic, antiquarian, and natural-historical evidence was organised.

## Research question

The seed case is the recurring engraved Clio frontispiece associated with the Weigel publishing constellation and Johann Christoph Gatterer's *Handbuch der neuesten Genealogie und Heraldik* (1762). Rather than treating a frontispiece as a single iconographic object, this repository treats it as a **serial artefact**: a plate or plate-family that can be reissued, altered, relabelled, repositioned, and embedded in different rhythms of consultation.

The working hypothesis is therefore operational rather than purely iconographic: changes in attributes, inscriptions, spatial arrangement, format, placement, and publishing context may record changes in how readers were expected to gather, check, compare, remember, and navigate evidence.

## Corpus unit

The preferred atomic unit is a **witness occurrence**: one verifiable appearance of a plate or closely related plate-state in one publication context and, where possible, one identified copy.

The corpus separates:

1. `plate_series` — a recurring design/plate lineage across impressions and formats;
2. `witness` — one publication occurrence of that plate or plate-state;
3. `copy` — a specific surviving institutional or digitised copy;
4. `agent` — designer, engraver, publisher, printer, author/editor, firm, heir, dealer;
5. `feature` — inscription, attribute, object, layout relation, scale, placement;
6. `source_evidence` — catalogue record, review, correspondence, scan, archival record, digitisation;
7. `relationship` — reuse, probable reuse, variant-of, derived-from, same-plate-as, publisher-succession, production association.

A bibliographic lead is not promoted to a witness until the relevant front matter or plate has been inspected.

## Current seed

### Core Clio series

The initial plate-series record groups the recurring frontispiece with the inscription:

> *Historia. Genealogia. Heraldica. Testes temporum et veritatis.*

The current research draft attributes the design to Gabriel Müller, engraving to Martin Tyroff, and issue to the heirs of Christoph Weigel. It describes surviving variants across calendar and handbook formats and identifies changes in attributes, inscriptions, and spatial arrangement. The 1762 Gatterer handbook is therefore entered as a core witness; the calendar material remains a witness cluster pending issue-by-issue enumeration.

### Extended Nuremberg network

Private research correspondence with the Germanisches Nationalmuseum (GNM) produced a 35-entry holdings list for Christoph Weigel and Martin Tyroff. These records are ingested as **bibliographic leads**, not as evidence that they contain the Clio plate. They deliberately widen the comparison set across:

- biblical image series and mnemonic history;
- professions, costume, and social orders;
- legal and civic print;
- natural history;
- numismatics;
- emblematic and heraldic engraving;
- historical chronologies and memory aids.

This wider set allows the project to ask whether recurrent graphic operations—juxtaposition, seriality, tabulation, mnemonic compression, classificatory ordering, evidentiary display—travel across genres in the Weigel–Tyroff production network.

## Evidence levels

Every record should carry one of these statuses:

- `verified_primary` — inspected in the object, scan, or reliable primary transcription;
- `verified_catalogue` — grounded in a catalogue/finding aid but object not yet inspected;
- `reported_correspondence` — reported by an archive/library in research correspondence;
- `research_inference` — an explicit analytical inference;
- `unresolved` — identity, date, plate-state, or relationship requires checking.

See [`docs/EVIDENCE_POLICY.md`](docs/EVIDENCE_POLICY.md).

## Repository layout

```text
README.md
schema/
  record.schema.json
data/
  core_records.jsonl
  gnm_holdings_seed.csv
  research_leads.csv
docs/
  EVIDENCE_POLICY.md
```

## Immediate work queue

1. Enumerate every surviving issue/copy of the *Geschichts-, Geschlechts- und Wappen-Kalender* that carries the Clio frontispiece.
2. Capture page-opening context, not only cropped images: binding, title/front matter sequence, recto/verso, plate placement, surrounding typography.
3. Compare the 1762 Gatterer witness against calendar impressions at feature level.
4. Resolve the Weigel authority problem before normalising agent IDs: correspondence explicitly warns of name confusion among Johann Christoph/Christoph Weigel family members.
5. Track the publishing-business succession from the Weigel household into Martin and Johann David Tyroff as a relationship graph, rather than flattening all imprints to one publisher name.
6. Use the GNM lead set to identify control cases where Tyroff or Weigel deploys analogous visual operations outside genealogy/heraldry.
7. Add review/advertising evidence (including *neu vermehrt und verbessert*) as dated source records linked to specific issues where possible.

## Inclusion rule

The corpus is intentionally broader than “frontispieces depicting Clio,” but narrower than “all eighteenth-century Nuremberg engraving.” A record belongs when it can help reconstruct at least one of the following:

- a plate's material/serial history;
- a publishing or engraving relationship relevant to the plate network;
- a comparable visual procedure for organising evidence;
- the circulation, consultation, or re-use conditions of relevant printed apparatus.

## Privacy and provenance

Raw Gmail messages, addresses, and unpublished attachments are **not** mirrored into this public repository. Correspondence-derived facts are stored only as sanitised source notes with institution, date, claim type, and verification status. Original messages remain in the private mailbox as provenance.