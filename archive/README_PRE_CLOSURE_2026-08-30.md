# Frontispieces and Eighteenth-Century Historiography

A provenance-first corpus for reconstructing engraved frontispieces, plate reuse, copy variation, and the visual/material infrastructures through which genealogy, heraldry, numismatics and historical evidence were organised from the late seventeenth to the later eighteenth century.

## Research problem

The seed programme is the recurring engraved threshold inscription:

> *Historia. Genealogia. Heraldica. Testes temporum et veritatis.*

It appears in the Weigel/Köhler *Geschichts-, Geschlechts- und Wappen-Calender* and survives across later Gatterer/Raspe formats. Direct image comparison now shows that the phrase does **not** identify one stable picture or one copperplate. At least three distinct composition families carry the same programme, and older designs can return after newer ones have circulated.

The project therefore keeps four levels separate:

`inscription/programme identity ≠ composition/design identity ≠ matrix/plate identity ≠ impression/copy identity`.

This turns the frontispiece from a single iconographic object into a **serial threshold apparatus and plate-stock ecology** whose verbal, graphic, material, bibliographic and evidentiary lives can diverge. A design can be replaced; an earlier design can recur; a matrix can move between publisher stocks; an impression can be detached, rebound or inserted into a later host; a copy can be enlarged by its owner.

The larger question is operational:

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

A bibliographic lead is not promoted to a plate witness until the image/front matter has been inspected. A motto match is not enough for composition identity; composition similarity is not enough for `same_plate_as`. Dimensions, lettering, signatures, frame, linework, stable defects, wear, scratches, retouching and copy chronology matter.

Evidence statuses:

- `verified_primary` — object, scan or reliable primary transcription inspected;
- `verified_catalogue` — institutional/catalogue evidence, image not yet directly inspected;
- `reported_correspondence` — archive/library correspondence;
- `research_inference` — explicit analytical hypothesis;
- `unresolved` — identity/date/state/relationship still open.

See [`docs/EVIDENCE_POLICY.md`](docs/EVIDENCE_POLICY.md).

## 1. Historia–Genealogia–Heraldica: composition families and recurrence

The controlled sequence is now recurrent rather than linear:

`1726 A → 1728 A → 1733 A → 1737 A → 1738 A → 1744 B → 1746 B → 1748 C → 1751 C → 1755 C → 1759 A → 1761 C → 1762 C? → 1763 C → 1765 A`.

### Type A — tree composition

Winged Historia stands at upper left beneath/against a tree; Time/Chronos sits centrally with scythe; putti and heraldic/genealogical media occupy the lower/right field. Direct or copy-level controls now exist for **1726, 1728, 1733, 1737, 1738, 1759 and 1765**.

The 1759 and 1765 returns are crucial. Type A does not simply disappear when later designs appear; it can be re-hosted after Type B and Type C. Whether these late impressions derive from the same physical copper as the early Type A sequence remains an open matrix-level question.

### Type B — Müller–Tyroff architectural composition

A different architectural/interior design is directly visible in **1744 and 1746**. The 1744 ULB Düsseldorf witness visibly reads `G. Müller del.` / `M. Tyroff sc.`. British Museum object `1910,0906.2` independently catalogues a 1740 *Historia Genealogia Heraldica* frontispiece as Martin Tyroff after Gabriel Müller, about 198 × 115 mm; a 1739 catalogue also reads the Müller/Tyroff signatures. Those earlier records are strong Type B hypotheses, but direct image comparison remains necessary before same-design or same-matrix promotion.

Since 1746 is directly Type B and 1748 is directly Type C, **1747 is now the single-year test** for the B→C change.

### Type C — seated Historia / open-book composition

A third design, with seated winged Historia and a large open book, is directly visible in **1748, 1751, 1755, 1761 and 1763**; 1762 is the leading probable assignment. The National Library of Finland independently records the 1762 frontispiece signature as `M. Turoff fec. 1755`.

Because Type C already exists by 1748 and a photographed physical 1755 calendar directly carries Type C, `fec. 1755` is now a **within-Type-C matrix/state problem**, not evidence for invention of the composition in 1755 and not evidence for continuity of Type B.

### Adoption boundary

