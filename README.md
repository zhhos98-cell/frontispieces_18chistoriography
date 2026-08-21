# Frontispieces and Eighteenth-Century Historiography

A provenance-first corpus for reconstructing engraved frontispieces, plate reuse, copy variation, and the visual/material infrastructures through which genealogy, heraldry, numismatics and historical evidence were organised from the late seventeenth to the later eighteenth century.

## Research problem

The seed object is the recurring engraved frontispiece:

> *Historia. Genealogia. Heraldica. Testes temporum et veritatis.*

It appears in the Weigel/Köhler *Geschichts-, Geschlechts- und Wappen-Calender* and survives across later Gatterer formats. British Museum object `1910,0906.2` independently catalogues the 1740 frontispiece as **Martin Tyroff after Gabriel Müller**, approximately 198 × 115 mm.

The project no longer treats this as a single iconographic image. It treats the frontispiece as a **serial artefact and threshold apparatus** whose material, bibliographic and evidentiary lives can diverge: it can be reissued, detached, rebound, copied, re-engraved, moved into a new publication rhythm, or survive after the text and editorial regime around it have changed.

The larger question is therefore operational:

> How did engraved images, coats of arms, genealogical tables, coins, seals, manuscripts, cabinet objects and their reproductions become transportable and comparable historical witnesses, and how were those witnesses reorganised across annual calendars, weekly serials, handbooks and cumulative armorials?

## Corpus unit and evidence discipline

The preferred atomic unit is a **witness occurrence**: one verifiable appearance of a plate or closely related plate-state in one publication context and, where possible, one identified copy.

The corpus keeps distinct:

1. `plate_series` — design/plate lineage;
2. `witness` — one publication occurrence;
3. `copy` — one surviving institutional, digitised or market copy;
4. `agent` — designer, engraver, publisher, editor, scholar, owner, dealer;
5. `feature` — inscription, object, attribute, arrangement, placement, dimensions;
6. `source_evidence` — object record, scan, catalogue, correspondence, review, advertisement;
7. `relationship` — reuse, same-plate-as, variant-of, derived-from, production association, textual use, teaching, publisher succession.

A bibliographic lead is not promoted to a plate witness until the image/front matter has been inspected. Similar iconography is not enough for `same_plate_as`; dimensions, lettering, line breaks, signatures, wear, scratches, retouching and copy chronology matter.

Evidence statuses:

- `verified_primary` — object, scan or reliable primary transcription inspected;
- `verified_catalogue` — institutional/catalogue evidence, image not yet directly inspected;
- `reported_correspondence` — archive/library correspondence;
- `research_inference` — explicit analytical hypothesis;
- `unresolved` — identity/date/state/relationship still open.

See [`docs/EVIDENCE_POLICY.md`](docs/EVIDENCE_POLICY.md).

## 1. The Clio plate: current chronology

The target allegory should **not** be projected backward across the whole Weigel calendar run.

- **1724** — a surviving copy is described with a different annual-memory frontispiece, *Gedenckwürdigkeiten des 1722ten Jahres*.
- **1725** — independent historical catalogue evidence establishes `Mit Titelkupfer`; BSB/MDZ `bsb10428127` and a free 308-page Google digitisation survive, but the title copper's identity remains unresolved.
- **1726** — surviving auction imagery visibly shows the target *Historia Genealogia Heraldica* allegory.
- **ca.1737** — a detached target frontispiece survives independently, about 198 × 122 mm, with reported traces of former binding.
- **1740** — British Museum `1910,0906.2`: target design explicitly catalogued as Martin Tyroff after Gabriel Müller.
- **1744** — complete-copy description explicitly names the target frontispiece.
- **1759** — Gatterer *Handbuch* copy explicitly transcribes `HISTORIA GENEALOGIA HERALDICA / TESTES TEMPORVM ET VERITATIS`.
- **1764** — *Fortgesetzter Wappen-Calender* again explicitly names the target.
- **1765** — title copper/frontispiece independently reported; identity not yet checked.
- **1767–1776** — Seyfart/Raspe four-volume *Wappenbuch* set is described with **three repeated engraved frontispieces**; a separate 1771 volume has a `Titelkupfer`. The repeated design has not yet been identified as Clio.

