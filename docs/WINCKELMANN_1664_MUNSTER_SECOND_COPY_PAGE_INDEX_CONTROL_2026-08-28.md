# Winckelmann 1664: Münster second-copy page-index control

Date: 2026-08-28  
Status: STRUCTURAL PAGE-MAPPING CONTROL — THE MÜNSTER ULB SECOND DIGITAL COPY IS NOW RESOLVED TO EXACT DFG-VIEWER IMAGE INDICES FOR THE THREE PRIORITY MATRIX/STATE TARGETS. THIS DOES NOT YET CONSTITUTE RASTER-LEVEL MATRIX VERIFICATION.

## Source copy

ZVDD / Münster ULB digital copy:

- URN: `urn:nbn:de:hbz:6:1-15914`
- title: Johann Just Winckelmann, *Der Americanischen Neuen Welt Beschreibung*, Oldenburg, 1664
- Münster ULB online edition: 2011
- extent: `[7] Bl., 228 S., [6] Bl. : Ill., Portr. ; quer-4-o`

ZVDD metadata:

`https://www.zvdd.de/dms/load/met/?PPN=urn:nbn:de:hbz:6:1-15914`

ZVDD table of contents:

`https://www.zvdd.de/dms/load/toc/?PPN=urn:nbn:de:hbz:6:1-15914`

## Exact offset control

The structured ZVDD/DFG-viewer links expose two independent anchors within the same Staden section:

- printed p.163 -> DFG-viewer `set[image]=181`
- printed p.172 -> DFG-viewer `set[image]=190`

Both yield the same relation:

`viewer_image_index = printed_page + 18`.

Because the two anchors are nine printed pages apart and the viewer indices are also nine images apart, the local mapping is internally consistent across the interval containing the first two priority targets and extends directly to the third target unless an unrecorded inserted scan occurs after p.172. The structured contents give no indication of such an insertion in this run; direct raster retrieval remains the final check.

## Priority target indices

Therefore the current second-copy target map is:

| printed page | target | Münster DFG-viewer image index | current status |
|---:|---|---:|---|
| 168 | attack on Indigenous village; JCB reports original names eliminated | 186 | PAGE INDEX CONTROLLED; RASTER PENDING |
| 171 | round ship; upper-left fish-mouth recut diagnostic | 189 | PAGE INDEX CONTROLLED; RASTER PENDING |
| 179 | São Vicente / Itanhaém shipwreck; JCB reports original names eliminated | 197 | PAGE INDEX CONTROLLED; RASTER PENDING |

DFG-viewer structure form exposed by ZVDD:

`https://dfg-viewer.de/show/?set[mets]=https://www.zvdd.de/dms/metsresolver/?PPN=urn:nbn:de:hbz:6:1-15914&set[image]=N`

where current target `N` values are 186, 189, 197.

## Evidence discipline

This result upgrades only the retrieval layer:

`SECOND COPY EXISTS`
+
`EXACT TARGET SCAN INDICES RESOLVED`

not:

`TARGET RASTERS INSPECTED`

and not:

`SAME_MATRIX_AS_1557 VERIFIED`.

Once the three raster pages are recovered, compare in this order:

1. composition and orientation;
2. outer frame geometry and dimensions;
3. integral lettering / labels;
4. distinctive line junctions;
5. stable defects, cracks, losses, filling and wear;
6. p.171 fish-mouth recut state;
7. compare the Münster occurrence with the JCB/IA 1664 copy to distinguish stable matrix state from copy/impression-level anomaly.

## Repository payoff

The second-copy state-control route is now structurally resolved. The remaining barrier is page-image transport rather than bibliographic identification or page-number uncertainty. Do not escalate this to a user action while public viewer / METS / IIIF / derivative routes remain available.