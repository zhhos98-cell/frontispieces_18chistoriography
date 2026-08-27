# Colour ontology addendum: inference target and warrant gradient

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

## 4. Why this matters beyond bodily colour

The same distinction applies across the colour corpus.

### Schlözer 1772

`Facta färben` is suspect because the intervention operates at `fact_proposition`; the target is effectively the factual content itself.

### Schlözer 1773 / 1775

Painted co-presence and table illumination act downstream. Their targets are `relational_assignment`, `reader_inspection` and `memory_pedagogy`, not new factual propositions.

### Gatterer `Synopsis`

Assigned pigment appears to mark relations/boundaries among already selected historical units. Its target is not literal source colour but `relational_assignment`.

### Heraldry

Literal tincture, hatch code and decoder can have distinct targets: source/object fidelity, semantic classification and reproducible surrogate decoding.

Thus:

> **The legitimacy of colour is relative not merely to where colour enters, but to what the observer is asked to infer from it.**

## 5. New failure pattern: `inference_overreach`

Recommended analytical failure:

`inference_overreach`

Definition:
A colour property or colour-coded relation is adequately warranted for a limited task but is made to support a stronger inference for which the evidence does not suffice.

Subtypes:

- `descriptive_to_taxonomic_overreach`
- `taxonomic_to_genealogical_overreach`
- `visible_to_essential_overreach`
- `salience_to_importance_overreach`
- `display_to_evidentiary_overreach`

This is different from simple colour error. The colour can be perceptually correct while the inference is methodologically excessive.

## 6. Project-level formulation

The new ontology supports a more exact question:

> **When is a visible difference allowed to become a historical difference, and which historical inference may it legitimately carry?**

This supplements, rather than replaces:

> **What may colour do to history?**

## 7. Primary controls required before merge

1. Gatterer, *Einleitung in die synchronistische Universalhistorie* (1771), pp. 61–62: `wesentliche / zufällige Unterscheidungszeichen`, `Varietäten`.
2. Gatterer, *Abriß der Geographie* (1775), pp. 4–5: `Anthropographia`, `Gestalt`, `Hautfarben`.
3. Gatterer, *Kurzer Begriff der Geographie* (1789), vol. 2, p. 606: language, skin colour, and origin-warrant.
4. Compare with Meiners only after Gatterer's own locations are direct-controlled; do not import later racial taxonomy backward into Gatterer's terms.
