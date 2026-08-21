# Frontispieces and Eighteenth-Century Historiography

A provenance-first corpus for tracking engraved frontispieces, their reissue across publication formats, and the wider Nuremberg print networks in which historical, genealogical, heraldic, antiquarian, and natural-historical evidence was organised.

## Research question

The seed case is the recurring engraved Clio frontispiece associated with the Weigel publishing constellation and Johann Christoph Gatterer's *Handbuch der neuesten Genealogie und Heraldik*. Rather than treating a frontispiece as a single iconographic object, this repository treats it as a **serial artefact**: a plate or plate-family that can be reissued, altered, relabelled, repositioned, detached, and embedded in different rhythms of consultation.

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

The current research draft attributes the design to Gabriel Müller, engraving to Martin Tyroff, and issue to the heirs of Christoph Weigel. These production roles remain provisional. The first external web sweep repeatedly corroborated the serial survival of the design but did **not** independently corroborate the Gabriel Müller attribution; this must be resolved from signatures, production records, or stronger catalogue evidence rather than repeated secondary metadata.

### First web-sweep result: a visual regime change, not simple repetition

The most important result of the 21 August 2026 sweep is that the target allegory should not be projected backwards across the entire calendar series.

- A **1724** copy is independently described with an annual historical-memory frontispiece, *Gedenckwürdigkeiten des 1722ten Jahres*.
- By **1726**, surviving auction imagery visibly shows the familiar *Historia Genealogia Heraldica* allegory.
- A detached example dated ca. **1737** by an antiquarian seller survives as a loose print, preserving the full *Testes temporum et veritatis* inscription and reported traces of former attachment to a book.
- A **1744** complete-copy description explicitly identifies the engraved frontispiece as *Historia Genealogia Heraldica*.
- A **1759** Gatterer *Handbuch* copy explicitly transcribes the same pretitular inscription.
- A **1764** *Fortgesetzter Wappen-Calender* copy again explicitly names *Historia Genealogia Heraldica: Testes Temporum Et Veritatis*.

The immediate problem is therefore to date and explain the replacement of an **annual-event / mnemonic frontispiece** by a **reusable abstract allegory of Historia–Genealogia–Heraldica**. Current web evidence brackets the change between 1724 and 1726; **1725 is the priority transition witness**.

This is potentially more important than a simple reprint census. If confirmed by direct scan comparison, the front matter itself shifted from retrospectively picturing memorable events to repeatedly staging the evidentiary operations by which historical truth was to be checked.

### Serial extent now under investigation

Authoritative serial catalogues establish the original Weigel calendar for **1723–1757**. The first sweep also reconstructs a longer successor sequence:

- 1723–1757 — *Geschichts-, Geschlechts- und Wappen-Calender*;
- 1759–1763 — Gatterer, *Handbuch der neuesten Genealogie und Heraldik*;
- 1764–1766 — *Fortgesetzter Wappen-Calender ... oder jährliches Handbuch*;
- 1767 onward — Seyfart continuation and later *Handbuch* / *vollständiges Wappenbuch* forms, with related surviving objects into the 1770s.

The Clio design is positively attested online across the Weigel-calendar, Gatterer-handbook, and Gatterer/Raspe continued-calendar phases. Its survival into the Seyfart phase remains open.

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

Particularly important controls currently include the 1696–97 *Gedächtnuß-hülffliche Bilder-Lust*, the 1698 *Sculptura Historiarum Et Temporum Memoratrix*, Köhler's weekly *Historische Münz-Belustigung* from 1729, the 1748 Oetter rare-coin tract, Rösel's 1758 frog natural history, and the 1766 *Grösse und Mannigfaltigkeit in den Reichen der Natur und Sitten*.

## Material afterlives and copy variation

The sweep has already shown why `copy` cannot be collapsed into `edition`:

- a 1738 auction copy explicitly lacks its frontispiece;
- a ca. 1737 target frontispiece survives detached from its former book;
- armorial leaves from the series circulate today as loose prints while retaining genealogical tables on the verso;
- historical collectors cut calendar plates out and recombined them into manuscript armorial collections;
- annotated genealogical tables occur in surviving copies.

The corpus should therefore preserve material states such as `detached_plate`, `cut_and_reused`, `rebound_composite`, `annotated_copy`, and `frontispiece_missing` rather than treating them as damage/noise.

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
  web_witness_records.jsonl
  wappenkalender_witness_census.csv
  gnm_holdings_seed.csv
  research_leads.csv
docs/
  EVIDENCE_POLICY.md
  WEB_SWEEP_2026-08-21.md
```

## Immediate work queue

1. **Transition sweep first:** inspect complete front matter for 1723, 1724, 1725, 1726, 1727, and 1728; establish exactly when the target Clio design enters the serial.
2. Expand the census issue by issue through 1757 using BSB/MDZ, Düsseldorf, Rostock and other surviving copies; record frontispiece identity, placement, dimensions, signature and copy condition.
3. Compare plate-state evidence at 1726, 1736/37, 1744, 1759 and 1764: lettering, dimensions, line breaks, signature, plate wear, retouching, replaced objects and spatial shifts.
4. Inspect 1766, 1767 and 1768 directly to determine whether the target design survives the Gatterer–Seyfart transition.
5. Resolve the **1755/1756 numbering anomaly** from title pages rather than normalising catalogue claims.
6. Resolve the Weigel authority problem before normalising agent IDs: correspondence explicitly warns of name confusion among Johann Christoph/Christoph Weigel family members.
7. Track the publishing-business succession from the Weigel household into Martin and Johann David Tyroff as a relationship graph, rather than flattening all imprints to one publisher name.
8. Run a parallel Köhler numismatic witness table and compare its serial evidentiary practices to the calendar.
9. Track detached, cut, rebound and annotated material as evidence of consultation and recombination.
10. Add review/advertising evidence (including *neu vermehrt und verbessert*) as dated source records linked to specific issues where possible.

## Inclusion rule

The corpus is intentionally broader than “frontispieces depicting Clio,” but narrower than “all eighteenth-century Nuremberg engraving.” A record belongs when it can help reconstruct at least one of the following:

- a plate's material/serial history;
- a publishing or engraving relationship relevant to the plate network;
- a comparable visual procedure for organising evidence;
- the circulation, consultation, or re-use conditions of relevant printed apparatus.

## Privacy and provenance

Raw Gmail messages, addresses, and unpublished attachments are **not** mirrored into this public repository. Correspondence-derived facts are stored only as sanitised source notes with institution, date, claim type, and verification status. Original messages remain in the private mailbox as provenance.