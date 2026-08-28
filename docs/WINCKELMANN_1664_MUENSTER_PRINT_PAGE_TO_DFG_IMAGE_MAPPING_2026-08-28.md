# Winckelmann 1664 Münster copy: printed-page → DFG image-index mapping

Date: 2026-08-28  
Status: STRUCTURAL-METADATA CONTROL — THREE INDEPENDENT CHAPTER-START LINKS IN THE ZVDD/DFG-VIEWER STRUCTURE ESTABLISH A STABLE `printed page + 18 = DFG image index` RELATION ACROSS THE STADEN SECTION. THIS LOCATES THE TARGET RASTERS P.168, P.171, P.179 WITHOUT GUESSING THE SCAN LEAF.

## Source copy

ZVDD record for the ULB Münster digital copy:

- Johann Just Winckelmann, *Der Americanischen Neuen Welt Beschreibung*, Oldenburg: Zimmer, 1664;
- online edition: Münster, Universitäts- und Landesbibliothek, 2011;
- extent: `[7] Bl., 228 S., [6] Bl. : Ill., Portr. ; quer-4-o`;
- URN: `urn:nbn:de:hbz:6:1-15914`.

ZVDD bibliographic record:

https://www.zvdd.de/dms/load/met/?PPN=urn%3Anbn%3Ade%3Ahbz%3A6%3A1-15914

ZVDD table of contents:

https://www.zvdd.de/dms/load/toc/?PPN=urn%3Anbn%3Ade%3Ahbz%3A6%3A1-15914

The table-of-contents entries link each chapter start to the corresponding image position in the DFG Viewer.

---

## 1. Three direct structural anchors

### Printed p.163 — chapter 14

ZVDD TOC:

`Das vierzehnde Capitel. Erste Schifffart Johan Staden ...` → printed p.163.

Following the linked DFG-viewer route resolves to:

`set[image]=181`.

Therefore:

`163 + 18 = 181`.

### Printed p.172 — chapter 15

ZVDD TOC:

`Das fünfzehnde Capitel. Zweyte Schiffart Johan Staden ...` → printed p.172.

Following the linked DFG-viewer route resolves to:

`set[image]=190`.

Therefore:

`172 + 18 = 190`.

### Printed p.223 — chapter 16

ZVDD TOC:

`Das sechszehnde Capitel. Schluß Rede` → printed p.223.

Following the linked DFG-viewer route resolves to:

`set[image]=241`.

Therefore:

`223 + 18 = 241`.

The same offset is independently reproduced at the beginning, middle, and end of the Staden narrative sequence:

`DFG image index = printed page + 18`.

Evidence status:

`+18 OFFSET THROUGH STADEN SECTION = CONTROLLED BY THREE INDEPENDENT STRUCTURAL ANCHORS`.

This is materially stronger than estimating from front-matter extent alone, because foldouts, covers, endsheets, or access-format exclusions can otherwise disturb naïve page arithmetic.

---

## 2. Target pages now located exactly

Applying the controlled relation:

| printed page | target | DFG image index | status |
|---|---|---:|---|
| 168 | Indigenous-village attack; JCB reports eliminated names | 186 | `DERIVED_FROM_THREE_STRUCTURAL_ANCHORS` |
| 171 | round ship; fish-mouth recut diagnostic | 189 | `DERIVED_FROM_THREE_STRUCTURAL_ANCHORS` |
| 179 | São Vicente / Itanhaém shipwreck; JCB reports eliminated names | 197 | `DERIVED_FROM_THREE_STRUCTURAL_ANCHORS` |

Thus future page-image retrieval should request **DFG images 186, 189, and 197** for the Münster copy.

Do not confuse these DFG image indices with:

- printed page numbers;
- ULB Münster internal `dpage/pageview` identifiers;
- Internet Archive leaf numbers;
- Wikimedia Commons PDF page numbers.

Those identifier systems remain distinct even where they refer to the same physical leaf.

---

## 3. Why this matters for the matrix comparison

The next physical comparison no longer has a page-identification ambiguity. Once the three DFG images or their underlying `FLocat` resources are recovered, compare them against the 1557 targets in this order:

### p.168 / DFG image 186

1557 motif: attack on an Indigenous village (`Ataque dos Tupiniquins à aldeia de Ubatuba` / Staden first-book chapter-29 attack motif in the current concordance).

Test:

- frame geometry;
- integral label inventory;
- exact line junctions;
- wear, breaks, splits, plugs, recutting;
- dimensions;
- whether JCB's reported missing names are a stable matrix state in the Münster copy as well as the JCB copy.

### p.171 / DFG image 189

1557 target: round-ship reusable block.

Diagnostic:

- upper-left fish-mouth recut/completed state described by Obermeier;
- but independently establish matrix identity before using state resemblance as proof.

### p.179 / DFG image 197

1557 target: São Vicente / Itanhaém shipwreck composition.

Test:

- geographic labels present in 1557;
- exact labels absent in 1664;
- stable state across Münster and JCB copies;
- physical alteration vs impression-level suppression vs recut-copy hypothesis.

---

## 4. Current retrieval bottleneck

The ZVDD structural layer exposes the DFG image index, but the current web environment blocks direct following of the nested DFG-viewer query URL and rejects the raw METS XML content type. This is a tool-routing restriction, not a source-access or page-identification problem.

Current next route:

`DFG image 186/189/197`
→ recover the corresponding METS `FLocat` / ULB Münster page resource
→ retrieve raster
→ physical side-by-side comparison.

This remains an assistant-side retrieval task and should **not** be escalated to `docs/USER_ACTION_LOG.md` at this stage.

---

## 5. Evidence rule

The mapping established here may be used to identify the target leaves, but it does not itself upgrade matrix identity.

Keep separate:

`PRINTED PAGE IDENTITY`
≠ `DIGITAL IMAGE POSITION`
≠ `COMPOSITION IDENTITY`
≠ `PHYSICAL MATRIX IDENTITY`
≠ `MATRIX STATE`.
