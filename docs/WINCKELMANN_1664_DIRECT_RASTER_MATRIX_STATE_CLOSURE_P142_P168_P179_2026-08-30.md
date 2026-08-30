# Winckelmann 1664 / Staden 1557 — direct-raster matrix/state closure for pp.142, 168, 179

Date: 2026-08-30  
Status: **PRIORITY 1 CLOSED — P.168 SOURCE OCCURRENCE CORRECTED; P.168 AND P.179 SAME-MATRIX RELATIONS PROMOTED BY DIRECT WHOLE-FIELD IMAGE CONCORDANCE; LETTERING-STATE DIFFERENCES DIRECTLY OBSERVED; PHYSICAL ALTERATION MECHANISM REMAINS UNSPECIFIED.**

## Result

User-assisted direct page images from the John Carter Brown Library / Internet Archive 1664 copy have removed the raster-access blocker for printed pp.142, 168 and 179.

The most important result is a correction:

**Winckelmann p.168 is not the Staden Ubatuba attack plate previously assigned in Batch 1.** It is the 1557 Igarassu / Igaraçu battle woodcut catalogued by Brasiliana Iconográfica as:

- `[Combate entre portugueses e índios caetés em Igarassu]`
- Hans Staden, 1557
- BBM Digital / Biblioteca Brasiliana Guita e José Mindlin
- ID `45000008047.28`
- `https://www.brasilianaiconografica.art.br/obras/23502/combate-entre-portugueses-e-indios-caetes-em-igarassu`

The direct 1557 / 1664 comparison now supports:

`SAME COMPOSITION`
+
`WHOLE-FIELD NON-LETTER GEOMETRY CONCORDANCE`
+
`DENSE LOCAL LINE-JUNCTION CONCORDANCE`
+
`FRAME / TERRAIN / FIGURE / PALISADE / VESSEL CONCORDANCE`

→ **`SAME PHYSICAL MATRIX = HIGH-CONFIDENCE DIRECT-RASTER VERIFICATION`** for p.168.

The p.179 shipwreck pair gives an independent second case with the same result.

The repository-wide bulk claim that all 32 Staden-section images are same-matrix impressions remains prohibited: two direct pairwise promotions do not license a 32-fold promotion.

---

## 1. p.168 — corrected source: Igarassu / Igaraçu battle

### 1557 source occurrence

Brasiliana Iconográfica directly catalogues the 1557 woodcut `[Combate entre portugueses e índios caetés em Igarassu]`, ID `45000008047.28`.

The previously assigned Ubatuba plate (`Ataque dos Tupiniquins à aldeia de Ubatuba`) is a different composition and must be removed from the p.168 concordance.

### Direct 1664 raster

Printed p.168 in the user-supplied JCB/IA page image contains the Igarassu battle composition.

The following non-letter structures coincide after perspective/scale normalization:

- the principal branching watercourse;
- lower bridge/palisade geometry;
- lower-left settlement/hill contour;
- central fortified enclosure;
- right-side mounted/armed figure group;
- upper-right circular/enclosed battle vignette;
- upper and lateral landscape/tree structures;
- repeated small figure/weapon intersections;
- outer frame geometry.

This is not merely iconographic similarity. Dense idiosyncratic line geometry survives across the image field.

A supporting feature-registration diagnostic on cropped source/host images yielded **49 ratio-filtered ORB matches, 41 RANSAC homography inliers (83.7%)**. This statistic is not treated as proof by itself; it is a reproducibility check on the visual whole-field concordance.

### Lettering/state result

The 1557 Igarassu image contains several integral place labels. The 1664 impression preserves substantial integral lettering but does not preserve every source label. In particular, a small place-name associated with the lower-left settlement/hill is present in the 1557 source and absent in the inspected 1664 p.168 impression, while surrounding non-letter relief geometry remains concordant.

The exact historical orthography of that small source label should not be silently normalized from a low-resolution screenshot; the matrix-state conclusion does not depend on doing so.

Current classification:

- `source_occurrence = CORRECTED / DIRECT`
- `same_matrix_as_1557 = HIGH_CONFIDENCE_DIRECT_RASTER`
- `lettering_state_difference = DIRECTLY_OBSERVED`
- `alteration_mechanism = UNRESOLVED`

Do not yet specify `cut away`, `plugged`, `masked`, `selectively inked`, or another physical intervention. A second 1664 copy would discriminate stable matrix state from impression-level treatment, but it is now confirmatory rather than a blocker for the pairwise identity result.

---

## 2. p.179 — Itanhaém / São Vicente shipwreck

### 1557 source occurrence

Brasiliana Iconográfica directly catalogues:

- `[Naufrágio nas proximidades da povoação de Itanhaém]`
- Hans Staden, 1557
- ID `45000008047.47`
- `https://www.brasilianaiconografica.art.br/obras/23511/naufragio-nas-proximidades-da-povoacao-de-itanhaem`

### Direct 1664 raster

Printed p.179 in the supplied JCB/IA page image is the same shipwreck composition.

Whole-field concordance includes:

- ship hull, rigging and mast intersections;
- wave contours and repeated curl geometry;
- left shoreline and settlement contour;
- circular/lagoon-like landform and enclosed buildings;
- upper-right figures and vegetation;
- lower-left peninsula/shore geometry;
- outer frame.

