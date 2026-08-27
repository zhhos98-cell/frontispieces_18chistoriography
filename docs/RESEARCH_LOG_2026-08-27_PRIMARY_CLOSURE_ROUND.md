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

## Pre-1792 falsification closed — Blumenbach 1788 private working copy

Write-back commit: `3a09a7d7f7465ddf146e4a7a8227afd5c1fe0e0e`.

File:
- `docs/BLUMENBACH_1788_PRIVATE_PERSISTENCE_GATE_AND_PUBLIC_ADOPTION_LAG.md`

Hard chronological revision:
- Blumenbach's private hand-copy of the third-edition *Handbuch der Naturgeschichte* (1788), SUB Göttingen `Cod. Ms. Blumenbach XVII`, already contains handwritten notes summarising the Kantian distinction between necessarily inherited race-characters and non-necessarily inherited varieties.
- Opposite printed p.22, Blumenbach records the `necessary inheritance → Race / non-necessary → Varietät` distinction.
- Opposite printed p.60, he records `Race` as a radical peculiarity indicating common descent and again notes the formula that a class difference within one stem counts as race insofar as it is unavoidably hereditary; the same working note also contains a Forster/Cook reference.
- The digital manuscript object is identified through Blumenbach Online (`ID 00036 / 00036.pdf`), but direct facsimile retrieval failed in the current web environment. Current status is therefore `primary object identified + scholarly transcription control`, not `primary_direct_facsimile`.

Consequence:

`concept publicly available ≠ private uptake ≠ published adoption ≠ cross-disciplinary uptake`.

The persistence gate was conceptually and locally available in Göttingen before Meiners's 1792 colour essay. Therefore the contrast between Blumenbach and Meiners cannot be explained by chronological non-availability alone.

New core question:

> Why did co-located scholars authorize different operations on visible human difference even when some of the relevant conceptual tools were already available in the same intellectual environment?

Possible dimensions to test, not assume:
- source corpus / evidence carrier;
- private vs public knowledge state;
- genre;
- inference target;
- interpersonal transfer;
- disciplinary jurisdiction.

## Next automatically tractable targets

1. Test whether the 1788 Blumenbach hand-copy annotations can be tied to subsequent published changes before 1797, without backdating later wording.
2. Search Meiners's own methodological / reading practices for evidence that he encountered Kant's 1788 persistence criterion independently of Blumenbach.
3. Continue apparatus/network work while manual queue M028–M031 remains pending.
