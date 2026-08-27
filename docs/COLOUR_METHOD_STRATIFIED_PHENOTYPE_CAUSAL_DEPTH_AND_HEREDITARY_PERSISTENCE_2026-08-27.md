# Colour method: stratified phenotype, causal depth, and hereditary persistence

Date: 2026-08-27

## 1. Why `distributed phenotype` is not yet enough

The Meiners 1792 sweep first required a `distributed phenotype` model because colour, facial/body form, hair and other visible characters can fail to move together within one asserted lineage. One trait may change while another remains genealogically persistent.

Comparative controls now show that this is not merely an isolated Meiners maneuver. The stronger historical structure is a **stratified phenotype**: eighteenth-century actors could assign different bodily characters different causal depth, response time and hereditary persistence.

The core distinction is:

`trait disagreement` = distributed phenotype

`trait disagreement + historically differentiated causal depth/time` = stratified phenotype

This matters because not every visible difference is granted equal evidentiary status even when every difference is equally visible.

## 2. Buffon 1766: an actor's causal stratification

Buffon's *De la dégénération des animaux* (1766) provides the clearest upstream control currently located. In his own causal grammar, skin, hair and eye colour belong among changes more readily produced by climate and exterior conditions. Stature, facial form and aspects of hair quality/form require additional causes, including food and land, and longer duration. Air/sky acts comparatively superficially; nourishment penetrates more deeply into bodily formation. Over sufficiently extended time, changes can become perpetuated by generation and stabilize as characters.

The important point is methodological rather than retrospective biological validity. Buffon supplies an eighteenth-century model in which bodily characters differ along at least three axes:

1. **causal depth** — how deeply the cause is imagined to act on bodily organization;
2. **response time** — how quickly the character can change under altered conditions;
3. **hereditary persistence** — whether and when the altered character becomes stable across generation.

Thus:

`visibility ≠ equal causal depth ≠ equal historical persistence ≠ equal genealogical weight`.

## 3. Wilson and historical surface/depth

Wilson's method is useful precisely because it prevents a modern materialist shortcut in which the scholar assumes that a visible `surface` conceals a truer causal `depth` underneath. In this project, surface/depth should therefore not be used as an unmarked modern ontology.

Buffon changes the situation. Here a historical actor himself explicitly differentiates more superficial effects from more internal/formative effects. That allows `surface/depth` to enter the analysis as an **object of historical reconstruction**, not as the historian's explanatory premise.

Coding rule:

- if surface/depth language or equivalent causal stratification is actor-explicit, record `actor_causal_depth = explicit`;
- if inferred only from different temporal behavior of traits, record `actor_causal_depth = reconstructed`;
- never infer that the historically `deeper` trait was epistemically more valid unless the source itself assigns it greater evidentiary weight.

## 4. Kant lecture culture: the inheritance-conversion problem

The BBAW transcript of the Herder notes from Kant's 1763–64 physical-geography lectures already juxtaposes:
- acquired/postnatal colour change;
- illness or injury producing white skin;
- alleged long-term climatic effects;
- Black–White admixture sequences;
- white children of Black parents with distinctive hair/eyes;
- the explicit problem of how a colour attributed to air/sun could become hereditary.

This identifies an earlier **inheritance-conversion problem**:

`environmentally/acquired visible change → ? → stable inherited character`.

The question is not merely what causes colour. It is what temporal or reproductive process converts a contingent modification into a genealogically persistent sign.

Later Kant physical-geography strata make the distributed phenotype still more explicit by juxtaposing colour, `Gestalt`, hair and descent. Because the Barth manuscript is composite and Rink's edition dates to 1802, those later formulations must be version-controlled rather than backdated wholesale to the 1760s.

## 5. Meiners 1792: causal reprioritisation inside a stratified field

Meiners's colour argument can now be read more precisely. The current near-contemporary derivative reconstruction indicates that parental blood receives the highest default causal rank by 1792, while climate, local environment, mixture and internal physiology remain genuine causal channels. The admixture example in which colour darkens more quickly than facial/body form shows differential persistence among traits.

This yields:

`descent/default cause × environmental modifiers × admixture × physiological modifiers → trait-specific trajectories`

rather than a single phenotype changing as one unit.

A genealogical inference therefore operates on a weighted bundle:

`genealogical signal = Σ(trait × persistence × causal susceptibility × provenance) + historical reports`

This formula is analytical, not Meiners's mathematical language. It makes explicit what needs to be coded in the historical operation.

## 6. Zimmermann 1778: geographical causal partition

