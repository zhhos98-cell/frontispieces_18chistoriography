# Winckelmann 1664 / Staden 1557 pairwise concordance — batch 1: pp.142, 168, 179

Date: 2026-08-28  
Status: PRIORITY-1 PARTIAL ADVANCE — COMPOSITION, LETTERING, DIMENSION, AND COPY-ROUTE CONTROLS IMPROVED; **NO NEW SAME-MATRIX PROMOTION** WITHOUT DIRECT 1664 RASTER/DEFECT COMPARISON.

Companion data:

`data/winckelmann_1664_staden_pairwise_matrix_control_batch1_2026-08-28.csv`

## Result

The first pairwise pass sharpens three diagnostic cases without relaxing the repository guardrail:

`composition identity`
≠ `catalogue same-block attribution`
≠ `physical matrix identity`
≠ `matrix state`
≠ `individual impression state`.

The immediate gain is asymmetric but useful. For p.142 the 1664 side now has an item-level JCB record with exact image dimensions and an explicit original-woodcut attribution. For pp.168 and 179 the 1557 labelled states can now be specified more concretely, while the JCB/IA bibliographic note controls reported name elimination in 1664. None of these facts independently establishes same physical matrix identity.

---

## 1. p.142 — fishing with bows/arrows

JCB Archive of Early American Images record `01512-5`, call number `J664 W761a oblong`, identifies Winckelmann p.142 as a woodcut measuring **10.5 × 10.8 cm**. Its description matches the distinctive Staden fishing composition: Indigenous men fishing with bows/arrows and with their hands. The item-level note says the illustrations were reprinted from the original woodcuts used in Staden's Marburg 1557 edition.

Source:

- JCB AEAI record `01512-5`: https://jcb.lunaimaging.com/luna/servlet/detail/JCB~1~1~4830~7600003

The 1557 motif is independently present in the Brasiliana/BBM Staden corpus as the fishing-with-bow-and-arrow image.

Current status:

`COMPOSITION MATCH = STRONG / DISTINCTIVE`

`1664 IMAGE DIMENSIONS = ITEM-LEVEL CONTROLLED`

`SAME PHYSICAL MATRIX = CATALOGUE ATTRIBUTION ONLY / NOT DIRECTLY VERIFIED`

This is therefore a good positive-control pair, but not yet a matrix proof. The next useful operation is normalized border/linework comparison, especially stable nicks, line endings, frame breaks and small defects that a composition-copy hypothesis would not normally reproduce exactly.

---

## 2. p.168 — Ubatuba attack composition in a different narrative context

The 1557 source occurrence is now securely identified at composition level as the attack on the village of Ubatuba, Staden Part I, chapter 29. Brasiliana Iconográfica catalogues the 1557 woodcut as:

`Ataque dos Tupiniquins à aldeia de Ubatuba`

ID `45000008047.77`.

Source:

- Brasiliana Iconográfica: https://www.brasilianaiconografica.art.br/obras/23530/ataque-dos-tupiniquins-a-aldeia-de-ubatuba

The 1557 image itself visibly carries the place-name label **`uwatibi`** in the upper image field. The spelling should be treated as an image transcription, not silently normalized to modern `Ubatuba`.

The JCB/Internet Archive/Open Library edition note reports that on Winckelmann p.168 names present on the original woodcut were eliminated.

Edition-level control:

- Open Library / JCB-derived record: https://openlibrary.org/books/OL33153163M/Der_americanischen_Neuen_Welt_Beschreibung
- Wikimedia Commons scan record, JCB source copy: https://commons.wikimedia.org/wiki/File:Der_americanischen_Neuen_Welt_Beschreibung,_-_darinnen_deren_Erfindung,_Lager,_Natur,_Eigenschaft,_Sitten,_Barbarey,_und_unerh%C3%B6rte_Grausamkeit_der_Einwohner,_Thier,_V%C3%B6gel_(IA_deramericanische00winc).pdf

