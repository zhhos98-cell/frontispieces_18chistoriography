# Colour-method extension ontology

Version: 0.1  
Opened: 2026-08-27

This is an **extension ontology**. It does not reopen or alter the frozen core identity hierarchy in `schema/ONTOLOGY.md`.

## 1. Governing distinction

`colour` is not one property.

The corpus must distinguish at least:

`observed/material colour`
≠ `semantic colour category`
≠ `graphic encoding of colour`
≠ `decoder/key for colour`
≠ `applied pigment on a copy`
≠ `arbitrary colour used as relational syntax`
≠ `colour used as a classificatory variable`.

The same printed object can instantiate several of these at once.

## 2. Core colour entities

### `colour_observation`
A source-backed observation that a physical or represented object has, is said to have, or is classified by a colour/hue.

Examples:
- a hand-coloured shield field;
- a human body's `Farbe` in a geographical/ethnographic classification;
- a natural specimen compared with a colour sample.

### `colour_category`
A semantic category such as `Gold`, `Silber`, `Roth`, `Blau`, `Schwarz`, `Grün`, `Purpur`, `Naturfarbe`, or a named historical colour term. A category is not identical to one physical pigment or visual sample.

### `colour_encoding`
A non-pigment or reduced-pigment sign that communicates colour information.

Encoding modes include:
- `letter_code`;
- `dot_code`;
- `hatching_vertical`;
- `hatching_horizontal`;
- `hatching_diagonal`;
- `cross_hatching`;
- `blank_field`;
- `verbal_name`;
- `numeric_code`;
- `mixed`.

### `colour_key`
A legend, declaration, table, prose section or other decoder connecting a colour encoding to colour categories and/or names.

Example:

`vertical hatching ↔ de Gueules ↔ Roth`.

A colour key may be entirely monochrome. It therefore conveys chromatic information without being a chart of physical colour samples.

### `colour_application`
The application of pigment to one physical impression/copy.

Possible states:
- `uncoloured`;
- `partially_coloured`;
- `fully_coloured`;
- `contemporary_colour_probable`;
- `later_colour_probable`;
- `retouched`;
- `faded`;
- `colouring_date_unresolved`.

Colour application is an impression/copy property unless evidence shows otherwise.

### `colour_operation`
The epistemic or practical work colour performs in a specific context.

Recommended values:
- `discriminate` — make adjacent units visibly different;
- `classify` — assign an object/person/territory to a category;
- `compare` — support similarity/difference judgments;
- `decode` — recover semantic colour information from a sign;
- `reconstruct` — enable a reader/colourist to recreate an absent colour state;
- `standardise` — stabilize names, samples or recipes across users;
- `verify` — check a representation against a source/object/code;
- `compress` — carry information in less visual/textual space;
- `navigate` — orient the reader through a complex information field;
- `memorise` — increase rapid recognition/retention;
- `mark_relation` — represent a relation not itself chromatic;
- `mark_change` — highlight transition, rupture or historical revolution;
- `mark_boundary` — distinguish spatial/political/cultural limits;
- `signal_status` — assign a hierarchical/systemic role;
- `finish_copy` — materially complete or enhance an impression.

### `colour_claim`
An assertion about what a colour, code, sample or pigment means or does. It must carry evidence basis and claim scope like any other canonical assertion.

### `colour_failure`
A source-backed or analytically bounded failure mode in colour transmission or use.

Recommended values:
- `scale_limit` — figure too small for code to remain discriminable;
- `symbol_ambiguity` — letters/hatching produce confusion;
- `missing_key` — decoder lost or absent from a copy;
- `missing_explanation` — explanatory channel removed across editions;
- `nonstandard_name` — names do not map stably across users/systems;
- `pigment_variance` — hand application varies among copies;
- `misapplication` — pigment conflicts with supplied code/source;
- `fading_or_change` — material colour no longer preserves initial appearance;
- `copy_divergence` — copies from the same matrix expose different colour information;
- `category_instability` — observed continuous/variable colour resists stable classification;
- `surrogate_loss` — monochrome or other reproduction suppresses chromatic information.

## 3. Colour roles

Every canonical colour record should specify `colour_role` rather than merely `colour_present`.

Recommended roles:

### `object_property`
Colour is treated as a property of the represented/observed object.

### `semantic_tincture`
Colour is a rule-governed heraldic category.

### `encoding_symbol`
A monochrome mark stands for a colour category.

### `decoder_key`
A key translates marks/categories/names.

### `copy_finish`
Pigment is physically applied to a particular impression.

### `fidelity_marker`
Colour is used or judged as part of faithful reproduction of an object/appearance.

### `classifier`
Colour is a variable for grouping or distinguishing objects, bodies, territories or other units.

### `relational_syntax`
Colour represents an abstract relation such as political dominance, competition, dependency, boundary or historical rupture rather than the literal colour of the referent.

This last role is crucial for Gatterer's synchronistic tables.

## 4. Referent versus carrier

Always separate:

- `colour_referent` — what the colour information is about;
- `colour_carrier` — where/how that information is physically encoded.