The highest-information unresolved object remains **1725**: if its title copper is Clio, the regime change occurs in 1725; if not, it occurs between 1725 and 1726.

## 2. Prehistory: genealogy-heraldry calendars already existed

The Weigel series did not invent genealogy/heraldry visual apparatus.

- **1717–1719?** — Ostertag *Genealogisch-Heraldischer Calender* ecology.
- **1718** — a surviving copy is described with a Johann Matthias Steidlin frontispiece, twelve monthly engravings, thirty-five armorial plates and a folding genealogical table.
- **1720–1726** — Steidlin *Genealogisch-heraldischer Staats-Calender* continues as an annual series; the 1720 Heidelberg digitisation separately indexes its frontispiece and includes `Bericht an den Buchbinder` instructions.
- Steidlin volumes survive for **1723 and 1726**, so Augsburg/Steidlin and Nürnberg/Weigel overlap during the Clio transition.

The 1723–26 problem is therefore one of **competition and reframing inside an existing calendar technology**, not simple genre invention.

See `data/predecessor_calendar_census.csv` and [`docs/PREHISTORY_COMPETITION_SWEEP_2026-08-21.md`](docs/PREHISTORY_COMPETITION_SWEEP_2026-08-21.md).

## 3. Contemporary standards: graphic quality is not evidentiary reliability

Two contemporary controls make the period's own evaluative vocabulary visible.

**Martin Schmeitzel, 1723.** In *Einleitung zur Wappen-Lehre* he praises the c.1720 Augsburg genealogical-heraldic calendar's coats of arms as cleanly engraved while dismissing the accompanying explanations. The current record remains below `verified_primary` until p.69 is checked directly in the scan.

**Johann Ehrenfried Zschackwitz, 1724.** The HAB full-text transcription of *Historisch-Genealogischer Schau-Platz* programmatically promises genealogies purged of fables and supported by necessary `Documenta`. Zschackwitz evaluates genealogical authors through accuracy, errors, certainty, trustworthiness and comparison; he criticises Hübner's tables for conspicuous mistakes despite their claimed worldwide correspondence and argues for including only genealogical origins about which one can speak with certainty. He also prints submitted corrections to Hübner's tables.

This is a strong contemporary control for the Clio transition: **visual execution, textual explanation, documentary support, comparison and certainty were already separable criteria of genealogical quality.**

See `data/contemporary_reception_records.jsonl`.

## 4. Evidence-language prehistory: witnesses, truth and comparison

The corpus records lexical and operational precedents without converting them into an unproven influence chain.

- **Cicero, *De oratore* II.36** — singular *Historia* as `testis temporum, lux veritatis`.
- **Gisbert Cuper, 30 Oct. 1691** — coins described as `certissimi testes temporum, clarissima lux veritatis` while arranging royal history from numismatic evidence.
- **Christian Schlegel, c.1696–97** — manuscript project titled *Historiae Saxonicae Antiquioris Veritas ex Nummis Demonstrata*.
- **Johann Georg Eccard, 1721–22** — scripts, seal impressions, coins, securely dated manuscripts and archives compared across media; when originals cannot travel, drawings and ectypes in isinglass, tin foil, wax, gypsum, lead or paper are accepted. Coins can `imo et firmare` genealogy.
- **Johann David Köhler, 1749** — *Nutz der Wappenkenntnüß zur Entdeckung einer historischen Wahrheit*: a material object, engraved representation, coats of arms and initials are used to resolve a historical identification; a 1751 response reopens the conclusion.

The current analytical category is **rhetorical-operational convergence / redistribution of evidentiary authority**. The corpus does not yet claim a Cicero → Cuper → Schlegel → Eccard → Köhler → Clio textual genealogy.