This strengthens the state question but does not close it:

`1557 LABEL PRESENT = DIRECT IMAGE CONTROL`

`1664 NAME ELIMINATION = CATALOGUE CONTROL`

`SAME PHYSICAL MATRIX = UNVERIFIED`

`REMOVAL MECHANISM = OPEN`.

The contextual discrepancy remains especially important. The inherited Ubatuba captivity-scene composition is inserted in Winckelmann within the earlier first-voyage Garasu/Igarassu sequence. Thus even if physical matrix identity is eventually proved, the object will simultaneously control:

`MATRIX AUTHENTICITY`
+
`CONTEXTUAL RECOMPOSITION`.

---

## 3. p.179 — shipwreck near Itanhaém / São Vicente

The 1557 source occurrence is the shipwreck scene associated with the São Vicente/Itanhaém episode. The 1557 image visibly contains multiple geographical labels. Two can be safely read from the currently recovered image as **`S. vin`** and **`S. maro`**; an additional upper-left place-name is present but should be transcribed from the best source scan rather than normalized from secondary captions.

Useful source controls:

- Brasiliana Iconográfica Staden corpus, where `Naufrágio nas proximidades da povoação de Itanhaém` is catalogued among the 1557 images: https://www.brasilianaiconografica.art.br/obras/%40relId/23469
- Wikimedia Commons reproduction `Stadens Schiffbruch bei Itanhaém.jpg`, sourced there to Franz Obermeier's 2005 study.

The JCB/IA/Open Library edition note reports the second name-elimination anomaly on Winckelmann p.179.

Current status:

`SAME EPISODE / COMPOSITION = STRONG`

`MULTIPLE 1557 PLACE LABELS = DIRECT IMAGE CONTROL`

`1664 NAME ELIMINATION = CATALOGUE CONTROL`

`SAME PHYSICAL MATRIX = UNVERIFIED`

`PHYSICAL STATE MECHANISM = OPEN`.

This should become the strongest state test once a direct p.179 raster is recovered, because several lettered zones can be compared simultaneously against the surrounding linework. The correct test order remains:

1. establish matrix identity from non-letter diagnostic geometry/defects;
2. inventory exactly which letterforms disappear;
3. inspect whether the affected zones show cutting, plugging, damage, weak inking, masking or another mechanism;
4. compare a second 1664 copy before treating the difference as a stable matrix state.

---

## 4. Independent 1664-copy routes now identified

The JCB/Internet Archive copy is not the only assistant-side route. Two further institutional discovery paths are now on record:

### Göttingen

GDZ exposes a 1664 digitization under:

`PPN829199152`

Landing record:

https://gdz.sub.uni-goettingen.de/id/PPN829199152

This is especially valuable because a second-copy comparison can distinguish a stable altered matrix/state from a copy/impression anomaly.

### Münster

ZVDD indexes a 1664 ULB Münster digital witness within the Jodocus Hermann Nünning Barockbibliothek. The already recovered URN route is:

`urn:nbn:de:hbz:6:1-15914`.

These routes remain **assistant-side retrieval tasks**. Nothing is escalated to `docs/USER_ACTION_LOG.md` at this stage.

---

## 5. Methodological consequence

This batch makes the matrix guardrail more operational. The p.168 and p.179 anomalies are tempting because the later image reportedly loses names, but the inference must run in the opposite order from the bibliographic tradition:

`same composition + altered lettering`

is **not** enough for:

`same physical matrix + altered matrix state`.

Direct non-letter diagnostics must establish or strongly constrain matrix identity first. Only then can disappearance of lettered relief be interpreted materially.

The next pass should therefore prioritize direct raster recovery for pp.168 and 179 from the GDZ/JCB/Münster routes, followed by p.142 as a positive-control overlay. After those three are exhausted, expand the same protocol to pp.140, 143, 144, 155, 157 and 158 rather than bulk-promoting the remaining corpus.
