# Colour method — Prange, Göttingen, and the gap between available apparatus and adopted apparatus

Date: 2026-08-27  
Status: Wilson-informed second web sweep  
Scope: 1769–1801 core; later references used only for bibliographic reconstruction

## 0. Research question

The first Wilson-informed sweep established that colour should be treated through six gates:

`availability → selection → discretisation → observer formation → operation → inference jurisdiction`.

The present sweep asks a more specific historical question raised by Christoph Meiners's 1792 essay on human colour:

> If eighteenth-century German scholars already possessed material colour-reference technologies, why did some domains adopt them while other domains continued to operate through verbal reports and looser colour categories?

This is not a question of simple technological availability. The evidence now supports a stronger distinction:

`available apparatus`
≠ `adopted apparatus`
≠ `usable apparatus`
≠ `authoritative apparatus`
≠ `legitimate inference`.

The key control is Christian Friedrich Prange's *Farbenlexicon* (1782), its reception in Göttingen, and its selective use in natural history and anatomy.

---

## 1. Prange 1782: a material colour-reference apparatus existed before Meiners 1792

Christian Friedrich Prange's *Farbenlexicon* (Halle, 1782) supplied a large-scale material colour-reference system intended explicitly for naturalists as well as painters, manufacturers, artists and craftspeople.

The work contained:

- 48 hand-coloured charts;
- 96 samples per chart;
- 4,608 numbered colour samples in total;
- a register connecting sample number, German colour name and pigment mixture/proportion;
- instructions for matching colours observed in nature to numbered samples.

Recent archival reconstruction by Giulia Simonini confirms that Prange's system was not merely a nomenclature. It was designed as a workflow:

`natural object`
→ `visual comparison with material swatches`
→ `chart + sample number recorded`
→ `portable notation`
→ `later recovery / colouring using the register`.

Prange's cheaper *Schule der Mahlerey* (1782) reduced this to 213 samples. A surviving copy of that reduced work is now held by the Niedersächsische Staats- und Universitätsbibliothek Göttingen (DD90 A 33229). Present-day holding location does **not** establish eighteenth-century acquisition or Meiners's access; provenance remains to be established.

### Method consequence

By 1782, the technical possibility of replacing an unstable verbal colour description with a material comparison + number code was demonstrably available in the German-speaking learned world.

Therefore:

> Meiners's 1792 dependence on travellers' colour words cannot be explained simply by the non-existence of colour standards.

That stronger claim still requires caution: no direct evidence has yet been found that Meiners personally knew, owned, consulted or rejected Prange.

---

## 2. Göttingen explicitly reviewed Prange's apparatus

The Göttingen Academy's eighteenth-century journal database (`Gelehrte Journale und Zeitungen der Aufklärung`) indexes a review of Prange's *Farbenlexicon* in Johann Beckmann's *Physikalisch-ökonomische Bibliothek*, vol. 12, pp. 454–458.

The volume was issued in Göttingen by Vandenhoeck & Ruprecht in 1783 (the Academy database indexes the review under 1782; bibliographic catalogues describe vol. 12 as 1783, and some holdings use 1782/1783). This dating discrepancy should be retained rather than silently harmonised.

Bibliographic controls:
- Niedersächsische Akademie der Wissenschaften zu Göttingen, GJZ18 database, review entry for Prange, *Physikalisch-ökonomische Bibliothek* 12, 454–458.
- Deutsche Digitale Bibliothek / Bayerische Staatsbibliothek, *Physikalisch-ökonomische Bibliothek* 12 (1783), URN `urn:nbn:de:bvb:12-bsb10130694-4`.
- Google Books full-view copies of vol. 12 identify Johann Beckmann as editor.

This establishes a local Göttingen reception channel independently of any hypothetical Meiners–Prange connection.

---

## 3. Beckmann: usefulness and reproducibility are different questions

Giulia Simonini's reconstruction of the review reproduces Beckmann's remarks from pp. 454–455. Beckmann regards the practical use of such a work as potentially `sehr nutzbar, mannigfaltig und bequem`, but immediately questions whether pigments can always be obtained in the same purity and whether different users following Prange's instructions will securely reproduce the same colour. His inclination is to answer that reproducibility question negatively.

This is extremely strong evidence for the present method because Göttingen's learned review culture already distinguished:

`useful reference idea`
from
`material reproducibility of the reference`.

Beckmann does not reject standardisation as such. He identifies a material-production problem inside the standard.

### Wilson-style reading

The colour chart is not a transparent carrier of a category. It is a manufactured object whose epistemic value depends on:

- pigment sourcing;
- pigment purity;
- mixture proportions;
- workmanship;
- copy-to-copy consistency;
- later material stability.

The standard itself therefore has provenance.

Add schema field:

