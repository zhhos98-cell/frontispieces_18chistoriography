# Tincture encoding as information architecture — Siebmacher 1605/1609 → Spener 1680 → 1772 retrospective

## Status

The project's 1772 publisher-side complaint about tincture notation can now be placed inside a much longer, technically explicit history of representing heraldic colour in monochrome print. Three stages are currently controlled at different evidentiary levels:

1. **Siebmacher 1605** — institutional bibliographic records preserve the work's own extended title/colour `Declaration`, explicitly explaining that the colours are stated so the work can be completed and so an individual purchaser (`emptor`) may have the arms `illuminiren und erhöhen` according to preference. This establishes a text-to-colouring workflow directly at title/paratext level.
2. **Siebmacher 1609** — a modern scholarly article in *Archivum Heraldicum* (2019), citing Gert Oswald, states that the second part uses lower-case letters on the plates to denote tinctures, e.g. `g` = Gold, `b` = Blau, `w` = Weiss/Silber. This is presently a secondary scholarly control; direct inspection of a 1609 plate would promote it to image-level primary control.
3. **Spener 1680** — direct primary text explains that his copperplates use the French method of dots and differently directed lines for metals and colours because Germans had hitherto used colour initials; when figures are too small for line systems to distinguish tinctures adequately, the reader must return to the printed explanation.
4. **Weigel/Raspe 1772** — the already controlled publisher retrospective says that earlier attempts to mark tinctures by letters had produced disorder and misunderstanding; this complaint is coupled to excessive compression, insufficient descriptive space and the changing nature of coats of arms.

These stages should not be written as a universal linear replacement of one system by the next. Textual colour descriptions, letter codes, hatch/dot systems, verbal blazons and hand colouring could coexist, recur or be distributed differently across editions and copies. The stronger claim is about **competing and complementary channels for transmitting colour information under the constraints of monochrome engraving**.

## I. 1605: verbal colour declaration is explicitly tied to later illumination

The institutional record for Johann Siebmacher's *New Wapenbuch* preserves the extended wording:

`Declaration Und Nothwendige vermeldung ... gehörigen Farben / damit ... ein jeder emptor, deme es beliebte / sie also seinem gefallen nach illuminiren und erhöhen lassen könne`.

The key operational fact is that the printed state need not itself contain the final colour appearance. The work supplies colour information that can guide a subsequent act of illumination.

This produces at least three materially distinct information states:

`engraved shape / shield geometry`
+
`verbal statement of tinctures`
→
`reader or hired colourist can reconstruct colour`
→
`hand-coloured copy`.

The 1605 `Declaration` is therefore not merely descriptive prose. It can function as **instructions for transforming an uncoloured printed object into a coloured copy**.

That distinction matters for copy census. Two copies struck from the same plate can carry different evidentiary affordances:

- uncoloured impression + verbal colour key;
- partially illuminated impression;
- fully illuminated impression;
- later owner colouring, which may or may not faithfully follow the supplied information.

The repository should not treat `colour_present` as an inherent property of the engraved matrix.

### Evidence level

The wording is preserved in HAB/LibReTo's reconstruction of the Gandersheim library, tied to VD17 and a digitised ONB carrier. This is strong institutional bibliographic control of the title/paratext wording. A page-image check of the `Declaration` would still be useful for exact layout and whether the colour statements are organised as a continuous list, plate-by-plate register or another format.

## II. 1609: colour information moves onto the engraved image through letters

A 2019 article in *Archivum Heraldicum* states that the earlier Siebmacher issue did not yet put colour indications on the plates and that in the 1609 second part the colours were designated by lower-case letters. The article gives concrete examples:

- `g` = Gold;
- `b` = Blau;
- `w` = Weiss / Silber.

The article cites Gert Oswald, *Lexikon der Heraldik* (1984), p. 353. A separate modern heraldic literature also reports that the later/second issue of the first part incorporated such letters and could consequently dispense with the separate colour-description text. Until an actual 1609 plate is directly inspected, keep the latter edition-state claim below primary image verification.

At the level presently safe to use, the important transition is:

`colour information adjacent to / separate from image`
→
`abbreviated colour information embedded in image`.

This compresses the information architecture. A user no longer has to move from shield to a separate prose colour declaration in order to identify every tincture; the plate itself carries a symbolic surrogate.

But the compression has costs:

