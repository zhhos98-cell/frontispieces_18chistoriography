# Research log — 2026-08-27

Rolling log for the Wilson-informed colour-method web sweeps. This file records search closures, unresolved items, methodological changes, and repo write-backs as work proceeds.

## 08:02 UTC — Sweep 1 written

Commit: `5ed4f252b450c80cc7c34aee4193391b534f36b3`

File:
- `docs/COLOUR_METHOD_WILSON_WEB_SWEEP_LEGIBILITY_MATERIAL_CONSTRAINT_AND_EVIDENCE_REGIMES_2026-08-27.md`

Main change:
- replaced a downstream colour-only chain with six gates: `availability → selection → discretisation → observer formation → operation → inference jurisdiction`;
- added modern surrogate / digitisation mirror;
- added observer-training and material-constraint fields;
- treated colour as a methodological probe rather than merely a historical variable.

Key controls located:
- early colour printing can be materially present yet historiographically absent because descriptive vocabulary, disciplinary selection and digitisation suppress visibility;
- reused frisket waste can both obscure original function and later become the only surviving evidence for workshop practice;
- Werner treats colour as an early sensory character but excludes some visible differences from classificatory relevance;
- Syme's finite colour standard trains the observer rather than exhaustively representing all possible shades;
- Gatterer's graphical/tabular methods can function as comparison or measurement instruments;
- human colour provides a stress test separating description, discretisation, classification and genealogical/causal inference.

## 08:13 UTC — Sweep 2 written

Commit: `53da6d5ac7741406c061c612b7dbe4883acdf267`

File:
- `docs/COLOUR_METHOD_PRANGE_GOTTINGEN_APPARATUS_AVAILABILITY_ADOPTION_AND_TASK_COMPRESSION_2026-08-27.md`

Main closures:
- Christian Friedrich Prange's *Farbenlexicon* (1782) supplied 4,608 material colour samples and a chart/number workflow before Meiners's 1792 colour essay;
- Göttingen's Johann Beckmann reviewed Prange and explicitly separated the usefulness of colour standardisation from the material reproducibility of the standard;
- Widenmann's later mineralogical adaptation showed that `more granular standard ≠ more usable standard`; task-specific compression can be epistemically productive;
- Friedrich August Walter 1796 used Prange colour references for 157 urinary calculi, demonstrating actual adoption of a colour-number apparatus on human pathological material;
- current interpretation: the contrast with Meiners cannot be explained by simple technical unavailability.

Unresolved after sweep 2:
- whether Meiners personally owned, consulted, knew or rejected Prange/Lambert/Schäffer;
- direct page-level closure of Meiners 1792, pp. 611–672;
- direct page-image closure of selected Gatterer/heraldry material.

## 08:xx UTC — Sweep 3: comparability regimes

Commit: `8891f6e68ddf62abafaef34fdc4a5c5e0d6b3e31`

File:
- `docs/COLOUR_METHOD_COMPARABILITY_REGIMES_EVIDENCE_TEMPORALITY_AND_OBSERVER_CALIBRATION_2026-08-27.md`

Main methodological revision:
- standardisation is only one technology for producing comparability;
- comparison should be preceded analytically by the historical production of `comparability`;
- four provisional regimes distinguished:
  1. Prange — object-reference calibration by material swatch;
  2. Meiners — population comparability by accredited / aggregated witness testimony;
  3. Forster — observer calibration and perspectival correction;
  4. Blumenbach — autopsy, provenance, persistent specimens and cross-material comparison.

New fields / concepts:
- `comparability_regime`
- `calibration_target`
- `evidence_temporality`
- `capture_protocol`
- `material_persistence`
- `retrostandardisability`
- `standardisation_entry_point`
- `observer_network_requirement`
- `domain_source_status`
- `inference_ceiling`

Primary / near-primary closures added:
- Blumenbach 1790 reproduces Meiners's requirement that reliable observers of human populations should have long-duration, large-N exposure and distinguish individual variation from recurrent traits; Blumenbach explicitly agrees that concordant reliable testimony may be more informative than one or a few skulls of uncertain provenance;
- this supports treating witness accreditation as an evidentiary protocol rather than an accidental substitute for direct observation;
- Forster's travel-writing methodology treats observer characteristics/perspective as metadata required before using reports, supporting `observer calibration` as a distinct comparability technology;
- Blumenbach combines autopsy, provenance, specimens, images and reliable testimony and limits some inferences even where direct physical evidence is available;
- hair collection practice provides a material control: detachable hair can survive, circulate and be re-compared; living skin colour often collapses into legacy description once the observed person is absent.

