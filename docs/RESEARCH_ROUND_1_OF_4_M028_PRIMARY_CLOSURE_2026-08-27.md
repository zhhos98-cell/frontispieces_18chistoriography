# Research round 1 of 4 — M028 Meiners 1792 primary closure

Date: 2026-08-27

## Scope

This is the first of the four planned closure rounds. It is deliberately restricted to the highest-value unresolved block:

Christoph Meiners, `Ueber die Farben, und Schattierungen verschiedener Völker`, *Neues Göttingisches historisches Magazin* I/4 (1792), pp.611–672 (`M028`).

No new comparator branch should be opened in this round.

## Current primary-access status

Primary carriers remain fixed:
- Internet Archive `neuesgttingisch00meingoog`;
- Google Books `3F4FAAAAIAAJ`;
- MPIWG `3GRRWV93`;
- BSB shelfmark `H.misc. 201-1`, URN `urn:nbn:de:bvb:12-bsb10738733-5`.

Automated browser routes currently expose metadata and derivative witnesses but not a clean continuous export of printed pp.611–672.

Manual escalation remains deliberately minimal:

> Download either the Internet Archive **PDF** or **FULL TEXT** for `neuesgttingisch00meingoog` and upload the whole file. No cropping, page extraction or OCR by the user is required.

On receipt, the analysis should programmatically locate printed pp.611–672 and run the finite falsification matrix in:

`docs/M028_MEINERS_1792_PRIMARY_VERIFICATION_MATRIX_AND_DERIVATIVE_LOCATOR_CORRECTION.md`.

## Verification matrix now fixed

Write-back:
- commit `460328f1603de9b17c344401bf01db5ddfcc9b47`.

Priority tests:
1. p.612 opening: colour as race/descent evidence; Hauptfarben; Grund-/Urfarben problem.
2. pp.614–615: differentiated external causal menu and distinction among cause / modifier / masking.
3. locate primary original of Krünitz's `am meisten von dem Blute der Eltern` sentence.
4. test physiological modifiers and causal equifinality.
5. pp.640–641 admixture / generational convergence and trait synchronization or decoupling.
6. locate the original trait-decoupling passage currently mislabelled in an older note as `p.679`.
7. concluding four Hauptfarben / two Urfarben structure and exact original page(s).
8. compare original section order, uncertainty markers and named evidence carriers against Krünitz's derivative organization.

## Locator correction

The older central method note uses `p.679 trait-decoupling case` as if it were Meiners's primary pagination.

That is impossible because the 1792 article ends on p.672.

Until the original is recovered:

`p.679 = derivative witness locator / unresolved bad locator`,

not:

`Meiners 1792 p.679`.

Do not cite the latter.

## Parallel chronology cleanup completed without opening a new branch

The anti-single-trait rule has been pushed earlier than the previous 1793 control.

Contemporary primary control:
- Blumenbach, *Beyträge zur Naturgeschichte* (1790), pp.62ff., states that he is reproducing remarks Meiners had printed in a note in *Göttingisches historisches Magazin* VI/3, pp.406–408.
- The reproduced Meiners passage rejects inference from one bodily part to whole peoples, from isolated bones to national morphology, and from skulls without geographical provenance to population varieties.

Repo update:
- `docs/MEINERS_ANTI_SINGLE_TRAIT_RULE_EDITION_CONTROL_1793_PRIMARY_TARGET_CORRECTION.md`
- commit `554ff5adc535f70b329414a63816441b850137da`.

Revised chronology:

`1785 p.23 = unresolved`
`→ 1790 = anti-single-trait / anti-isolated-specimen / provenance rule securely public`
`→ 1793 p.23 = same rule controlled in second-edition Grundriß`.

Therefore the 1793 rule should no longer be treated as a possible innovation specific to the 1793 revision.

## Sharpened M028 consistency test

Because the methodological rule was public by 1790, the 1792 colour essay can now be tested for consistency:

> Does Meiners actually subject skin colour to the provenance, multi-trait and population-warrant standards he had already articulated against single-part inference, or does he relax those standards when colour is used for racial, genealogical or hierarchical conclusions?

This is a primary-text falsification target, not a new theoretical branch.

## Round-closure condition

Round 1 closes when:
- printed pp.611–672 are directly available;
- every high-value matrix item is marked `confirmed / weakened / falsified / unresolved`;
- the central 1792 method note is updated to primary-safe pagination and evidence status;
- derivative-only locators are removed or explicitly labelled;
- no new comparator is added.

If the original substantially confirms the current reconstruction, proceed to round 2.
If Krünitz materially regularizes Meiners, spend at most one repair sub-pass inside this round and then close it.