- **1724** — a surviving copy is described with a different annual-memory frontispiece, *Gedenckwürdigkeiten des 1722ten Jahres*.
- **1725** — historical catalogue evidence establishes `Mit Titelkupfer`; BSB/MDZ `bsb10428127` survives, but the title copper remains unclassified.
- **1726** — a photographed physical copy directly shows Type A.

The programme-adoption boundary is therefore still **1725/1726**.

See [`docs/HISTORIA_GENEALOGIA_HERALDICA_COMPOSITION_FAMILIES_1726_1765_2026-08-26.md`](docs/HISTORIA_GENEALOGIA_HERALDICA_COMPOSITION_FAMILIES_1726_1765_2026-08-26.md), `data/frontispiece_composition_control_1726_1765_2026-08-26.jsonl`, and `data/wappenkalender_witness_census.csv`.

## 2. Prehistory: genealogy-heraldry calendars already existed

The Weigel series did not invent genealogy/heraldry visual apparatus.

- **1717–1719?** — Ostertag *Genealogisch-Heraldischer Calender* ecology.
- **1718** — a surviving copy is described with a Johann Matthias Steidlin frontispiece, twelve monthly engravings, thirty-five armorial plates and a folding genealogical table.
- **1720–1726** — Steidlin *Genealogisch-heraldischer Staats-Calender* continues as an annual series; the 1720 Heidelberg digitisation separately indexes its frontispiece and includes `Bericht an den Buchbinder` instructions.
- Steidlin volumes survive for **1723 and 1726**, so Augsburg/Steidlin and Nürnberg/Weigel overlap during the threshold transition.

The 1723–26 problem is therefore one of **competition and reframing inside an existing calendar technology**, not simple genre invention.

See `data/predecessor_calendar_census.csv` and [`docs/PREHISTORY_COMPETITION_SWEEP_2026-08-21.md`](docs/PREHISTORY_COMPETITION_SWEEP_2026-08-21.md).

## 3. Contemporary standards: graphic quality is not evidentiary reliability

Two contemporary controls make the period's own evaluative vocabulary visible.

**Martin Schmeitzel, 1723.** In *Einleitung zur Wappen-Lehre* he praises the c.1720 Augsburg genealogical-heraldic calendar's coats of arms as cleanly engraved while dismissing the accompanying explanations. The substantive wording is controlled; direct p.69 inspection remains useful for diplomatic quotation.

**Johann Ehrenfried Zschackwitz, 1724.** The HAB full-text transcription of *Historisch-Genealogischer Schau-Platz* programmatically promises genealogies purged of fables and supported by necessary `Documenta`. Zschackwitz evaluates genealogical authors through accuracy, errors, certainty, trustworthiness and comparison; he criticises Hübner's tables for conspicuous mistakes despite their claimed worldwide correspondence and argues for including only genealogical origins about which one can speak with certainty. He also prints submitted corrections to Hübner's tables.

This is a strong contemporary control for the threshold transition: **visual execution, textual explanation, documentary support, comparison and certainty were already separable criteria of genealogical quality.**

See `data/contemporary_reception_records.jsonl`.

## 4. Evidence-language prehistory: witnesses, truth and comparison

The corpus records lexical and operational precedents without converting them into an unproven influence chain.

- **Cicero, *De oratore* II.36** — singular *Historia* as `testis temporum, lux veritatis`.
- **Gisbert Cuper, 30 Oct. 1691** — coins described as `certissimi testes temporum, clarissima lux veritatis` while arranging royal history from numismatic evidence.
- **Christian Schlegel, c.1696–97** — manuscript project titled *Historiae Saxonicae Antiquioris Veritas ex Nummis Demonstrata*.
- **Johann Georg Eccard, 1721–22** — scripts, seal impressions, coins, securely dated manuscripts and archives compared across media; when originals cannot travel, drawings and ectypes in isinglass, tin foil, wax, gypsum, lead or paper are accepted. Coins can `imo et firmare` genealogy.
- **Johann David Köhler, 1749** — *Nutz der Wappenkenntnüß zur Entdeckung einer historischen Wahrheit*: a material object, engraved representation, coats of arms and initials are used to resolve a historical identification; a 1751 response reopens the conclusion.