Göttingen domain control:
- Gatterer's diplomatics used extensive original-charter / seal / script material as an object-intensive teaching and comparison apparatus;
- recent collection history reports that Gatterer, Schlözer and Meiners did not correspondingly treat ethnographica as research sources in universal history / Völkerkunde, while Blumenbach and later Heeren have clearer object-use traces;
- implication: `object locally available ≠ object authorised as source`;
- PDF text-layer passage located; page-image verification remains pending and is explicitly not upgraded beyond text-layer verification.

## Current active closure — Meiners 1792, pp. 611–672

Target:
- Christoph Meiners, “Ueber die Farben, und Schattierungen verschiedener Völker,” *Neues Göttingisches historisches Magazin* I/4 (1792), pp. 611–672.

Current status:
- article identity and pagination controlled;
- Bielefeld digital object identifier / viewer route located (`1923581_001`), but direct page-image/API retrieval remains unstable in the current web session;
- Krünitz's near-contemporary encyclopaedic article explicitly marks a section as derived `nach Hrn. Hofr. Meiners` and preserves the sequence of research questions, but is being treated only as a derivative witness, not as a substitute for the 1792 original;
- prior repo sweep already records secondary controls for Meiners pp. 614–15 (environmental modification of colour) and the opening research questions;
- no claim about the full argumentative sequence of pp. 611–672 will be upgraded to `primary_direct` until the original text/page images are recovered.

Coding goal once original is recovered:
for each claim or paragraph, record:
- `evidence_carrier`: personal observation / named traveller / anonymous report / inherited textual authority / specimen / comparison / speculation;
- `capture_time_relation`;
- `observer_metadata_present`;
- `population_aggregation_logic`;
- `colour_discretisation`;
- `causal_target`: climate / descent / mixture / other;
- `inference_target`: description / population classification / genealogy / hierarchy / causation;
- `inference_ceiling`;
- `retrostandardisability`.

## Archival leads still open

1. Meiners posthumous library sale catalogue (1810): inspect for Prange / Lambert / Schäffer / colour-nomenclature works. Do not infer absence from web-search silence.
2. Meiners → Johann Beckmann, 1788, SUB Göttingen, `Cod. Ms. Beckmann 6:8`, between pp. 520/521: existence/location controlled; content not yet recovered; no claim of colour transfer.
3. Meiners → Lavater correspondence, 1782–1788: e-manuscripta holdings with transcription indicated; inspect for complexion, physiognomy, observer reliability, comparative method.
4. Gatterer diplomatics / ethnographica contrast: obtain direct page-image control for recent collection-history passage and primary Gatterer teaching evidence.
5. Blumenbach teaching / collection use: reconstruct exact chronology of hair, skull, portrait/image, ethnographic object and witness-report use.

## Current stop rules

- Do not infer `personally known` from local Göttingen availability.
- Do not infer `adopted` from `reviewed`.
- Do not infer `source` from `collection object`.
- Do not infer exact historic colour from a legacy verbal adjective.
- Do not infer broader genealogical/causal warrant from improved descriptive precision.
- Do not treat near-contemporary derivative witnesses as equivalent to the original 1792 article.
- Log all unresolved retrieval failures instead of silently converting them into negative evidence.

## 08:46 UTC — Temporary closure before next research round

Status: **temporarily closed; no further inferential upgrades until the next sweep.**

Additional closure from Library re-check:
- Araújo's 2012 study directly juxtaposes Meiners's 1785 and 1793 formulations on human colour. In 1785, Meiners gives causal priority to climate and only secondarily to descent; in 1793, the order is reversed, with parental blood first and climate second. This is now treated as a controlled temporal change, not a retrospective summary.
- The 1792 colour essay therefore sits at a potentially decisive transition point between an environment-first and heredity-first causal architecture. This makes direct recovery of pp. 611–672 especially important.
- Araújo's reconstruction also confirms that Meiners's history of humanity is explicitly comparative and world-encompassing, and that his evidentiary practice is heavily text- and report-mediated rather than reducible to direct specimen inspection.
- A separate 1788 Meiners argument already claims that relocation to milder climates does not alter certain national/natural traits; this supplies a pre-1792 bridge toward increased causal weight for inherited constitution, but does **not** by itself establish the exact argument of the 1792 colour essay.
- Araújo further notes that the 1793 second edition added 188 titles, 115 of them published after 1785, and that Meiners himself highlighted additions from newer travel literature. This strengthens the model in which causal revision may be driven through a changing witness/report corpus rather than through adoption of a colour-standard apparatus.
- Blumenbach's 1790 response remains an important control: he accepts the need for broad, reliable eyewitness testimony while rejecting overextended inference from isolated bodily parts to moral/mental disposition. The issue is therefore not direct observation versus testimony in a simple binary, but competing evidence hierarchies and inference ceilings.