```yaml
standard_material_provenance:
  pigment_source:
  pigment_purity_control:
  production_method:
  maker_or_colourist:
  copy_consistency:
  ageing_risk:
```

and a stop rule:

> `reference standard` is an epistemic role, not a guarantee of material identity across copies.

---

## 4. The paradox of completeness: 4,608 colours can be less usable than 74

The next finding is more important than a simple history of increasing precision.

Prange pursued extraordinary completeness. In natural-historical use, that granularity could become an obstacle. André Karliczek and Giulia Simonini reconstruct several points:

- each major colour family extends across many samples/pages;
- rapid optical comparison with a specimen becomes difficult;
- Franz Ambros Reuß later found multiple Prange candidates for a single mineralogical colour term;
- for `Röthlichbraun`, Reuß points to eight possible Prange samples;
- contemporary natural historians increasingly developed domain-specific `Farbentabellen` restricted to colours frequent in one kingdom or task.

An anonymous 1793 review explicitly asks why botanists do not use Lambert's colour pyramid or Prange's *Farbenlexicon*. Simonini interprets the reception evidence as showing that natural historians did not particularly welcome Prange's system, perhaps because of excessive detail and the absence of Latin colour terminology.

Production history reinforces the point. Archival evidence reconstructed by Simonini indicates that unsold/incomplete copies remained in Hendel's stock as late as 1816, some lacking half or all of their colour charts. Hand-painting thousands of samples was itself a severe production bottleneck.

### Method consequence

This defeats a linear model:

`more colour distinctions → greater precision → better science`.

A better model is:

`available continuum`
→ `possible exhaustive atlas`
→ **task-specific compression**
→ `usable comparison set`
→ `repeatable judgment`.

Add:

```yaml
reference_granularity:
task_specific_compression:
matching_ambiguity:
portability_cost:
production_cost:
```

Core rule:

> `more granular standard` ≠ `more usable standard`.

A successful standard must fit the discrimination burden of the task.

---

## 5. Widenmann 1794: adaptation rather than adoption

Johann Friedrich Wilhelm Widenmann's *Handbuch des oryktognostischen Theils der Mineralogie* (1794) is a clean case of a domain adapting a universal standard rather than simply adopting it.

Simonini shows that Widenmann:

- produced a mineralogical chart with 74 principal colour varieties;
- cross-referenced 55 generic colour terms to Prange;
- explicitly warned that only one lightness variation of each colour could be represented;
- expected the observer to compensate mentally when comparing minerals;
- compressed many Prange samples into single mineralogical categories.

This is not information loss in a simple sense. It is a deliberate reduction designed to make a comparison instrument usable for mineralogy.

The operation is:

`Prange universal colour atlas`
→ `domain selection`
→ `74 mineralogical varieties`
→ `observer compensation for omitted lightness`
→ `usable field/classroom comparison`.

This is a strong example of `operation_generated_by_constraint` and `observer_training_function` working together.

---

## 6. Reuß 1801: cross-reference can expose category non-equivalence

Franz Ambros Reuß used Widenmann's cross-references to Prange in his mineralogical work. Simonini notes that Reuß links 45 colour terms with Prange samples (largely following Widenmann).

The interesting result is not merely diffusion. Comparisons between Widenmann and Prange show that identical or near-identical verbal names do not consistently map to identical material samples, and Widenmann can treat materially distinct Prange mixtures as belonging to one mineralogical colour variety.

Thus:

`same colour word`
≠ `same material recipe`
≠ `same perceived hue`
≠ `same domain category`.

This is directly relevant to travellers' descriptions of human complexion: verbal equivalence cannot be presumed to establish observational equivalence.

---

## 7. Walter 1796: Prange enters anatomical specimen description directly

The strongest new primary-control case is Friedrich August Walter's *Anatomisches Museum* (Berlin, 1796).

Walter's catalogue describes human urinary and renal calculi through fields including:

- age/source;
- figure;
- size;
- colour;
- surface;
- material consistency;
- weight;
- anatomical/operative context.

The Heidelberg digitisation gives direct examples such as:

- `Blass Goldgelb (Tab. XVIII. No. 13)`;
- `Blass Weizengelb (Tab. XVII. No. 13)`;
- `Hell Bräunlichgelb (Tab. XVI. No. 41)`;
- `Blass Rohrbraun (Tab. XLVI. No. 45)`.

Modern comparison by Simonini establishes what Walter himself states explicitly at the end of the urinary-stone section: he named the colours according to Prange's *Farben-Lexicon*, and the plate/number beside each stone's colour identifies the corresponding position in Prange.

Simonini counts **157 urinary-calculus specimens** described through this reference system.

This closes the adoption chain:

`Prange material swatch`
→ `visual comparison with anatomical specimen`
→ `Prange colour name`
→ `plate + number`
→ `catalogue record`.