The current analytical category is **rhetorical-operational convergence / redistribution of evidentiary authority**. The corpus does not yet claim a Cicero → Cuper → Schlegel → Eccard → Köhler textual genealogy.

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
- `owner_augmented_visual_comparison_set`;
- `annotated_copy`;
- plate/text separation and later plate reuse.

Two copy-level controls now show owners actively enlarging the published apparatus. A 1747 copy described in 1912 had **more than one hundred additional named aristocratic copper engravings** cut out and lightly attached to existing plate versos. A 1750 luxury copy associated by armorial supralibros with **Maria Josepha of Saxony, Dauphine of France** had its 108 issued armorial engravings coloured and heightened with gold and silver, while numerous additional coloured arms were pasted onto blank pages.

A copy is therefore not merely an imperfect representative of an edition. Damage, extraction, rebinding, colouring, metallic heightening, insertion and annotation can reveal how these visual systems were handled and recomposed. In some cases the calendar became an **extensible private armorial database**.

See `data/copy_afterlife_controls_2026-08-26.jsonl` and [`docs/COPY_AUGMENTATION_AS_PRIVATE_ARMORIAL_DATABASE_1747_1750_2026-08-26.md`](docs/COPY_AUGMENTATION_AS_PRIVATE_ARMORIAL_DATABASE_1747_1750_2026-08-26.md).

## Repository layout

```text
README.md
schema/
  record.schema.json
data/
  core_records.jsonl
  web_witness_records.jsonl
  wappenkalender_witness_census.csv
  frontispiece_composition_control_1726_1765_2026-08-26.jsonl
  copy_afterlife_controls_2026-08-26.jsonl
  predecessor_calendar_census.csv
  handbook_copy_records.jsonl
  parallel_apparatus_census.csv
  production_network_records.jsonl
  transmission_network_records.jsonl
  evidentiary_language_records.jsonl
  contemporary_reception_records.jsonl
  research_leads.csv
docs/
  EVIDENCE_POLICY.md
  HISTORIA_GENEALOGIA_HERALDICA_COMPOSITION_FAMILIES_1726_1765_2026-08-26.md
  CLIO_PLATE_STATE_CONTROL_1739_1762_2026-08-26.md
  COPY_AUGMENTATION_AS_PRIVATE_ARMORIAL_DATABASE_1747_1750_2026-08-26.md
  PREHISTORY_COMPETITION_SWEEP_2026-08-21.md
  EVIDENCE_AND_TRUTH_SWEEP_2026-08-21.md
  MATERIAL_SURROGATE_AND_NUREMBERG_1725_SWEEP_2026-08-21.md
```

## Immediate high-information queue

1. **1725:** extract/classify the documented title copper from BSB/MDZ `bsb10428127`; this decides whether the recurring programme begins in 1725 or 1726.
2. **1739/1740:** directly classify the Müller/Tyroff witnesses and compare them with 1744 Type B before any same-matrix claim.
3. **1747:** inspect the Rostock/Bassenge opening image; with 1746 Type B and 1748 Type C, this single year now locates the B→C replacement.
4. **1752:** inspect BSB `bsb10428150`; test Type C persistence and the historical Gandersheim catalogue entry `Historia Genealogia Heraldica de An. 1751 et 1752`.
5. **Type C matrix sequence:** compare 1748 → 1751 → 1755 → 1761 → 1762 → 1763, especially the relation of the 1755 copy to Finna's `M. Turoff fec. 1755` reading.
6. **Type A recurrence:** compare 1726–1738 against 1759 and 1765 for signatures, dimensions, stable defects and wear; a positive same-matrix result would directly document long-lived threshold plate stock across host/publisher regimes.
7. **1767–1776:** identify the three repeated Seyfart/Raspe frontispieces by composition family before asking whether any matrix persists.
8. Compare the 1725 calendar and undated handbook **85-plate** configurations plate by plate before claiming shared stock.
9. Inspect Eccard 1725 plates directly and reconstruct Tab. I–III plus text copper.
10. Keep every documented transmission edge separate from operational similarity until direct citation, correspondence, matrix or production evidence is found.

## Privacy and provenance

Raw Gmail messages, addresses and unpublished attachments are **not** mirrored into this public repository. Correspondence-derived facts are stored only as sanitised source notes with institution, date, claim type and verification status. Original messages remain in the private mailbox as provenance.
