# User action log

Purpose: single authoritative place for anything that requires the user's direct intervention.

## Workflow rule

- Any task that genuinely requires the user to act must be recorded here rather than scattered across chat messages or research notes.
- Each entry must state: `ID`, `status`, `object`, `why user action is required`, `minimum action`, `completion criterion`, and any relevant link/call number/file path.
- Do not create a user-action item merely because a route is inconvenient. First exhaust normal public-web, catalogue, repository, OCR, alternate-copy, and institutional-mirror routes.
- Completed actions are retained for evidentiary history.
- A parked refinement is **not** an open research blocker and must not keep the repository in an active state.

## Open blocking actions

**None.**

## Completed actions

### UA-001 — Winckelmann 1664 JCB pages for p.168 / p.179 matrix testing

- **Status:** DONE — 2026-08-30.
- **Object:** Johann Just Winckelmann, *Der americanischen Neuen Welt Beschreibung* (Oldenburg, 1664), John Carter Brown Library copy, call `J664 W761a`, Internet Archive identifier `deramericanische00winc`.
- **User contribution:** direct page images for printed pp.168 and 179 were supplied, together with p.142 as positive control and 1557 Brasiliana comparison material.
- **Completion result:** p.168 source occurrence corrected from the previously misassigned Ubatuba plate to the 1557 Igarassu battle plate; direct whole-field image concordance promotes pp.168 and 179 to high-confidence same-matrix relations and directly controls selective lettering-state differences.
- **Mechanism guardrail:** the exact physical cause of the lettering differences remains unresolved; do not specify cutting, plugging, masking, selective inking, damage, or another intervention without stronger copy/state evidence.
- **Definitive checkpoint:** `docs/WINCKELMANN_1664_DIRECT_RASTER_MATRIX_STATE_CLOSURE_P142_P168_P179_2026-08-30.md`.
- **Former download route:** `https://archive.org/download/deramericanische00winc/deramericanische00winc.pdf`.

## Parked non-blocking refinements

### UA-002 — Winckelmann 1684 Oldenburg Horn full scan for carrier/image-chain control

- **Status:** PARKED — NON-BLOCKING REFINEMENT.
- **Object:** Johann Just Winckelmann, *Des Oldenburgischen Wunder-Horns Ursprung/ Herkunft/ Materie/ Form/ Gestalt/ Figuren und Hieroglyphische Auslegung* (Bremen, 1684), Landesbibliothek Oldenburg, shelfmark `GE IX B 70 A`, URN `urn:nbn:de:gbv:45:1-3959`.
- **Why it was logged:** the official digital object mixes historical material with a catalogue-noted 1912 Schohusen tracing after an original woodcut. Full local collation would allow exact carrier identification before comparing the 1684 representation with Jacobaeus 1696 and the surviving object.
- **Current research status:** broad Horn research is closed. Object-access/source-criticism chain, digital carrier warning, 1696 Tab. XVI presence, and long-range reuse are already controlled. The full scan can refine the direct image genealogy but is not required for repository closure.
- **Optional minimum action if this branch is deliberately reopened:** download and upload `https://digital.lb-oldenburg.de/ihd/download/pdf/234884`.
- **Reopen condition:** only if direct 1684 carrier identity or the exact `1696 derived_from 1684` image relation becomes necessary for a publication claim.
- **Closure checkpoint:** `docs/WINCKELMANN_1684_HORN_CARRIER_FIREWALL_AND_DIRECT_IMAGE_BOUNDARY_2026-08-30.md`.