A supporting registration diagnostic yielded **61 ratio-filtered ORB matches, 51 RANSAC inliers (83.6%)** across the cropped 1557/1664 pair.

The density and distribution of concordant non-letter geometry across the full block support a direct pairwise promotion:

`same_matrix_as_1557 = HIGH_CONFIDENCE_DIRECT_RASTER`.

### Lettering/state result

The 1557 source visibly contains multiple geographical labels. The inspected 1664 impression shows selective survival rather than wholesale removal of all lettering:

- the 1557 `S. vin` label inside the circular landform is absent in the 1664 impression;
- the upper-left settlement label visible in 1557 is absent in 1664;
- `S. maro` survives in the lower-left/peninsula zone;
- other small source lettering should be transcribed only from a stronger source raster before exact orthography is asserted.

This selective pattern is materially important because the surrounding coastline, buildings, waves and ship geometry remain concordant while individual lettered relief zones differ.

Current classification:

- `source_occurrence = DIRECT`
- `same_matrix_as_1557 = HIGH_CONFIDENCE_DIRECT_RASTER`
- `lettering_state_difference = DIRECTLY_OBSERVED`
- `alteration_mechanism = UNRESOLVED`

The evidence strongly supports a later state/use of the same matrix in which selected lettering no longer prints. It does **not** yet identify the mechanical cause of that difference.

---

## 3. p.142 — fishing positive control

User-assisted retrieval also supplies a direct 1664 p.142 raster.

The 1557 source occurrence is directly catalogued by Brasiliana Iconográfica as:

- `[Pescaria com arco e flecha]`
- Hans Staden, 1557
- ID `45.000.008.047.139`
- `https://www.brasilianaiconografica.art.br/obras/23570/pescaria-com-arco-e-flecha`

JCB item-level record `01512-5` independently identifies Winckelmann p.142, gives image dimensions `10.5 × 10.8 cm`, and attributes the 1664 illustrations to reprinting from Staden's original 1557 woodcuts.

Current p.142 status is upgraded from `1664 raster unavailable` to `direct 1664 raster inspected`. Its source occurrence and composition are secure and it remains a positive control. This closure does not need to over-promote p.142 from catalogue attribution alone because p.168 and p.179 now supply the decisive direct pairwise matrix tests.

---

## 4. What the direct comparison changes

The old evidence hierarchy was:

`catalogue says original blocks`
+
`composition mapping`
→ `matrix identity still open`.

For pp.168 and 179 the hierarchy is now:

`direct 1557 source raster`
+
`direct 1664 host raster`
+
`distributed non-letter linework concordance`
+
`local junction/frame/terrain/figure concordance`
→ **`same_matrix` promoted pairwise**

followed by:

`same_matrix`
+
`selective lettering disappearance`
→ **`matrix/impression state difference observed`**

while:

`exact physical intervention`
remains **unresolved**.

This is exactly the distinction the repository ontology was designed to preserve:

`composition identity ≠ matrix identity ≠ matrix-state identity ≠ impression identity`.

---

## 5. Contextual consequence

The p.168 correction matters beyond source bookkeeping. The 1664 image belongs to the Igarassu/Garasu sequence rather than the later Ubatuba captivity scene. The earlier Batch-1 claim of radical contextual relocation based on the mistaken Ubatuba pairing is therefore withdrawn.

The broader dual-source architecture remains valid:

- Winckelmann's textual/arrangement access was mediated through later carriers such as Gottfried/Merian;
- at least some old Staden-associated physical matrices were available at Kassel;
- direct pairwise control now proves two such matrix survivals at pp.168 and 179;
- physical matrix survival still does not imply access to the 1557 princeps as a bibliographic object.

Thus the secure formulation remains:

`ACCESS TO OLD MATRIX STOCK ≠ ACCESS TO ORIGINAL BIBLIOGRAPHIC CONTEXT`.

---

## 6. Münster second-copy route

The Münster ULB second-copy target indices remain useful:

- p.168 → DFG viewer image 186;
- p.179 → image 197.

A Münster comparison could determine whether the observed lettering omissions are stable across 1664 copies and therefore more securely assignable to a matrix state rather than an impression-level anomaly.

This is now **bounded confirmatory refinement**, not an open research blocker.

Do not reopen generic raster hunting on its account.

---

## 7. Priority-1 closure judgment

**p.168 source occurrence: CORRECTED AND CLOSED.**  
**p.168 same-matrix identity: HIGH-CONFIDENCE DIRECT-RASTER VERIFIED.**  
**p.168 lettering-state difference: DIRECTLY OBSERVED; physical mechanism unresolved.**  
**p.179 same-matrix identity: HIGH-CONFIDENCE DIRECT-RASTER VERIFIED.**  
**p.179 lettering-state difference: DIRECTLY OBSERVED; physical mechanism unresolved.**  
**p.142 direct 1664 raster: RECOVERED; positive-control source occurrence secure.**  
**32-fold bulk same-matrix claim: STILL PROHIBITED without pairwise control.**  
**Münster second-copy test: NON-BLOCKING CONFIRMATORY REFINEMENT.**

Priority 1 is therefore **CLOSED**.