Zimmermann's *Geographische Geschichte des Menschen* supplies a pre-1792 natural-historical geography in which migration, reproduction and climate are joined into a history of human variation. Recent scholarship quotes p.115 as describing populations gradually adapting as humanity moved through different climates. Blumenbach's own colour discussion cites Zimmermann pp.94ff. in the debate over causes of human skin colour.

Zimmermann is therefore an important bridge between:
- bodily variation;
- geographical relocation;
- temporal persistence;
- natural-historical explanation.

Until pp.94–115 are directly recovered, however, the exact structure of his causal ranking remains unresolved.

## 7. Meiners's anti-single-trait rule

A recent critical volume quotes Meiners's *Grundriß der Geschichte der Menschheit*, p.23, stating that whole peoples and individuals cannot be judged from the formation of a single bodily part, nor can the characteristic formation of one part across a nation be inferred from isolated bones.

Once primary-direct verification is obtained, this should be treated as a general methodological rule:

`single trait / single specimen → insufficient population warrant`.

This does not make Meiners's resulting racial or hierarchical claims methodologically sound. It identifies the evidentiary threshold he says must be crossed before collective inference is authorised.

## 8. Downstream Girtanner/Blumenbach formalization

Girtanner's 1796 *Über das Kantische Princip für die Naturgeschichte* and Blumenbach's 1797 revision provide a later control on the conversion of variable character into `Rasse`. In Blumenbach's formulation, following the Kantian distinction and referring readers to Girtanner, a racial character is one produced through degeneration that necessarily reproduces through generation; a mere `Spielart` lacks that reproductive necessity.

This supplies a downstream formal criterion:

`visible difference + necessary reproductive persistence → race-status`

rather than:

`visible difference → race-status`.

This should not be projected backward into Meiners 1792 without direct evidence, but it clarifies the broader problem-space in which persistence itself becomes an evidentiary operation.

## 9. New coding architecture

### Trait layer
- `trait_type`
- `trait_visibility`
- `distributed_phenotype`
- `cross_trait_concordance`
- `trait_decoupling`

### Causal-depth layer
- `trait_causal_depth`
- `actor_causal_depth = explicit / reconstructed / absent`
- `surface_change_vs_structural_change`
- `trait_specific_causal_susceptibility`

### Temporal layer
- `trait_response_time`
- `trait_temporality`
- `trait_hereditary_persistence`
- `inheritance_conversion_problem`
- `stabilisation_timescale`

### Inference layer
- `trait_specific_inference_weight`
- `cross_trait_weighting`
- `cross_trait_conflict_resolution`
- `trait_origin_status`
- `genealogical_threshold`
- `population_warrant`
- `inference_ceiling`

## 10. Methodological questions

For any historical use of colour or other bodily difference, ask:

1. Is the trait merely visible, or is it assigned causal depth?
2. How quickly is it thought capable of changing?
3. Can an acquired modification become inherited, and by what mechanism or timescale?
4. Which traits are allowed to disagree within one body or lineage?
5. When traits disagree, which one preserves genealogical authority?
6. Does persistence across generation change the category from `variation` to `race`, `stock`, `descent`, or another historical classification?
7. What evidence establishes persistence: direct generations, travel reports, analogy with animals, migration histories, specimens, or theoretical postulate?
8. Is the scholar observing the trait itself, or a legacy description whose original observation cannot be retro-standardised?

## 11. Strong current thesis

> Late-Enlightenment colour classification cannot be reconstructed adequately as a taxonomy of visible shades. In a significant natural-historical and anthropological strand, visible bodily characters were distributed across a stratified causal-temporal architecture: some were treated as rapidly responsive and comparatively superficial, others as slower and more deeply formative, and still others as evidentially decisive only once their persistence through generation was established. Colour therefore operated not simply as a category but as a test of how contingent appearance could—or could not—be converted into durable historical descent.

The Wilson-informed question can now be sharpened again:

> **How does a visible difference acquire temporal depth sufficient to become historical evidence?**

and, where several traits disagree:

> **Which difference is authorised to remember descent when another has already changed?**

## 12. Pending closure

- direct Zimmermann 1778 pp.94–115;
- primary Meiners *Grundriß* p.23;
- exact Girtanner 1796 passages on colour/form/hair and reproductive necessity;
- direct Meiners 1792 pp.611–672 scan;
- version-level reconstruction of when Kant's more explicit `Gestalt + Farbe + Haar` formulation enters the lecture tradition;
- test whether Buffon's causal depth vocabulary is explicitly cited or merely structurally paralleled in Zimmermann, Kant, Blumenbach or Meiners.