Examples:

1. Heraldic tincture:
   - referent: semantic tincture of shield field;
   - carrier: vertical hatching in a monochrome copperplate.

2. Hand-coloured armorial copy:
   - referent: semantic tincture of shield field;
   - carrier: applied pigment on one impression.

3. Gatterer synchronistic table:
   - referent: political relation/duration/revolution;
   - carrier: applied pigment on a historical table.

4. Menschen- und Völkerkunde:
   - referent: observed/classified human bodily colour;
   - carrier: verbal category, description, table or other classificatory notation.

## 5. Translation chains

Colour information often moves through several media. Record the chain rather than treating them as equivalent.

### Heraldic encoding chain

`claimed/known tincture`
→ `colour category/name`
→ `letter or hatch code`
→ `monochrome printed impression`
→ `colour key / prose blazon`
→ `reader reconstruction`
→ optional `hand colouring`.

### Natural-history fidelity chain

`observed object hue`
→ `named/sample colour`
→ `recipe/reference system`
→ `colourist's mixture`
→ `pigment on copy`
→ `comparison/evaluation`.

### Historical-table syntax chain

`historical relation/change`
→ `assigned colour category`
→ `pigment applied to diagram`
→ `rapid visual discrimination/overview`.

In this third chain the original referent has no literal colour. Colour is a notation system.

## 6. Two high-level regimes

### A. `de_pigmented_colour`
Colour information is made portable through words, letters, dots, hatching or keys while actual pigment is absent.

Advantages to test:
- reproducibility;
- compatibility with monochrome copperplate printing;
- lower cost;
- categorical clarity;
- cross-copy invariance.

Failure modes to test:
- ambiguity at small scale;
- missing legend/prose;
- learned-code dependence;
- loss of perceptual specificity.

### B. `re_pigmented_colour`
Pigment is materially applied to an impression/table/map/image.

Advantages to test:
- immediate discrimination;
- perceptual resemblance/fidelity;
- rapid overview;
- lower decoding burden.

Failure modes to test:
- copy variance;
- unstable recipes/names;
- hand-colouring error;
- fading/material change;
- higher production cost;
- uncertain edition-level invariance.

These regimes can coexist in one publication and should not be written as a simple historical succession.

## 7. Current corpus mapping

### Siebmacher 1605/1609
Colour information can be verbalized separately and/or embedded through letter codes; printed information can guide later hand illumination.

### Spener 1680
Dot/line hatching replaces German initial-letter practice for many figures, while prose remains necessary when scale defeats graphic discrimination.

### Weigel/Köhler Wappenkalender, 1728–1757
The recurring monochrome `Erklärung der Farben` acts as a centralized decoder linking hatching, heraldic categories and German/French names; prose blazon supplies another redundant channel.

### Köhler/Weigel retrospective, 1734/1747 and 1772
Loss of colour explanation and disorder generated by letter-coded tinctures become historically articulated failures of information architecture.

### Gatterer, `Synopsis historiae universalis`, 1766/1769
Pigment is applied by hand and varies by copy. Colour does not merely reproduce an object's appearance; it highlights historical boundaries/relations/revolutions in a synoptic diagram. This is `relational_syntax`.

### Gatterer, `Abriß der Geographie`, 1775
`Farbe` enters Menschen- und Völkerkunde as a classificatory variable of human bodies alongside shape. This is a distinct `classifier/object_property` regime and must not be collapsed into heraldic or tabular colour syntax.

## 8. Methodological question

The working question is not:

> How did eighteenth-century historians use colour?

It is:

> **Under what conditions could colour be made into a legitimate historical operation: encoded, decoded, reproduced, compared, standardized, abstracted, or rejected as unstable?**

A still stronger formulation is:

> **How was difference made operational through colour, and what happened when colour itself resisted the demands of reproducibility, comparison and evidentiary control?**

## 9. Relation to the Göttingen controversy

Colour should initially be treated as a **methodological discriminator**, not as an explicitly documented topic of the 1773 Gatterer–Schlözer polemic.

The existing dispute map establishes a contested economy of historical method and media: how universal history should be selected, synchronized, compressed and kept before the reader/student. The colour branch can test whether Gatterer's specific graphical implementations delegated part of that work to colour in ways not shared by Schlözer's programme.

A direct `colour controversy` claim requires primary evidence that either actor polemicized about colour, graphic tables, illumination or related media choices. Until then:

`Gatterer–Schlözer dispute`
+
`different media implementations`
→ `analytical comparison`, not a demonstrated polemic about colour.

## 10. Historiographical guard

Do not claim novelty for:
- eighteenth-century colour standardization as such;
- colour charts/reference systems as such;
- methodological problems of hand-colouring scientific illustrations;
- cognitive use of colour in Gatterer's `Synopsis` as such.

The stronger gap to test is the history of **colour translation regimes within historical methods**, especially the movement between monochrome semantic encoding, centralized decoding, copy-level pigment, arbitrary relational syntax and classificatory colour in the Nürnberg–Göttingen historical sciences.
