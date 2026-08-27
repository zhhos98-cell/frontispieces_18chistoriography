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

## Next automatically tractable branch

Proceed to Girtanner 1796 / Blumenbach 1797 and close the downstream criterion by which a variable bodily character becomes a reproductively persistent `Rasse`. This branch is kept downstream of Meiners 1792 unless direct transfer evidence appears.