Unresolved at closure:
- direct primary-text reconstruction of Meiners 1792 pp. 611–672;
- whether the 1792 essay itself explicitly performs the causal-priority shift later visible in 1793;
- Meiners's personal access to / ownership of Prange, Lambert, Schäffer or related colour standards;
- contents of the 1788 Meiners–Beckmann letter;
- direct page-image verification for the Gatterer / ethnographica negative-side control.

Resume point for next round:
1. recover the 1792 primary text or a trustworthy page-level surrogate;
2. code its evidence carriers and causal targets paragraph-by-paragraph;
3. compare the 1785 → 1792 → 1793 sequence;
4. only then decide whether the key transition is best described as `causal reprioritisation`, `evidence-regime change`, `observer-network change`, or some combination.

## 08:50 UTC — New round restarted: stronger primary routes and correspondence controls

New primary-access routes:
- Deutsche Digitale Bibliothek now exposes the Bayerische Staatsbibliothek copy of *Neues göttingisches historisches Magazin*, vol. 1 (1792), shelfmark `H.misc. 201-1`, URN `urn:nbn:de:bvb:12-bsb10738733-5`. This provides an independent institutional route beyond the unstable Bielefeld viewer.
- Google Books independently exposes a full-view copy of volume 1 (1792). Its indexed common terms include `Farbe`, `Ursachen`, `Neger`, `Mulatten`, `rothe`, `schwarzen`, `weissen`, etc., confirming that the target colour essay is in the indexed volume; however, page-level visual verification has not yet been recovered through the current tool path.
- The BSB/DDB route is therefore upgraded to `primary volume located`, not yet `target pages visually verified`.

Meiners posthumous library catalogue:
- Blumenbach Online supplies a direct digitisation link for *Verzeichniß von nachgelassenen Büchern des Herrn Hofrath Meiners* (Göttingen: J. C. Baier, 1810), and the underlying PDF URL has been resolved as `https://blumenbach-online.de/PDF-Dateien/ChrMeiners_Verzeichnis_Nachlass_1810.pdf`.
- Current fetch attempts return a cache miss, so the catalogue has **not** yet been searched internally for Prange / Lambert / Schäffer / colour works.
- Status remains: `catalogue digital object resolved; ownership test pending`.

Lavater–Meiners correspondence:
- Zentralbibliothek Zürich / e-manuscripta explicitly holds seven letters from Johann Caspar Lavater to Christoph Meiners, dated 1784–1798, shelfmarks `FA Lav Ms 574.12–18`, DOI `10.7891/e-manuscripta-83497`; the record exposes a IIIF manifest and a downloadable 5.94 MB file.
- A separate 23 July 1788 billet from Lavater to Christoph Meiners and Ludwig Timotheus Spittler is catalogued as `FA Lav Ms 589a.79`, DOI `10.7891/e-manuscripta-64233`.
- This replaces the earlier vague lead of “Meiners → Lavater correspondence, 1782–1788” with a controlled holding on the reverse direction (Lavater → Meiners) plus a joint Lavater → Meiners/Spittler item. Contents still require inspection before any claim about physiognomy, colour or observer calibration.

1792 derivative/quotation controls strengthened:
- Krünitz's *Oekonomisch-technologische Encyclopädie*, entry `Leibes-Farbe der Menschen`, explicitly attributes its account to Meiners's 1792 essay and preserves the opening research programme: causal partition between climate and descent/parental blood; whether colour is a reliable sign of race/descent; number of principal colours; and whether some should be treated as ground-colours.
- Secondary quotation controls identify specific Meiners pages 614–15 (environmental effects), 640–41 (mixture / generational lightening logic) and 672 (late-stage conclusion), but these remain secondary page controls until checked against the primary scan.

Next actions:
1. recover BSB/Google page-level access for pp. 611–672;
2. use exact quoted strings to reconstruct the internal argumentative sequence while keeping quotation controls distinct from primary verification;
3. retry the 1810 auction PDF through alternate mirrors/catalogue portals;
4. inspect the Lavater letters for terms related to physiognomy, complexion, observation, witness reliability and comparison.

## 08:58 UTC — Meiners 1792 derivative witness now supports causal reprioritisation

Evidence status: **near-contemporary derivative witness (Krünitz), not yet primary-direct.** Direct e-rara PDF open again failed in the web parser after the indexed text was recovered; therefore these findings are not upgraded beyond derivative/text-layer control.

