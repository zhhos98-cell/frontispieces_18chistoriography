# Köhler–Heumann–Gatterer collection provenance correction — 26 August 2026

## Status

The previously used shorthand `Köhler Nachlass → Gatterer-Apparat` is too linear. Current evidence supports a **multi-source provenance model**. Köhler's collection remains a real material predecessor, but Johann Heumann von Teutschenbrunn must be represented as a second, direct contributor, and the mature apparatus also contains later institutional and personal acquisitions.

The safe model is:

`Heumann Urkunden-/Wappensammlung`
+
`Köhler Urkunden-/Wappensammlung and other auxiliary-science holdings`
+
`Gatterer's own Nürnberg/Göttingen acquisitions`
+
`later gifts, purchases, loans, and gifts addressed to the Königliches historisches Institut`
→
`Gatterer's mature teaching apparatus`.

This correction matters because the corpus is explicitly provenance-first: a later object aggregation must not be retrospectively normalized into a single inherited collection.

---

## I. Gierl 2013 explicitly gives two donors, not one linear chain

Martin Gierl's 2013 Gatterer-Medaille address states that Gatterer became a historian in the Nürnberg/Altdorf environment particularly around Johann David Köhler and Johann Heumann von Teutschenbrunn. The crucial sentence says that **Köhler and Heumann supported Gatterer and left/gave him their `Urkunden- und Wappensammlungen`.**

Direct page-image control: DAGV-News Jahresband 2013, p. 98.

This is a two-source transfer statement:

`Köhler collection → Gatterer`

and

`Heumann collection → Gatterer`.

It does **not** say:

`Heumann collection → Köhler → Gatterer`.

This distinction is now the preferred modern scholarly control unless an earlier primary transfer document establishes a more specific path.

---

## II. Chronology makes a simple Heumann → Köhler → Gatterer chain doubtful

Johann David Köhler taught at Altdorf from 1711 and moved to Göttingen in **1735**.

Johann Heumann returned to Altdorf after Vienna and began his professorial career there in **1740**; he became ordinary professor in **1744**. Gatterer studied in the Altdorf/Nürnberg environment in the later 1740s and early 1750s.

Therefore a statement that Heumann first built the relevant Altdorf teaching collection and that this same collection then passed through Köhler before reaching Gatterer would require a specific transfer mechanism not presently documented. Köhler had already left Altdorf before Heumann's professorial collection-building period.

This chronology does not make every Heumann–Köhler object transfer impossible, but it rules out treating a linear Heumann → Köhler → Gatterer chain as the default reconstruction.

---

## III. Speyer/Debus preserves a Köhler-nucleus tradition, but it should be decomposed

The Landesarchiv Speyer / Debus tradition describes Gatterer's teaching apparatus as beginning from the `Nachlass` of his Göttingen predecessor Johann David Köhler, reportedly containing material relating to:

- numismatics;
- diplomatics;
- heraldry;
- geography.

This evidence remains important. It supports a genuine Köhler → Gatterer material edge.

However, later summaries that immediately add that `auch diese Sammlung` was older and originally associated with Heumann can easily be read as a single-line provenance. In light of Gierl's explicit two-donor wording and the chronology above, that compression should not be reproduced without direct inspection of Goetting 1969 and Debus 1998.

Current evidence status:

- `Köhler holdings → Gatterer`: **strong secondary / collection-history control**;
- `Heumann holdings → Gatterer`: **strong modern scholarly control, directly page-checked**;
- `Heumann holdings → Köhler → Gatterer`: **unresolved and presently disfavoured as a default model**.

---

## IV. Pütter 1765 shows Gatterer treating the Cabinet as his working collection, while institutional loans remain distinct

Pütter's 1765 description of Göttingen teaching refers to Gatterer's `sein ... ziemlich vollständiges diplomatisches Cabinett` and describes a heterogeneous apparatus containing:

- seals;
- monograms;
- chancery marks;
- chrismons;
- alphabets and scripts;
- writing implements;
- original charters;
- engraved and drawn charters/surrogates.

Pütter then separately records around twenty particularly useful and old original charters entrusted to Gatterer for lectures from the royal-electoral archive.

This is analytically important. Already in 1765 the apparatus is not one undifferentiated ownership block. It contains at least:

`Gatterer's working cabinet`
+
`externally entrusted originals`.

The language `sein` is functional/possessive in the teaching description; it should not be treated as a legal title for every object in the cabinet.

---

## V. Liebenau 1877 proves later institutional acquisition and mixed ownership