Sources:
- Friedrich August Walter, *Anatomisches Museum*, vol. 1 (Berlin, 1796), especially p. 84 and individual specimen entries; Heidelberg University Library digital edition, DOI series `10.11588/diglit.11272`.
- Giulia Simonini, *Color Charts in 18th-century Europe: Natural, Pigmentary, and Trichromatic*, pp. 216ff.

### Why this matters for Meiners

This case demonstrates that by 1796 a human-anatomical collection could use Prange's standard to encode bodily/pathological objects numerically and reproducibly.

It does **not** prove that skin colour could have been standardised with equal success. Skin differs from calculi in lability, illumination dependence, living-body variation, and inferential stakes.

But it removes a weak explanation:

> “German scholars around 1790 had no practical way to connect a bodily colour observation to a material standard.”

They did.

The sharper question becomes:

> Why was material numerical colour comparison adopted for certain human anatomical objects while Meiners's comparison of living peoples remained organised through reports, words, causal hypotheses and genealogical categories?

This is now a historical problem of **task/domain selection**, not a generic absence of technical possibility.

---

## 8. A Göttingen circulation bridge: Blumenbach owned Walter's *Anatomisches Museum*

The Blumenbach Online reconstruction of Johann Friedrich Blumenbach's private library lists:

`Walter, anat. Museum. Berlin 796 mit Kpfr.`

as catalogue entries Quarto-0302–0303 / ID 0496.

The searchable auction catalogue likewise records Walter's *Anatomisches Museum* in Blumenbach's library.

This establishes that Walter's Prange-coded anatomical catalogue entered Blumenbach's private book collection.

Claim limit:
- ownership is established at catalogue level;
- active reading, use of the colour references, or transfer into Blumenbach's human-variety method is **not** established;
- no Prange *Farbenlexicon* has yet been found in the searchable Blumenbach private-library record.

This is nevertheless useful because it shows that a Prange-derived colour-coding practice in anatomy was bibliographically present in the Göttingen orbit.

---

## 9. Prange's own intended domain was wider than minerals, plants and insects

Simonini's reconstruction of Prange's practical examples notes that *Farbenlexicon* and *Schule der Mahlerey* supplied numerical colour instructions for motifs including flowers, insects, landscapes and **human bodies**.

This matters because it weakens another possible explanation: that Prange's standard was conceived only for non-human naturalia.

Still, intended applicability is not equivalent to scientific adoption:

`authorial intended domain`
≠ `actual user domain`
≠ `disciplinary evidentiary authority`.

---

## 10. Meiners 1792: apparatus availability and inferential ambition diverge

The near-contemporary Krünitz encyclopaedia's digest of Meiners's 1792 essay reproduces the essay's research programme with unusual clarity. Meiners asks whether:

- national colour depends more on climate or descent;
- children's colour depends more on birthplace or parental blood;
- colour is a secure sign of human races / gradations;
- a finite number of principal colours can be distinguished;
- one or several principal colours can be treated as original/basic colours from which others arose.

Article source:
- Christoph Meiners, “Ueber die Farben, und Schattierungen verschiedener Völker,” *Neues Göttingisches historisches Magazin* I/4 (1792), pp. 611–672.
- Direct volume: BSB / DDB, vol. 1 (1792), URN `urn:nbn:de:bvb:12-bsb10738733-5`.
- Near-contemporary digest: Krünitz, *Oekonomisch-technologische Encyclopädie*, vol. 71, article “Leibes-Farbe der Menschen,” p. 657ff.

Secondary page-level pointers indicate that Meiners also explicitly catalogues environmental causes that lighten, darken or mask skin colour (sun, climate, air/wind, location, clothing, occupation, cleanliness) while continuing to ask what colour can reveal about descent and mixture.

The direct 611–672 article still requires page-by-page primary transcription before final promotion of detailed argumentative claims.

### The new comparison

Around Meiners's essay, three regimes coexist:

1. **Prange / Walter regime**  
`object → swatch → number → portable description`.

2. **Widenmann regime**  
`universal standard → domain compression → trained comparison → mineral category`.

3. **Meiners regime**  
`traveller/observer report → unstable colour word → aggregation → climate/descent/mixing/rank inference`.

The historical question is not which regime is simply “more scientific.” It is why each task selected a different evidentiary architecture.

---

## 11. Revised schema: apparatus adoption must become explicit

Add to the colour ontology:

```yaml
apparatus_availability:
  status:
    - unavailable
    - available_in_field
    - locally_reviewed
    - locally_held
    - explicitly_cited
    - unknown

apparatus_adoption:
  status:
    - adopted_directly
    - adapted
    - selectively_cross_referenced
    - explicitly_rejected
    - available_but_untraced
    - unknown

adoption_barrier:
  - cost
  - production_time
  - material_reproducibility
  - excessive_granularity
  - nomenclature_mismatch
  - portability
  - task_mismatch
  - disciplinary_norm
  - observer_burden
  - unknown

standardisation_layer:
  - vocabulary
  - material_reference
  - observer
  - workflow
  - data_record
  - inference

reference_granularity:
task_specific_compression:
matching_ambiguity:
```

Core rule:

> **Available apparatus ≠ adopted apparatus ≠ usable apparatus ≠ validated inference.**

---

## 12. New stop rules

### Stop rule 11 — no technical-availability-to-use inference

A colour chart's existence in the relevant decade or city does not prove an actor knew or used it.

### Stop rule 12 — no ownership-to-use inference

A book in a private or institutional catalogue proves bibliographic availability, not active reading or methodological uptake.

### Stop rule 13 — no completeness-to-precision inference

A larger reference set can increase matching ambiguity and observer burden.

### Stop rule 14 — no adoption-to-inference transfer

A chart may standardise description while leaving causal, genealogical or ontological inference entirely unsupported.

### Stop rule 15 — distinguish adaptation from adoption

Domain-specific pruning may be the central epistemic operation rather than degradation of a universal standard.

---

## 13. Evidence-status ledger

| Claim | Status | Next closure |
|---|---|---|
| Prange 1782 contained 4,608 numbered material colour samples | strong bibliographic / material scholarship | direct sample-copy inspection optional |
| Prange intended visual matching + number notation | strong primary quotation via multiple scholarly transcriptions | direct Prange page image desirable |
| Prange was reviewed in Göttingen in Beckmann's journal | direct journal-database + volume metadata | direct pp. 454–458 scan/OCR |
| Beckmann questioned pigment/reproduction consistency | strong exact primary quotation reproduced in current scholarship | direct review scan desirable |
| Natural historians often found Prange too granular | strong modern reconstruction + contemporary 1793 review pointer | identify/directly capture Anonymous 1793b |
| Widenmann 1794 cross-referenced Prange and compressed to 74 mineral colours | strong direct/archival reconstruction | direct Widenmann pages if promoted |
| Reuß 1801 used Prange via Widenmann; one term could map to 8 samples | strong source-level reconstruction | direct Reuß p. 86 capture |
| Walter 1796 explicitly used Prange for urinary-calculus colours | **primary direct + modern cross-check** | direct p. 84 OCR/page capture if desired |
| Walter encoded 157 urinary-calculus specimens through Prange | strong modern item-by-item reconstruction | sample audit sufficient |
| Blumenbach owned Walter 1796 | **direct private-library catalogue record** | no further closure for ownership |
| Blumenbach used Walter's colour method | **unproven** | marginalia/notes/citations needed |
| Meiners knew/rejected Prange | **unproven** | search correspondence/library/article text |
| Prange apparatus solves Meiners's skin-colour problem | **too strong / not established** | task-material comparison needed |

---

## 14. Immediate next research queue

1. Search Meiners's 1792 essay and correspondence/library records for `Prange`, `Farbenlexicon`, `Lambert`, `Farbenpyramide`, `Schäffer`, `Muster`, `Tafel`.
2. Identify `Anonymous 1793b`, p. 300, which asks why botanists do not use Lambert or Prange; capture exact publication context.
3. Close Beckmann's pp. 454–458 directly from the BSB/DDB volume.
4. Capture Walter 1796 p. 84 directly and sample 10–20 coded specimens against Prange's register.
5. Search Blumenbach's surviving notes/correspondence for Walter 1796 and colour standards.
6. Establish acquisition/provenance history of SUB Göttingen's Prange *Schule der Mahlerey* copy; do not infer contemporary presence from current holding.
7. Compare the material problem of urinary calculi with the material problem of living skin: illumination, mobility, exposure, physiological variation, dirt/clothing, and the inferential target.
8. Return to Gatterer heraldry with the same apparatus-adoption distinction: conventional hatching succeeds partly because the category-space is finite and the decoding operation is task-specific.

---

## 15. Strongest formulation from this sweep

> **The history of colour standardisation is not a linear movement from subjective words to objective swatches. Around 1790, scholars already chose among competing evidentiary architectures. Universal atlases could fail through excessive granularity and unstable manufacture; successful domains compressed them into task-specific tables; anatomical cataloguers could use material colour codes without thereby authorising genealogical inference. The methodological problem is therefore to reconstruct why an apparatus became usable and authoritative for one operation but remained absent, unnecessary, or untraced for another.**

And, for the Meiners comparison:

> **The question is no longer whether an eighteenth-century material colour standard was technically possible. It is why the classification of human complexion did not obviously pass through the same standardising gate that contemporary mineralogical and anatomical colour description could use.**