New high-value closures from the Krünitz `Leibes-Farbe` entry, explicitly marked as following Meiners's 1792 essay:
- p. 675 preserves a formulation that human colour depends *most* on parental blood. This places the 1785 → 1793 causal-priority reversal at or before the 1792 essay: by this derivative witness, parental descent is already ranked above climate in 1792.
- The same discussion nonetheless allows colour to change through disease, wounds, emotions, age and other internal physiological causes. Thus stronger heredity does not mean fixity.
- p. 665 uses geographical relocation and same-origin comparison to isolate external causes: extreme heat need not darken skin uniformly, while moist/softening/bleaching air, sea winds and local conditions can counteract solar heat. External environment remains a genuine causal channel.
- p. 685 treats Asian colour variation as jointly generated by external causes acting on transplanted populations and by mixture among peoples of unequal origin; it explicitly describes numerous shades merging into one another.
- p. 690 derives black colour on parts of the Indian peninsula from an alleged transformation of an earlier yellow/yellow-brown/greenish colour under coastal conditions.
- p. 695 states with unusual clarity that colour differences may arise partly from soil/climate and partly from mixture with foreign blood; travel accounts and linguistic affiliation are used alongside colour in ancestry arguments.
- pp. 705–706 supply a direct control on causal underdetermination. Light/white skin accompanied by features such as blond hair, blue eyes and other associated traits can be interpreted as evidence of European/Norman ancestry; elsewhere light colour in Guiana/Paraguay can be explained without European admixture by local climatic bleaching. The same visible outcome therefore does not carry one causal meaning.
- p. 710 begins `VIII. Ueber die Haupt-Farben und Ur-Farben der Menschen`: four Hauptfarben are white, yellow, red and black, but only white and yellow are treated as Urfarben. Red and black are derived as transformations of yellow under different physical conditions. The genealogical/original-colour architecture therefore coexists with environmental transformability.

Interpretive upgrade:
- the 1785 → 1792 → 1793 transition is best provisionally described as **causal reprioritisation within a plural causal model**, not replacement of climate by heredity;
- `parental blood` becomes the dominant/origin-level cause, while climate, migration/local environment, internal physiology and mixture remain modifier or transformation channels;
- colour is therefore causally underdetermined: `same visible colour ≠ same causal route`;
- genealogical use of colour requires triangulation with associated bodily traits, geography/provenance, witness reports, language and mixture narratives;
- this supplies a stronger formulation of `inference jurisdiction`: colour alone does not automatically authorise ancestry inference even inside Meiners's own racialising framework.

Proposed new coding fields:
- `causal_rank`
- `causal_partition`
- `modifier_vs_origin_cause`
- `cause_identifiability`
- `phenotypic_equifinality`
- `triangulation_requirement`
- `genealogical_threshold`
- `causal_underdetermination`

Provisional operational chain:
`colour observation × associated traits × geography/provenance × witness report × comparison → causal attribution → genealogical/classificatory inference`

This replaces the too-simple model `colour → ancestry`.

## 09:06 UTC — Trait decoupling / differential persistence added

Evidence status: **near-contemporary derivative witness (Krünitz), original p.679 still pending direct scan verification.**

New closure:
- the Krünitz reconstruction preserves a Meiners argument in which repeated unions between Europeans or their descendants and Black women can progressively darken descendants until the third/fourth generation becomes black or blackish, while bodily formation—especially facial form—is still described as European or at least more European than `Neger-artig`;
- the same genealogical line can therefore carry traits that change at different rates: `colour change rate ≠ morphology change rate`;
- phenotype cannot be treated as a single integrated marker even within Meiners's own argument. Colour, facial/body form, hair and other traits require separate temporal and causal coding.

Interpretive upgrade:
- add **trait decoupling** to **phenotypic equifinality**. Equifinality concerns one outcome produced by several causes; trait decoupling concerns several traits within one body/lineage following different causal-temporal trajectories;
- genealogical inference becomes a weighted cross-trait operation rather than accumulation of equivalent corroborating signs;
- proposed formula: `genealogical signal = weighted bundle of partially decoupled traits + provenance/history`;
- new fields: `trait_decoupling`, `trait_persistence_rate`, `trait_temporality`, `cross_trait_concordance`, `trait_specific_inference_weight`, `trait_specific_causal_susceptibility`, `cross_trait_weighting`.

Repo write-back:
- methodology file updated in commit `a9431f4521cf6397b45bc3e1aecdab50ee735f57`:
  `docs/MEINERS_1792_COLOUR_CAUSAL_REPRIORITISATION_EQUIFINALITY_AND_INFERENCE_JURISDICTION_2026-08-27.md`

Next comparative test:
- determine whether this separation of skin colour, facial/body form and hair is specific to Meiners or part of a broader late-Enlightenment physical-geography / anthropology evidentiary grammar.