Theodor von Liebenau's 1877 account of `Gatterer's Lehrapparat in Luzern` explicitly warns that the collection had **not originally been Gatterer's unrestricted property in its entirety**.

He gives concrete institutional acquisition examples. In 1788 Johann Ludwig Aretin sent documents and seals to Gatterer **for the Königliches historisches Institut**; other correspondents likewise sent historical documents in the context of affiliation with the institute.

This yields another provenance layer:

`institutional gifts addressed to the Historisches Institut`
→ `physically incorporated into the apparatus used/kept by Gatterer`.

Therefore the later inheritance of the whole apparatus by Gatterer's son should not be projected backward as proof that all constituent objects were originally Gatterer's private property.

This source strongly supports the repository rule:

> **collection history ≠ legal ownership history ≠ object provenance.**

---

## VI. The Göttingen `Diplomatischer Apparat` and the surviving `Gatterer-Apparat` are also not one uninterrupted collection

Modern Göttingen institutional history states that Gatterer brought/used his own `Diplomatisches Cabinet`, but that the present Göttingen Diplomatic Apparatus ultimately rests on the later collection assembled by Carl Traugott Gottlob Schönemann after conflict over access/ownership.

Meanwhile Gatterer's own cabinet passed to his son and eventually, through later transfers, into the collection now associated with the Landesarchiv Speyer.

Thus two institutional/material histories must be separated:

### A. Gatterer's personal/institute-associated apparatus

`Heumann + Köhler + Gatterer acquisitions + institute gifts/loans`
→ `Gatterer teaching cabinet`
→ `son / later private and institutional transfers`
→ `Speyer corpus`.

### B. Present Göttingen Diplomatischer Apparat

`later Schönemann teaching apparatus`
→ `institutional continuity at Göttingen`.

Calling the present Göttingen collection simply `Gatterer's collection` would therefore be incorrect.

---

## VII. Revised relation vocabulary for the corpus

Do not encode one relation named `Köhler collection inherited by Gatterer` as if it explained the whole apparatus.

Prefer separate edges:

1. `Heumann collection_material → Gatterer` — `transfer/support`, strong secondary;
2. `Köhler collection_material → Gatterer` — `transfer/inheritance`, strong collection-history secondary;
3. `Gatterer self-acquisition → teaching_cabinet` — purchases / collecting / production, mixed evidence;
4. `royal archive originals → Gatterer lectures` — `loan/entrustment`, primary via Pütter;
5. `Historisches Institut gifts → Gatterer apparatus` — `institutional donation`, primary/near-primary via Liebenau's preserved examples;
6. `Gatterer apparatus → Christoph Wilhelm Gatterer` — inheritance/controversial possession;
7. `Schönemann apparatus → present Göttingen Diplomatischer Apparat` — separate institutional lineage.

This vocabulary is more useful than a single `Nachlass` node because it preserves the heterogeneous legal and material statuses of objects.

---

## VIII. Consequence for the Köhler–Gatterer succession thesis

The broader mid-century succession thesis remains strong, but its collection component changes form.

Still secure:

- Köhler's Göttingen professorial environment → Gatterer;
- Köhler's unfinished numismatic serial → collaborative posthumous closure including Gatterer;
- Weigel/Tyroff/Bieling publication and plate ecology → Gatterer's 1759 handbook;
- Köhler collection material → one component of Gatterer's apparatus.

Corrected:

`Köhler collection = foundational whole of Gatterer-Apparat`

becomes

`Köhler material = one major inherited component within a multi-source apparatus, alongside Heumann material and later acquisitions`.

The article-level implication is stronger, not weaker: scholarly succession is **braided across carriers** rather than a single master-to-pupil transfer.

---

## IX. Remaining bounded control

High-value remaining check:

- obtain/read Hans Goetting, `Geschichte des Diplomatischen Apparats der Universität Göttingen`, *Archivalische Zeitschrift* 65 (1969), pp. 11–46, especially the opening history of Gatterer's cabinet;
- obtain/read Karl Heinz Debus, *Der Gatterer-Apparat* (Patrimonia 119, 1998), and identify exactly which assertion is Debus's and which derives from Goetting or older collection tradition.

These are worth controlling because they may identify individual acquisition episodes, but they are no longer required to prevent the corpus from making the linear-provenance error.

---

## Sources controlled in this pass

- Martin Gierl, Dankesrede zur Verleihung der Johann Christoph Gatterer-Medaille, *DAGV-News* 04/2013, p. 98: direct page-image inspection; explicit plural/two-donor statement for Köhler and Heumann's `Urkunden- und Wappensammlungen`.
- Deutsche Biographie, Johann Heumann von Teutschenbrunn: professorial chronology, extraordinary professor 1740, ordinary professor 1744.
- LMU / biographical control for Johann David Köhler: moved from Altdorf to Göttingen in 1735.
- Johann Stephan Pütter, *Versuch einer academischen Gelehrtengeschichte ...* (1765), as preserved in collection-history quotation: Gatterer's cabinet plus separately entrusted royal-electoral archival originals.
- Theodor von Liebenau, `Gatterer's Lehrapparat in Luzern` (1877): mixed ownership and gifts to the Königliches historisches Institut.
- Göttingen institutional history of the Diplomatischer Apparat: distinction between Gatterer's cabinet and the later Schönemann-based institutional collection.
