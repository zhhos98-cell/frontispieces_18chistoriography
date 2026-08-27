# Colour ontology addendum: inference target, discretisation and warrant gradient

Date: 2026-08-27
Status: active extension; candidate for later merge into `COLOUR_ONTOLOGY.md`

## 1. Why `epistemic_location` is not enough

The existing `epistemic_location` axis answers **where** a colour-bearing operation occurs in a knowledge chain. It does not by itself answer **what inference is being licensed from the same colour observation**.

The Gatterer human-colour case makes this distinction unavoidable. On the current secondary control through André de Melo Araújo (2012):

- Gatterer in 1771 treats outward human differences as `zufällige` rather than `wesentliche Unterscheidungszeichen` / `blose Varietäten`;
- in 1775 he nevertheless projects an `Anthropographia` / `Geographie der Menschenkörper nach Gestalt und Hautfarben` for descriptive differentiation;
- in 1789 language, rather than skin colour, is preferred as stronger evidence of the `Ursprung der Völker`; colour can persist where reliable linguistic information is unavailable.

Therefore the same visible property can be legitimate for one epistemic task and weak for another.

`visible difference`
≠
`essential difference`
≠
`genealogical difference`.

## 2. New recommended field: `inference_target`

Recommended controlled values:

- `descriptive_discrimination`
  - distinguishes visibly or verbally reported properties without necessarily claiming deeper structure.
- `taxonomic_partition`
  - assigns units to classes or groups.
- `relational_assignment`
  - marks a relation among already accepted units, e.g. synchronism, boundary, duration or political relation.
- `genealogical_origin`
  - infers common or distinct origin/descent.
- `causal_explanation`
  - treats colour as explanatory of another state or historical outcome.
- `essential_difference`
  - treats colour as indicating a constitutive rather than accidental difference.
- `source_identity_or_fidelity`
  - uses colour to identify or verify an object/source property.
- `reader_inspection`
  - changes perceptual access, navigation or salience without adding a historical inference.
- `memory_pedagogy`
  - supports retention/association of an already organized relation.

Multiple values are permitted only when the source or implementation genuinely supports multiple tasks.

## 3. New recommended field: `warrant_relative_to_target`

A single colour observation may have different warrant statuses by inference target.

Recommended values:

- `directly_warranted`
- `conventionally_warranted`
- `system_assigned`
- `comparatively_preferred`
- `fallback_under_data_scarcity`
- `insufficient_resolution`
- `causally_underdetermined`
- `insufficient_for_target`
- `rhetorically_suspect`
- `unresolved`

Suggested encoding pattern:

```json
{
  "colour_property": "Hautfarbe",
  "epistemic_location": "classification",
  "inference_targets": [
    {"target": "descriptive_discrimination", "warrant_relative_to_target": "directly_warranted"},
    {"target": "essential_difference", "warrant_relative_to_target": "insufficient_for_target"},
    {"target": "genealogical_origin", "warrant_relative_to_target": "fallback_under_data_scarcity"}
  ]
}
```

This example is a schema illustration based on the current Araújo control and must not be promoted to a direct-primary assertion until Gatterer 1771 pp. 61–62, 1775 pp. 4–5 and 1789 vol. 2 p. 606 are directly inspected.

## 4. A missing operator before classification: `colour_discretisation`

The Heeren control introduces a problem that precedes classification itself.

A visible chromatic field may be continuous or contain more gradations than a classificatory system can stably name. Before colour can function as a classifier, a method must decide how continuous variation is converted into finite categories.

Recommended analytical sequence:

`continuous visible variation`
→ `discretisation / binning / naming`
→ `colour category`
→ `classification`
→ `historical inference`.

Recommended entity/operation:

- `colour_discretisation`
- operations: `bin`, `name`, `standardise_boundary`, `collapse_nuance`, `retain_nuance`

Recommended failure modes:

- `measurement_granularity_limit`
- `category_precision_limit`
- `boundary_instability`
- `data_scarcity`

These are analytically distinct from an incorrect inference. A classification can fail before any causal or genealogical claim is made because the chromatic continuum itself has not been stably partitioned.

## 5. Heeren as the control for discretisation and causal underdetermination

Araújo's reconstruction of Heeren provides two separate controls, each with a different evidence status.

### 1817 lecture-note derivative: category precision

A surviving student transcript of Heeren's `Allgemeine Länder- und Völkerkunde` lecture in summer 1817, later excerpted by Christoph Becker-Schaum, reports Heeren refusing an exact classification of all peoples/types because there are too many colour nuances and they are insufficiently known. Only coarse `Hauptvölker`, identified by dominant colours, can be classified.

This belongs at:

- `epistemic_location = classification`
- `inference_target = taxonomic_partition`
- `warrant_relative_to_target = insufficient_resolution`
- failure: `measurement_granularity_limit; category_precision_limit; data_scarcity`

Evidence status must remain `primary_derivative / probable`: the surviving carrier is a lecture transcript, and the current control is through a later scholarly edition quoted by Araújo.