- the user must know the code;
- letters occupy graphic space;
- a small or crowded figure may make code placement ambiguous;
- the code gives categorical colour information without reproducing colour perceptually;
- copied, worn or poorly printed letters can become uncertain.

These are precisely the kinds of trade-offs that become explicit in Spener and, retrospectively, in 1772.

## III. 1680 Spener: hatching replaces initials on the plate, but prose remains a fallback

Spener's *Historia insignium illustrium* gives the strongest primary technical statement in the chain. In the preface he says his engraved tables use the French manner of indicating metal and colour by `punctulis aut lineolis`, with lines transverse, perpendicular, diagonal or cross-hatched. He explains the reason historically: `hactenus nostri literis initialibus colorum solebant indicia facere` — Germans had hitherto been accustomed to indicating colours with their initial letters.

This sentence explicitly identifies **letter initials as a pre-existing German graphic convention** and positions Spener's dot/line system as an alternative.

The next sentence is equally important. Where figures are too small for the lines to distinguish the colours sufficiently, `ad explicationem typis expressam recurrere necesse erit`: one must recur to the explanation expressed in type.

The architecture is therefore not:

`letters → hatching → prose obsolete`.

It is:

`graphic coding system`
↔
`figure scale / visual resolution`
↔
`printed verbal explanation as redundancy / fallback`.

This is an unusually explicit early-modern statement of **multi-channel information design**. The image carries as much tincture information as its scale permits; prose takes over when the graphic channel loses discriminating power.

## IV. 1772 retrospective: letter codes become part of a diagnosis of armorial failure

The Weigel/Raspe `Vorbericht` to the cumulative Wappenbuch, already controlled in `docs/PUBLISHER_RETROSPECTIVE_KOHLER_1723_VISUAL_INFORMATION_PROBLEM_1772_2026-08-26.md`, criticises the older armorial ecology on several linked grounds:

- attempts to include very large numbers of arms forced figures into a format too small for adequate clarity;
- blazoning had not yet been sufficiently determinate;
- later attempts to indicate tinctures by letters led to disorder and misunderstanding;
- the huge corpus left too little room for descriptions;
- arms themselves changed and received augmentations over time.

The tincture complaint should now be read not as an isolated remark but as a retrospective judgment on a demonstrably older encoding regime.

A bounded technical genealogy is therefore available:

`1605 verbal tincture declaration supports hand illumination`
→
`1609 letter-coded tinctures embedded in plates`
→
`1680 Spener explicitly contrasts German colour initials with dot/line hatching and retains prose as small-scale fallback`
→
`1772 publisher retrospective judges letter notation to have generated confusion within older armorial publication`.

This is a history of **information channels and their limits**, not a simple narrative of technical progress.

## V. Colour is a copy-state problem as well as a representation problem

The chain strengthens several already established copy-level controls in this repository. Existing eighteenth-century witnesses include fully or partly coloured copies, black-and-white copies, incomplete colour states and materially altered copies. The early Siebmacher evidence shows why those differences cannot be treated as mere decoration.

A useful copy schema should distinguish:

`matrix contains no tincture code`
`matrix contains letter code`
`matrix contains hatch/dot code`
`verbal tincture description present`
`contemporary hand colouring present`
`partial colouring present`
`later/owner colouring suspected`
`colour information lost through missing leaf / abrasion / cropping`.

Several of these properties can coexist in one copy.

The analytical consequence is important: **same matrix does not imply same accessible colour information**. The matrix may encode tincture symbolically, while one owner additionally sees actual pigment and another relies only on letters/hatching/prose. A later colourist can also introduce a new error layer not present in the engraved code.

## VI. Encoding and finishing should be kept separate

The project should distinguish two questions that are easy to collapse:

### Encoding
How does a monochrome print state represent the semantic category of colour?

Possible channels:

- prose description;
- initials / letters;
- dot and line conventions;
- cross-reference to a key or blazon.

### Finishing
What happens to a particular physical impression after printing?

Possible states:

- remains monochrome;
- coloured according to printed instructions;
- selectively coloured;
- coloured by a later owner;
- colour retouched or faded;
- colour applied inconsistently with the printed code.

The 1605 wording about a purchaser having the work illuminated is particularly useful because it explicitly bridges the two layers without making them identical.

## VII. Relation to plate-stock ecology

