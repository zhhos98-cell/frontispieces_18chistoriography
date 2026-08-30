# Winckelmann 1664 / Staden 1557 pairwise concordance — batch 1: pp.142, 168, 179

Date: 2026-08-28  
Corrected and superseded at direct-raster level: 2026-08-30  
Status: **SUPERSEDED BY DIRECT-RASTER CLOSURE. P.168 SOURCE MAPPING CORRECTED.**

Definitive successor:

`docs/WINCKELMANN_1664_DIRECT_RASTER_MATRIX_STATE_CLOSURE_P142_P168_P179_2026-08-30.md`

Companion data:

`data/winckelmann_1664_staden_pairwise_matrix_control_batch1_2026-08-28.csv`

## Correction notice

The original 2026-08-28 Batch-1 pass incorrectly mapped Winckelmann p.168 to Staden's Ubatuba attack woodcut. Direct comparison with the recovered 1664 p.168 raster shows that the correct 1557 source is:

`[Combate entre portugueses e índios caetés em Igarassu]`

Brasiliana Iconográfica / BBM ID `45000008047.28`.

The earlier `uwatibi` / Ubatuba discussion and the resulting claim of a Ubatuba composition recontextualized into the Igarassu sequence are withdrawn.

## Revised pairwise results

### p.142 — fishing with bows/arrows

1557 source:

`[Pescaria com arco e flecha]`, Brasiliana / BBM ID `45.000.008.047.139`.

A direct 1664 p.142 raster is now available from the user-assisted JCB/IA retrieval. JCB item `01512-5` controls the 1664 image dimensions at `10.5 × 10.8 cm` and gives an original-woodcut attribution. Source occurrence and composition are secure; p.142 remains the positive control.

### p.168 — Igarassu / Igaraçu battle

Correct 1557 source:

`[Combate entre portugueses e índios caetés em Igarassu]`, ID `45000008047.28`.

Direct 1557/1664 comparison shows dense whole-field concordance in watercourses, palisades, figures, vessels, terrain, frame and local line junctions. A supporting feature-registration test gives 49 ratio-filtered ORB matches with 41 RANSAC inliers (83.7%).

Revised status:

`SAME_MATRIX_AS_1557 = HIGH_CONFIDENCE_DIRECT_RASTER`

`LETTERING_STATE_DIFFERENCE = DIRECTLY_OBSERVED`

`PHYSICAL_REMOVAL_MECHANISM = UNRESOLVED`.

A small source place-name in the lower-left settlement/hill zone is absent in the inspected 1664 impression while surrounding linework remains concordant. Exact historical spelling is deliberately not normalized from the current small source image.

### p.179 — Itanhaém / São Vicente shipwreck

1557 source:

`[Naufrágio nas proximidades da povoação de Itanhaém]`, ID `45000008047.47`.

Direct comparison shows whole-field concordance in ship/rigging, waves, shorelines, settlements, figures and frame. Supporting registration gives 61 ratio-filtered ORB matches with 51 RANSAC inliers (83.6%).

Revised status:

`SAME_MATRIX_AS_1557 = HIGH_CONFIDENCE_DIRECT_RASTER`

`LETTERING_STATE_DIFFERENCE = DIRECTLY_OBSERVED`

`PHYSICAL_REMOVAL_MECHANISM = UNRESOLVED`.

The 1557 `S. vin` label and the upper-left settlement label are absent in the inspected 1664 impression; `S. maro` survives. This selective difference should be treated as a matrix/impression-state problem, not as evidence for a different composition or recut facsimile.

## Guardrail retained

Two direct pairwise same-matrix promotions do **not** authorize the old bulk claim that all 32 Staden-section images in Winckelmann 1664 have been independently verified as impressions from the same 1557 matrices.

The evidence rule remains:

`same composition`
≠ `same physical matrix`
≠ `same matrix state`
≠ `same impression state`.

For pp.168 and 179 the physical matrix relation is now directly controlled at high confidence. The exact mechanical cause of the lost lettering remains open, and the Münster second copy is retained only as a non-blocking confirmatory state test.