See `data/evidentiary_language_records.jsonl` and [`docs/EVIDENCE_AND_TRUTH_SWEEP_2026-08-21.md`](docs/EVIDENCE_AND_TRUTH_SWEEP_2026-08-21.md).

## 5. Visual surrogates can transmit and corrupt evidence

A particularly important earlier control comes from the Sagittarius–Schlegel numismatic material reconstructed by Martin Mulsow.

In the 1680s Johann Christfried Sagittarius planned a work on roughly **600 bracteates**. Some images derived from originals and others from received drawings; **497 coin images** were cut in wood across four full sheets. Schlegel later criticised reproduction errors: names could be omitted and letters transposed. He nevertheless understood the sheets as a way for Sagittarius to communicate remotely what his collection contained. A Gotha witness (`Ch. A 1205`) preserves Schlegel's handwritten identifications beneath the images.

The operational sequence is therefore already visible before 1700:

`object / received drawing → printed surrogate → remote circulation → reproduction error → expert correction`

Schlegel's own c.1696–97 manuscript and its eight intended folio copperplates later acquired separate documentary lives, providing an early control for the corpus rule **plate history ≠ text history ≠ host-publication history**.

See [`docs/MATERIAL_SURROGATE_AND_NUREMBERG_1725_SWEEP_2026-08-21.md`](docs/MATERIAL_SURROGATE_AND_NUREMBERG_1725_SWEEP_2026-08-21.md).

## 6. Nürnberg 1725 as a microhistory

The transition year is becoming a dense local comparison rather than a single missing frontispiece.

### Weigel calendar

A 1930 Emil Hirsch catalogue records the **1725 Wappenkalender** with:

- `Titelkupfer`;
- twelve portraits;
- about one hundred coloured arms on **85 copperplates**;
- a colour-key copperplate.

### Weigel-widow handbook

The immediately following Hirsch lot is the undated *Genealogisches und heraldisches Hand-Buch*, catalogued `(1725)`, also with:

- `Titelkupfer`;
- **85 engraved armorial plates**.

Other surviving copies range from 60 to 106 armorial plates and include later recombination. One 2026 auction copy explicitly has its original frontispiece/title missing and a **foreign frontispiece plus calendar leaves inserted** by a later owner.

The Hirsch 85/85 coincidence is therefore a test, not a conclusion. Plate-by-plate comparison should check captions, sequence, verso Stammtafeln, dimensions, scratches/wear and colour state before any same-stock claim is made.

### Eccard / Ebner / Monath

In the same year Johann Georg Eccard published in Nürnberg with **Peter Conrad Monath** an explanation of an old jewel/casket from the Ebner cabinet. The object, depicting a dynastic betrothal, is used together with related old coins to illuminate Brunswick-Lüneburg history. Copy descriptions report **three copperplates**, one folding, plus a text copper and woodcut paratext.

A later numismatic writer, Johann Alexander Döderlein, cites Eccard's **p.45, Tab. III, Fig. XXVI** in a coin identification. This demonstrates that Eccard's plates functioned as numbered, reusable reference figures rather than decorative illustration alone.

No direct Eccard–Weigel/Köhler production relation has yet been established. Monath is a separate publisher. The significance is **same-year, same-city evidentiary practice**, not influence proof.

## 7. A 1729 Nürnberg bridge: Döderlein reads Schlegel and Eccard

Johann Alexander Döderlein's *Commentatio Historica de Numis Germaniae Mediae* (Nürnberg, 1729) places two previously separate strands inside one printed numismatic argument:

- he refers the reader to **Schlegel**;
- in the same comparison environment he says he encountered Eccard's 1725 *Kleinodien-Kästlein* and explicitly uses **Eccard p.45 / Tab. III Fig. XXVI** to judge a coin.

This is the strongest printed Nürnberg bridge yet found between the late-seventeenth-century Schlegel world and Eccard's 1725 object publication.

The same year Köhler launches *Historische Münz-Belustigung*. A direct Johann David Köhler → Döderlein citation has **not** been found in the current searchable series index (`Döderlein / Doederlein / Doderlein` all zero hits).

