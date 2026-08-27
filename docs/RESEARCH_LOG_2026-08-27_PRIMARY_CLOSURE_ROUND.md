# Research log — 2026-08-27 — Primary closure / falsification round

This log begins after the closure of Sweep 4. The governing instruction for this round is: **primary closure and falsification before further theory expansion**.

## Manual-escalation rule adopted

Formal policy commit: `4bc8fe8e11630378e5826a136b5c058b13c5c6a2` (`docs/EVIDENCE_POLICY.md`).

Operational queue commit: `358b1f364faa344b5be9d749d8a0353285669a31` (`docs/MANUAL_DOWNLOAD_AND_INSPECTION_LOG.md`).

Rule:
- if a historical target is sharply bounded but automated access is disproportionately costly;
- and one click/download/OCR/screenshot by the user is likely to close it cheaply;
- log it in the single manual queue and **do not stall the main sweep**;
- keep the claim at its present evidence status until the manual material arrives;
- if automation later closes it first, mark the item `resolved_no_manual_needed`.

Current high-priority manual escalations:
- `M028` — Meiners 1792 colour essay, pp.611–672: bounded OCR/export of the original article;
- `M029` — Meiners 1785 *Grundriß*, p.23: primary check of the anti-single-body-part rule;
- `M030` — Zimmermann 1778, pp.94–115: bounded OCR of colour/climate/migration discussion;
- `M031` — Meiners 1810 sale catalogue: keyword search for Prange / Lambert / Schäffer / related colour works.

## Primary source carriers now fixed

### Meiners 1792
- Google Books object: `3F4FAAAAIAAJ`;
- Internet Archive identifier: `neuesgttingisch00meingoog`;
- MPIWG object: `3GRRWV93`;
- BSB shelfmark: `H.misc. 201-1`, URN `urn:nbn:de:bvb:12-bsb10738733-5`.

The current environment still fails on direct target-page retrieval. This is now a manual-queue problem, not a reason to pause research.

### Meiners 1785 *Grundriß*
- Open Library edition: `OL26631818M`;
- Internet Archive identifier: `grundrissdergesc00mein`;
- Halle DOI: `10.25673/60781`, URN `urn:nbn:de:gbv:3:1-636379`;
- public-domain PDF / IIIF are available through Halle.

### Zimmermann 1778
- Google Books full-view object located, including ID `7tINaWqBUA0C`;
- Internet Archive identifier previously located: `geographischege00zimmgoog`.

## Library control

A Library search for the exact Meiners 1792 article/title and distinctive phrases returned Araújo and other secondary/derivative material, not the 1792 primary volume itself. This does **not** establish absence from the entire Library; it establishes only that the current semantic search did not expose a usable primary copy. Do not waste the round repeatedly probing the same Library route.

## Automatically tractable branch closed — Girtanner 1796 / Blumenbach 1797

Write-back commit: `e6ff7cfb0016640918109e699ff588152befbe25`.

File:
- `docs/COLOUR_METHOD_HEREDITARY_PERSISTENCE_GATE_GIRTANNER_BLUMENBACH_1796_1797.md`

Hard closure:
- Blumenbach's 1797 fifth-edition *Handbuch* gives a primary-direct definition of `Rasse` as a character produced through `Degeneration` that is unavoidably and necessarily inherited through reproduction; a `Spielart` lacks this necessary reproductive consequence.
- The same note explicitly credits Kant's 1788 distinction and directs readers to Girtanner 1796 for fuller treatment.
- This supplies a downstream `persistence gate`: a visible difference is not admitted to race-level classificatory jurisdiction merely because it is perceptible, repeated or causally intelligible; it must be construed as necessarily transmissible through generation.

Current analytical chain:

`visible difference → reproductive persistence test → necessary inheritance claim → historical memory → category / inference jurisdiction`.

Important contrast with provisional Meiners 1792 reconstruction:
- Meiners: plural causal field + causal underdetermination + triangulation;
- Girtanner/Blumenbach downstream control: persistence functions as a categorical threshold.

Girtanner evidence status:
- primary book located (Google Books full view; ETH/e-rara DOI `10.3931/e-rara-42705`);
- Google Books indexes `Farbe der Haut`, `Gesichtsbildung`, `Haare`, `Schminke`, `erblichen`, `Rasse`, `Spielart`, etc.;
- exact page-specific claims such as the p.39 inheritance principle and the characterization of climatic skin-colour change as non-heritable `Schminke` remain controlled through page-specific modern scholarship until direct primary extraction is completed.

Do **not** project this 1796–97 persistence criterion backward into Meiners 1792 without transfer evidence.

## Next automatically tractable targets

1. Test whether Girtanner's persistence gate changes only nomenclature (`Rasse` / `Spielart`) or the causal narratives allowed for human history.
2. Search pre-1792 Göttingen materials for an explicit persistence threshold, especially Blumenbach's handwritten 1788 Kant notes, without assuming publication-level circulation.
3. Continue apparatus/network work on sources that do not depend on the manual queue.
