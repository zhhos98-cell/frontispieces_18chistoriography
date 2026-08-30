# User action log

Purpose: single authoritative place for anything that requires the user's direct intervention.

## Workflow rule

- Any task that genuinely requires the user to act must be recorded here rather than scattered across chat messages or research notes.
- Each entry must state: `ID`, `status`, `object`, `why user action is required`, `minimum action`, `completion criterion`, and any relevant link/call number/file path.
- Do not create a user-action item merely because a route is inconvenient. First exhaust normal public-web, catalogue, repository, OCR, alternate-copy, and institutional-mirror routes.
- Chat may mention that an item has been logged, but this file remains the authoritative queue.
- When completed, retain the entry and mark it `DONE` with date/result so the evidentiary history is preserved.

## Open actions

### UA-001 — Winckelmann 1664 JCB full scan for p.168 / p.179 matrix testing

- **Status:** OPEN — user volunteered to handle direct download when faster than assistant-side page-image recovery.
- **Object:** Johann Just Winckelmann, *Der americanischen Neuen Welt Beschreibung* (Oldenburg, 1664), John Carter Brown Library copy, call `J664 W761a`, Internet Archive identifier `deramericanische00winc`.
- **Why user action is required:** assistant-side web access can read the IA OCR, catalogue metadata and item-level JCB records, but current fetch/render routes do not expose the full 31.99 MB PDF or sufficiently high-resolution direct rasters for printed pp.168 and 179. Those two pages are the decisive defect/linework test for whether the labelled 1557 Ubatuba and shipwreck matrices survive as altered states in 1664.
- **Minimum action:** download the complete PDF and upload it into the chat when convenient. Direct file: `https://archive.org/download/deramericanische00winc/deramericanische00winc.pdf`.
- **Completion criterion:** assistant receives a usable PDF or direct page images containing printed pp.168 and 179 (preferably also p.142 as positive control), renders them at high resolution, and records item-level matrix/state judgments against the controlled 1557 images.
- **Do not substitute:** screenshots of catalogue descriptions alone; the test requires actual printed image linework.

### UA-002 — Winckelmann 1684 Oldenburg Horn full scan for carrier/image-chain control

- **Status:** OPEN — user volunteered to handle direct downloads when faster than assistant-side page traversal.
- **Object:** Johann Just Winckelmann, *Des Oldenburgischen Wunder-Horns Ursprung/ Herkunft/ Materie/ Form/ Gestalt/ Figuren und Hieroglyphische Auslegung* (Bremen, 1684), Landesbibliothek Oldenburg digital copy, shelfmark `GE IX B 70 A`, URN `urn:nbn:de:gbv:45:1-3959`.
- **Why user action is required:** the official viewer exposes individual pages but the 31.79 MB complete PDF exceeds the current fetch layer. Direct carrier control is needed because the catalogue explicitly warns that one Wunderhorn illustration in the digital object is **not an original impression**, but a 1912 tracing by Fr. Schohusen after the original woodcut. The volume also contains three folded leaves and a mixed apparatus (`Ill. Holzschn.; 1 Kt. Kupferst.; 1 Ill. Kupferst.; 1 Ill. Holzschn.`), so image identity must be established before comparing the 1684 representation with Jacobaeus 1696 and the surviving object.
- **Minimum action:** download and upload the complete PDF. Direct file: `https://digital.lb-oldenburg.de/ihd/download/pdf/234884`.
- **Completion criterion:** assistant receives the PDF, isolates the original/1912-surrogate Horn image(s), map and copperplate/folded leaves, and performs the 1684 ↔ 1696 ↔ surviving-object comparison without conflating the 1912 tracing with a 1684 impression.
- **Catalogue warning:** `1 Ill. (Wunderhorn) nicht im Orig., sondern nach dem Orig.-Holzschn. durchgez. von Fr. Schohusen 1912`.

## Completed actions

None yet.