A genuine later social edge does exist: Johann David's son **Johann Tobias Köhler** was educated at Weißenburg under Döderlein and later contributed to/continued his father's *Münzbelustigungen*. This is an intergenerational connection, not proof of Johann David's 1729 borrowing.

See `data/parallel_apparatus_census.csv` and `data/production_network_records.jsonl`.

## 8. Overlapping publication rhythms

The current object ecology is not linear:

- annual genealogy/heraldry calendars;
- annual Weigel historical-genealogical-heraldic calendar, **1723–1757**;
- undated Weigel-widow genealogical/heraldic handbook for **newspaper reading**;
- Köhler weekly *Historische Münz-Belustigung*, **1729–1750**, 22 parts;
- Gatterer handbook, **1759–1763**;
- continued annual handbook/calendar, **1764–1766**;
- Seyfart/Raspe cumulative *Wappenbuch*, **1767–1776**.

The more useful vocabulary is **competition, extraction, recomposition, de-serialisation, re-serialisation and accumulation**. The same kinds of armorial, genealogical and material witnesses move between different rhythms of consultation.

## 9. Material afterlives are evidence

The corpus preserves rather than normalises away:

- `frontispiece_missing`;
- `detached_plate`;
- `cut_and_reused`;
- `rebound_composite`;
- `inserted_foreign_frontispiece`;
- `calendar_leaves_inserted`;
- `annotated_copy`;
- plate/text separation and later plate reuse.

A copy is therefore not merely an imperfect representative of an edition. Damage, extraction, rebinding and annotation can reveal how these visual systems were actually handled and recomposed.

## Repository layout

```text
README.md
schema/
  record.schema.json
data/
  core_records.jsonl
  web_witness_records.jsonl
  wappenkalender_witness_census.csv
  predecessor_calendar_census.csv
  handbook_copy_records.jsonl
  parallel_apparatus_census.csv
  production_network_records.jsonl
  evidentiary_language_records.jsonl
  contemporary_reception_records.jsonl
  gnm_holdings_seed.csv
  research_leads.csv
docs/
  EVIDENCE_POLICY.md
  WEB_SWEEP_2026-08-21.md
  DEEP_SWEEP_2026-08-21.md
  PREHISTORY_COMPETITION_SWEEP_2026-08-21.md
  EVIDENCE_AND_TRUTH_SWEEP_2026-08-21.md
  MATERIAL_SURROGATE_AND_NUREMBERG_1725_SWEEP_2026-08-21.md
```

## Immediate high-information queue

1. **Extract the 1725 title copper** from BSB/MDZ `bsb10428127` or another complete copy.
2. Compare the 1725 calendar and handbook **85-plate** configurations plate by plate before claiming shared stock.
3. Inspect Eccard 1725 plates directly; identify engraver/signatures and reconstruct Tab. I–III plus text copper.
4. Search Johann David Köhler's writings/correspondence for Döderlein and Eccard; keep current zero-hit searches bounded.
5. Identify the **three repeated Seyfart frontispieces** across 1767–1776 and test whether any are the Müller–Tyroff Clio design.
6. Compare 1718/1720/1723/1726 Steidlin frontispieces against the Weigel 1724–26 sequence.
7. Verify Schmeitzel 1723 p.69 directly and expand contemporary review/advertising evidence for `neu vermehrt`, `verbessert`, `Wahrheit`, `Prüfung`, `Gewißheit` and correction.
8. Resolve Weigel household/firm authority records before normalising imprints.
9. Continue Köhler's numismatic corpus issue-by-issue, recording objects, engravings, provenance, comparison language, corrections and reader correspondence.
10. Keep every documented transmission edge separate from operational similarity until direct citation, correspondence or production evidence is found.

## Privacy and provenance

Raw Gmail messages, addresses and unpublished attachments are **not** mirrored into this public repository. Correspondence-derived facts are stored only as sanitised source notes with institution, date, claim type and verification status. Original messages remain in the private mailbox as provenance.