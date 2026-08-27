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

### Meiners 1793 *Grundriß*, second edition
- Halle DOI: `10.25673/56435`, URN `urn:nbn:de:gbv:3:1-454120`;
- shelfmark: ULB Sachsen-Anhalt `Na 1156`;
- Google Books full-view carrier located, ID `B0PWEZYUBEcC`;
- target pages are now sharply bounded by exact-page specialist controls: p.60 for the Kant 1785 race-essay citation; p.85 for the revised descent/climate passage corresponding to 1785 p.39.

The carrier is primary and public-domain, but the current automated HTML routes do not expose the target-page text. These page-specific claims remain `exact-page secondary control + primary carrier fixed`, not `primary_direct`.

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

## Publication-lag falsification refined — Blumenbach 1788 → 1797

Write-back commit: `3e354358b0c266d1691ccf376b95998976a12c4f`.

File:
- `docs/BLUMENBACH_1788_1797_MODULAR_PUBLICATION_LAG_CAUSAL_INTEGRATION_BEFORE_RACE_GATE.md`

Hard revision:
- 1788: Kantian persistence criterion is present in Blumenbach's private working apparatus.
- 1790 *Beyträge*: the public architecture explicitly foregrounds `Ausartung`, but the human division remains five `Spielarten`.
- 1791 fourth *Handbuch*: official Blumenbach Online editorial description identifies a real new public causal integration in §§13–15, where variation in the `Bildungstrieb` explains altered/new forms through `Ausartung / Degeneration`; the human section nevertheless remains five `Varietäten`.
- independent edition-history control reports that `Race` is absent from the 1791 fourth edition.
- 1795 *De generis humani varietate nativa*: major public anthropological recasting and first use of the five named `varietates`; do **not** yet promote this intermediate state to the explicit 1797 reproductive persistence gate without page-specific primary control.
- 1797 fifth *Handbuch*: explicit public `Rasse / Spielart` persistence gate with Kant/Girtanner framing.

The older binary model `private uptake → public adoption` is therefore too coarse.

Revised model:

`concept availability ≠ private categorical uptake ≠ public causal integration ≠ terminological adoption ≠ categorical jurisdiction ≠ explicit attribution`.

The important chronological result is **modular publication lag**: Blumenbach publicly reorganized causal natural history before he publicly stabilized the race/variety hereditary gate.

Stop rule:
- chronological proximity does not prove that the 1791 causal revisions were directly caused by Kant; Blumenbach's own Bildungstrieb trajectory, Buffonian degeneration and multiple-source interaction remain live explanations.

## Meiners–Kant access question closed at the weak level

Write-back commit: `154d6bba4a900669c7d1b2b90f757243e4356103`.

File:
- `docs/MEINERS_KANT_DIRECT_ENGAGEMENT_AND_REPURPOSING_OF_HEREDITARY_DESCENT_1788_1793.md`

Hard revision:
- Meiners and Feder jointly edited the *Philosophische Bibliothek* from 1788 to 1791; specialist work describes this journal as systematizing Meiners's Kant controversy and extending it across Kant's oeuvre.
- the weak hypothesis that Meiners needed Blumenbach as his route to Kantian conceptual material is therefore unnecessary.
- race-specific specialist work finds Meiners's explicit references to Kant's race writings comparatively rare, but identifies selective Kantian uptake by 1790: hereditary permanence and descent receive increased weight relative to place/climate.
- the 1793 second edition of the *Grundriß* is reported to cite Kant's 1785 race essay at p.60 and to revise a 1785 passage at p.39 into a 1793 p.85 formulation that removes a climate reference in order to highlight `Abstammung`.
- the public-domain 1793 primary carrier is now fixed, but target-page direct extraction failed in the current automated route. Keep these two exact-page claims below `primary_direct` until page images/text are inspected.

Consequent research shift:

The central question is no longer:

> Did Meiners have access to Kant's persistence/descent concepts?

It is now:

> Which Kantian operations did Meiners selectively appropriate, and what inferential work did he authorize with them that Blumenbach did not?

Provisional operational contrast, to be tested against direct pages:

- Blumenbach: `persistence test → category jurisdiction`;
- Meiners: `persistence / descent claim → inferential amplification within historical, evaluative and political reasoning`.

This does **not** mean that Meiners faithfully adopted Kant, nor that Kant supplies Meiners's political conclusions. It means access/non-availability is no longer a sufficient explanation for divergence.

## Revised core problem

The earlier question remains useful but can now be made sharper:

> Why did scholars operating in the same Göttingen information environment authorize different operations on visible human difference when both conceptual and textual resources overlapped?

Test dimensions:
- source corpus / evidence carrier;
- private vs public knowledge state;
- genre;
- inference target;
- interpersonal transfer;
- disciplinary jurisdiction;
- selective appropriation;
- module-specific publication lag;
- jurisdiction expansion from natural history into historical or political inference.

## Next automatically tractable targets

1. **Meiners exact Kant uptake.** Primary-close the 1793 *Grundriß* p.60 Kant citation and compare 1785 p.39 with 1793 p.85. The carriers and exact pages are fixed; do not treat failed automated extraction as negative evidence.
2. **Meiners 1790 race essays.** Map explicit Kant citations versus unattributed Kantian operations at exact pages, especially `Ueber die Natur der Afrikanischen Neger` around pp.395–399 and `Von den Varietäten und Abarten der Neger` from p.625 onward. Separate source borrowing from inferential repurposing.
3. **Blumenbach 1795 intermediate state.** Test the primary Latin text for an explicit hereditary-persistence threshold before 1797. Until that is located, code 1795 as public anthropological recasting, not as a closed persistence-gate adoption.
4. Continue apparatus/network work while manual queue M028–M031 remains pending.

No further theory expansion should override the primary-closure priority.
