# Winckelmann 1664 Münster copy: scan-index control for pp.168, 171, 179

Date: 2026-08-28

Status: INSTITUTIONAL STRUCTURE-METADATA CONTROL — TARGET PRINTED PAGES ARE NOW MAPPED TO EXACT PHYSICAL SCAN INDICES IN THE ULB MÜNSTER 2011 DIGITAL COPY. DIRECT RASTER EXTRACTION / MATRIX COMPARISON REMAINS NEXT.

## Result

The ULB Münster second digital copy is now structurally controlled through zvdd rather than inferred from OCR or pagination guesswork.

Work:

Johann Just Winckelmann, *Der Americanischen Neuen Welt Beschreibung* (Oldenburg: Zimmer, 1664).

ULB Münster digital edition: 2011.

Formal URN:

`urn:nbn:de:hbz:6:1-15914`

Extent recorded by zvdd:

`[7] Bl., 228 S., [6] Bl. : Ill., Portr. ; quer-4-o`

The zvdd table of contents links structural chapter starts directly into the DFG Viewer. Two independent anchors provide a fixed printed-page/scan-image offset:

- printed p.163, start of chapter XIV (`Erste Schifffart Johan Staden ...`) → DFG Viewer `image=181`;
- printed p.172, start of chapter XV (`Zweyte Schiffart Johan Staden ...`) → DFG Viewer `image=190`.

Thus across the target interval:

`scan_image = printed_page + 18`.

Target mappings are therefore:

- printed **p.168 → scan image 186**;
- printed **p.171 → scan image 189**;
- printed **p.179 → scan image 197**.

Evidence status:

`PRINTED-PAGE → SECOND-COPY SCAN-INDEX MAPPING = INSTITUTIONAL STRUCTURE METADATA CONTROLLED`.

This is stronger than the earlier OCR-based page-location inference. The remaining obstacle is transport/display of the raster itself, not identification of the physical page.

## Source controls

zvdd bibliographic record:

`https://www.zvdd.de/dms/load/met/?PPN=urn:nbn:de:hbz:6:1-15914`

zvdd structural table of contents:

`https://www.zvdd.de/dms/load/toc/?PPN=urn:nbn:de:hbz:6:1-15914`

The chapter-XIV structural link resolves through zvdd to a DFG Viewer call whose selected image is `181`; the chapter-XV structural link resolves to selected image `190`.

The zvdd record also exposes a METS XML route. Current retrieval infrastructure recognizes the route but does not render the XML response directly; this is a transport-layer issue and should not be escalated to a user action while alternate image-access routes remain.

## Matrix/state targets once rasters are retrieved

### p.168 / scan 186

Obermeier identifies the motif as an attack by Indigenous people on an Indigenous village, corresponding to the inherited Staden image repertory while occurring in a different narrative context in Winckelmann. JCB catalogue metadata further reports that names present on the original were eliminated in the 1664 occurrence.

Compare against the 1557 Ubatuba-village attack occurrence for:

- border/frame geometry;
- surviving and missing labels;
- exact internal line junctions;
- cuts, gaps, cracks, filling, recutting or wear;
- dimensions and cropping;
- whether label suppression is a stable matrix state.

### p.171 / scan 189

Obermeier identifies the round-ship image and notes the upper-left fish-mouth recut/completed state, already observable in repeat impressions within the 1557 edition.

Use this only as a diagnostic state feature after independent same-matrix tests based on frame/line/defect concordance.

### p.179 / scan 197

Obermeier independently identifies the São Vicente / Itanhaém shipwreck scene; JCB reports elimination of names present in the original. The 1557 image visibly carries several geographic labels.

This is currently the highest-value label-state pair.

## Methodological consequence

The second-copy route is no longer an undefined future task. We know exactly which three physical scans must be compared:

`186 | 189 | 197`.

Therefore the next operation should be raster acquisition, not renewed page identification.

Do not change any `same_matrix` status merely because the page-index problem has been solved.