The colour problem further qualifies `same_plate_as`. Even if two impressions can eventually be demonstrated to derive from the same copper matrix, their informational states may differ because:

1. the matrix itself may have been altered later to add letters or other coding;
2. one edition may supply separate prose that another omits;
3. copy finishing may add pigment;
4. later trimming can remove peripheral keys or letters;
5. wear can make small engraved letters increasingly difficult to read;
6. re-engraving can preserve composition while changing the coding system.

Accordingly, matrix continuity and information continuity are separate empirical questions.

## VIII. Evidence guards

1. **1605:** the colour `Declaration` and its illumination purpose are institutionally controlled; do not yet infer the precise page architecture without directly inspecting the image.
2. **1609:** use the *Archivum Heraldicum* statement as a scholarly secondary control for lower-case letter coding. Do not claim a particular plate's exact letters until the 1609 image is checked.
3. Claims that the 1612/second issue retrospectively added letters to all first-part plates are plausible and widely repeated, but remain a separate edition-state question requiring direct or high-grade bibliographical confirmation.
4. **1680 Spener:** direct primary text securely states the contrast between German initial-letter practice and his French dot/line convention, plus prose fallback at small scale.
5. **1772:** the criticism of letters is a publisher-side retrospective historical judgment, not proof that all users misunderstood every letter-coded armorial.
6. Do not write a universal evolutionary sequence from verbal description to letters to hatching. Different systems overlapped, and copy finishing adds another layer entirely.
7. Do not call hand colouring automatically `original colour`. Date, hand and relation to printed codes require copy-level evidence.

## Sources / locators

### 1605 Siebmacher
HAB / LibReTo, reconstructed Gandersheim library record, with VD17 control and ONB digital carrier. The record preserves the extended title/Declaration including the phrase explaining that an `emptor` could have the work `illuminiren und erhöhen`:

`http://data.onb.ac.at/ABO/%2BZ22135990X`

Institutional record surfaced at HAB's Gandersheim reconstruction and LibReTo.

### 1609 Siebmacher
Universitätsbibliothek Heidelberg HEIDI record: *New Wapenbuch*, part 2, Nürnberg 1609, `[5] Bl., 164 Bl. Abb., [8] Bl.`, shelfmark `B 721 RES::2`.

Secondary technical control: *Archivum Heraldicum* 2019, p. 115: the 1609 second part uses lower-case tincture letters, with `g`, `b`, `w` given as examples; note 10 cites Gert Oswald, *Lexikon der Heraldik* (1984), p. 353.

### 1680 Spener
Philipp Jakob Spener, *Historia insignium illustrium sive Operis heraldici pars specialis*, 1680; CAMENA transcription of the preface in the 1717 second-edition carrier, lines/images `as011`, especially sections VII:

`https://mateo.uni-mannheim.de/camenaref/spener/spener2/books/spener2_front.html`

Key text begins `Ceterum sculptae sunt Gallico more punctulis aut lineolis...` and continues with the explicit contrast to German `literis initialibus colorum`, followed by the small-figure prose fallback.

### 1772 publisher retrospective
UB Tübingen OpenDigi `Fe 18-1`, title-state 1772 `Vorbericht`, 2r–3v; repository analysis:

`docs/PUBLISHER_RETROSPECTIVE_KOHLER_1723_VISUAL_INFORMATION_PROBLEM_1772_2026-08-26.md`.

## Next discriminators

1. Directly inspect one 1609 Siebmacher plate at high resolution and record the exact letter code, placement relative to shield/charges and whether the same letter can be visually confused at plate scale.
2. Compare an early 1605 first-part plate, its separate colour description and the same plate/state after letters were reportedly added in a later issue. This would give a rare **same-design / altered-information-channel** test.
3. Trace when dot/line hatching enters the Fürst–Helmers–Weigel Siebmacher lineage. Do not rely on the often-repeated claim that 1705 was the first such state until a primary or strong bibliographical control is obtained.
4. Compare a coloured surviving copy against the engraved letters/hatching. Record whether pigment follows the code exactly; any discrepancy would expose the distinction between encoded information and copy finishing.
5. Re-read Köhler's 1734 preface for an explicit history of colour notation. A direct reference to Spener or to letter-vs-hatching systems would create a textual bridge; absent that evidence, keep the 1605/1609–1680–1772 chain as a technical comparison rather than a demonstrated line of influence.