### 1826 witness: causal proof

Araújo quotes *Historische Werke*, vol. 15, pp. 5–7, where Heeren considers whether bodily organisation associated with skin-colour difference may affect the easier or harder development of mental capacities. He explicitly asks who can prove such influence and treats historical experience as capable of increasing probability without proving absolute incapacity or establishing colour-related bodily difference as the sole cause.

This belongs at:

- `inference_target = causal_explanation`
- `warrant_relative_to_target = causally_underdetermined`
- failure: `causal_underdetermination`

The 1826 witness is *Historische Werke*, vol. 15 = *Ideen über die Politik, den Verkehr und den Handel der vornehmsten Völker der alten Welt*, part III, `Europäische Völker`, first division, `Griechen`, fourth revised edition. The `Griechen` division is independently attested by 1812, but the textual ancestry of the pp. 5–7 passage has not yet been edition-controlled. Do not date the quoted formulation to 1793 merely because the larger *Ideen* project began publication in the 1790s.

## 6. Why this matters beyond bodily colour

The same distinction applies across the colour corpus.

### Schlözer 1772

`Facta färben` is suspect because the intervention operates at `fact_proposition`; the target is effectively the factual content itself.

### Schlözer 1773 / 1775

Painted co-presence and table illumination act downstream. Their targets are `relational_assignment`, `reader_inspection` and `memory_pedagogy`, not new factual propositions.

### Gatterer `Synopsis`

Assigned pigment appears to mark relations/boundaries among already selected historical units. Its target is not literal source colour but `relational_assignment`.

### Heraldry

Literal tincture, hatch code and decoder can have distinct targets: source/object fidelity, semantic classification and reproducible surrogate decoding. Heraldry also supplies an important contrast to human bodily colour: conventional tinctures are pre-discretised into a finite code-space, making stable naming and hatching possible.

### Human bodily colour

No such finite conventional code-space is given in advance. The method must first decide how many chromatic differences count, where category boundaries lie and whether those categories warrant any stronger historical inference.

Thus:

> **The legitimacy of colour is relative not merely to where colour enters, but to how visible variation is discretised and to what the observer is asked to infer from the resulting category.**

## 7. New failure pattern: `inference_overreach`

Recommended analytical failure:

`inference_overreach`

Definition:
A colour property or colour-coded relation is adequately warranted for a limited task but is made to support a stronger inference for which the evidence does not suffice.

Subtypes:

- `descriptive_to_taxonomic_overreach`
- `taxonomic_to_genealogical_overreach`
- `visible_to_essential_overreach`
- `classification_to_causal_overreach`
- `salience_to_importance_overreach`
- `display_to_evidentiary_overreach`

This is different from simple colour error. The colour can be perceptually correct while the inference is methodologically excessive.

## 8. Cross-domain methodological control

A useful controlled comparison is now available without asserting historical transfer:

### Heraldry

`finite conventional tincture set`
→ stable category names
→ hatch code
→ decoder
→ reproducible classification.

### Human bodily colour

`continuous/poorly measured chromatic variation`
→ contested discretisation
→ coarse or unstable categories
→ restricted classificatory and causal warrant.

The comparison asks how the **structure of the colour domain itself** constrains what methods can do with it.

This is not evidence that Gatterer or Heeren consciously transferred heraldic methods into anthropology.

## 9. Project-level formulation

The ontology now supports a more exact sequence of questions:

1. Is the colour difference observable?
2. Can it be discretised into stable categories?
3. Is the category useful for a stated classificatory task?
4. What stronger historical inference, if any, may be drawn from it?
5. Does graphical or chromatic display merely make that inference easier to see, or does it falsely increase its apparent warrant?

The strongest compact formulation remains:

> **When is a visible difference allowed to become a historical difference, and which historical inference may it legitimately carry?**

This supplements, rather than replaces:

> **What may colour do to history?**

## 10. Primary and derivative controls required before merge

1. Gatterer, *Einleitung in die synchronistische Universalhistorie* (1771), pp. 61–62: `wesentliche / zufällige Unterscheidungszeichen`, `Varietäten`.
2. Gatterer, *Abriß der Geographie* (1775), pp. 4–5: `Anthropographia`, `Gestalt`, `Hautfarben`.
3. Gatterer, *Kurzer Begriff der Geographie* (1789), vol. 2, p. 606: language, skin colour and origin-warrant.
4. Heeren lecture transcript, summer 1817, as edited in Becker-Schaum 1993, p. 311: colour nuances and limits of exact classification; if possible, inspect the underlying Gagern manuscript.
5. Heeren, *Historische Werke*, vol. 15 (1826), pp. 5–7: direct page control of the causal passage.
6. Compare 1826 `Griechen` pp. 5–7 against the 1812 and 1817 editions to date the formulation.
7. Compare with Meiners only with exact edition/page controls; do not import later racial taxonomy backward into Gatterer's terms.
