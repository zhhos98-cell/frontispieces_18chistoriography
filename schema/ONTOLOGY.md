# Corpus ontology and lifecycle model

Version: 1.0  
Frozen baseline: 2026-08-27

## 1. Purpose

The repository has grown from a discovery log into a provenance-first corpus. The ontology therefore distinguishes the identity of a verbal/semantic programme, a graphic design, a physical printing matrix, a matrix state, an individual impression, the publication that hosts it, and the surviving copy in which it is observed.

The governing identity rule is:

`programme identity != design identity != matrix identity != matrix-state identity != impression identity != host identity != copy identity`

A shared inscription can survive across different designs. A design can be re-engraved on a new matrix. One matrix can be reworked into later states. One state can yield many impressions. An impression can be rebound, detached, inserted, or omitted in a surviving copy. A host work can change publication rhythm while reusing older visual stock.

The preferred atomic research unit remains the **witness occurrence**: one source-backed statement that a programme/design/matrix/state/impression appears, or is reported to appear, in a particular host issue and, where possible, a particular surviving copy.

## 2. Core record types

### `programme`
A recurring verbal, semantic, or allegorical programme that may be realised by more than one graphic design.

Example: `Historia. Genealogia. Heraldica. Testes temporum et veritatis.`

Identity is established by the programme itself, not by exact typography or composition.

### `design`
A compositional/iconographic arrangement independent of the physical copperplate on which it was engraved.

Current controlled designs:

- Type A: tree composition;
- Type B: Müller–Tyroff architectural composition;
- Type C: seated Historia / open-book composition.

`same_design_as` never implies `same_matrix_as`.

### `matrix`
One physical printing matrix (normally a copperplate in the present corpus). Matrix identity requires material evidence such as dimensions, line-level coincidence, lettering, plate mark, stable defects, scratches, wear, retouching, or explicit contemporary custody evidence.

### `matrix_state`
A chronologically distinguishable state of one matrix after reworking, correction, relettering, retouching, or other physical intervention. A dated signature on an impression can date a state only when the relationship to the matrix is independently established.

### `impression`
One physical pull from a matrix/state. Impression-level features include paper, trimming, inking, offset, plate mark and copy-specific damage on the printed sheet.

### `host_work`
A bibliographic/serial work or publication regime, e.g. the *Geschichts-, Geschlechts- und Wappen-Calender*, Gatterer's *Handbuch*, or the cumulative Seyfart/Raspe *Wappenbuch*.

### `host_issue`
One dated issue, edition, volume, or annual instalment of a host work. `host_year` and `imprint_year` must be stored separately when they diverge or when indexing contamination is possible.

### `copy`
One surviving exemplar, institutional copy, digitised copy, or market object. Copy-specific states are evidence, not noise: missing plates, inserted foreign frontispieces, extra mounted engravings, rebinding, detachment and annotation remain copy properties.

### `witness`
A source-backed occurrence linking a programme/design/matrix/state/impression to a host issue and optionally a copy. A witness may be secure at one identity level and unresolved at another; this must be represented by claim-specific observations rather than by promoting the whole record to the strongest claim.

### `agent`
A person, family member, workshop, publisher, printer, bookseller, engraver, designer, editor, owner, institution or firm authority. Literal source forms are retained separately from authority resolution.

### `source`
The evidence item itself: primary object/scan, institutional catalogue, market catalogue/image, correspondence, secondary scholarship, or research-derived note.

### `assertion`
A claim connecting two records. Assertions carry their own evidence basis, status, confidence, sources and claim limit. This is where inference lives; inference is not encoded as though it were an object property.

### `historiography_claim`
A claim about what existing scholarship has already established, what it leaves open, or what counts as prior art for the present project. Historiography claims belong to the analytical layer and are kept distinct from primary-object assertions.

### `lead`
Operational research material only. Leads, locators and search queues are not canonical corpus entities unless promoted into one of the types above.

## 3. Three-axis evidence model

The legacy `evidence_status` field mixed three different questions. Version 1 separates them.

### A. `evidence_basis`: what kind of evidence supports the claim?

Allowed canonical values:

- `primary_direct` — the relevant primary object/page/plate/scan was directly inspected;
- `primary_derivative` — a trustworthy reproduction or derivative image of the primary item was inspected;
- `institutional_catalogue` — library, museum, archive or authority metadata;
- `market_catalogue` — auction/dealer catalogue or market image;
- `correspondence` — archive/library/museum correspondence;
- `secondary_scholarship` — modern scholarly reconstruction;
- `research_derived` — project inference, calculation or synthesis;
- `mixed` — more than one evidence basis materially supports the claim.

### B. `assertion_status`: how far does the claim go?

- `established` — supported at the stated claim granularity;
- `probable` — best current explanation but not yet demonstrated;
- `possible` — live hypothesis with positive reason to test;
- `unresolved` — evidence does not yet discriminate;
- `bounded_negative` — a defined search found no result; never universal absence;
- `disconfirmed` — a previous claim is contradicted by stronger evidence.

### C. `lifecycle_status`: how should the repository treat the record/dataset?

- `canonical` — loaded into the current synthesis and expected to validate against the current schema;
- `active` — still live research input, not yet canonicalised;
- `frozen` — evidential snapshot or closed analytical branch; retained and not silently rewritten;
- `quarantined` — discovery, experimental, operational or out-of-scope material excluded from canonical queries;
- `superseded` — replaced by a named canonical dataset/record but retained for auditability.

Lifecycle is not epistemic confidence. A frozen record can be strong or weak; it is frozen because the present research decision is complete at its intended resolution.

## 4. Claim scopes

Claims should name the identity level they support. Recommended `claim_scope` values include:

- `programme_identity`
- `design_identity`
- `matrix_identity`
- `matrix_state_identity`
- `impression_identity`
- `host_pairing`
- `copy_state`
- `agent_identity`
- `imprint_resolution`
- `production_relation`
- `custody_relation`
- `publication_transition`
- `historiographical_prior_art`
- `historiographical_gap`

A source that supports `design_identity` must not be promoted to `matrix_identity` without new evidence.

## 5. Core relationship predicates

Recommended predicates:

- `realises_programme`
- `same_design_as`
- `derived_from_design`
- `engraved_on_matrix`
- `state_of_matrix`
- `printed_from_state`
- `appears_in_host_issue`
- `exemplar_of_host_issue`
- `issue_of_host_work`
- `bound_in_copy`
- `detached_from_copy`
- `inserted_into_copy`
- `designed_by`
- `engraved_by`
- `printed_by`
- `published_by`
- `issued_by`
- `continued_firm_of`
- `successor_to`
- `predecessor_to`
- `owned_by`
- `evidenced_by`
- `reported_in`
- `cites`
- `reuses_material_from`
- `same_matrix_as`
- `variant_state_of`
- `probable_relation`
- `no_relation_established`

## 6. Merge and deduplication rules

### Stable keys

Use the strongest available stable key, not a normalised title string alone.

- programme: canonical programme id;
- design: canonical design id;
- matrix: physical matrix id only after matrix-level evidence;
- host issue: `host_work + host_year/edition + literal imprint when needed to discriminate`;
- copy: institutional shelfmark/object id, or stable market-object id when no institutional copy exists;
- witness: `host_issue + copy/source anchor + observed programme/design`; 
- source: DOI/URN/PPN/shelfmark/object id/stable URL plus source institution;
- agent: authority id when resolved; otherwise a provisional id preserving literal name form.

### Field precedence

Newer does not automatically mean better. When overlapping records are merged:

1. preserve every distinct source;
2. prefer direct primary observation for the field it actually supports;
3. prefer institutional object metadata over market metadata for bibliographic facts;
4. retain market images when they provide visual evidence unavailable institutionally;
5. never overwrite a conflicting literal imprint, signature or title with a normalised authority form;
6. keep conflicts as parallel source-backed observations or assertions;
7. promote a relation only to the strongest identity level actually demonstrated.

### Supersession

A legacy dataset can be marked `superseded` only after its non-duplicate information has been migrated or explicitly declared outside the canonical scope. Superseded files remain in Git history and are listed in the dataset manifest.

## 7. Freeze and quarantine rules

Freeze a branch when:

- the intended question is closed at its stated resolution;
- additional work would require a new class of primary evidence rather than more search repetition;
- a newer canonical dataset has absorbed the relevant records;
- a historiographical comparator has served its boundary-setting function.

Quarantine material when:

- it is a locator/search artifact rather than an evidence record;
- it is an experimental census not yet integrated with the core ontology;
- it is a broad comparator outside the plate/frontispiece object scale;
- it derives from private correspondence and has not been independently promoted;
- it is a volatile web/market discovery record preserved for provenance but unsuitable as a canonical object description.

## 8. Current core versus extension

The canonical core is the longitudinal material-bibliographic problem:

`programme -> design -> matrix/state -> witness occurrence -> host issue -> surviving copy`

with agent/firm and publication-stock relations attached.

Contextual extensions such as heraldic historisation, genealogical proof-distance, evidentiary vocabulary and Gatterer method remain valuable, but they enter canonical synthesis only when they explain a core object, relation or historiographical boundary. Otherwise they are frozen or quarantined as controlled extensions.

## 9. Current closure criterion

The repository is considered substantively closed when:

1. the programme/design chronology is represented in one canonical witness dataset;
2. open matrix-level questions are explicitly separated from already-closed design-level questions;
3. copy afterlives and publication-regime changes remain visible rather than normalised away;
4. discovery/experimental files are excluded from canonical queries through lifecycle metadata;
5. historiographical prior art is mapped to claims, so the project does not present established scholarship as novelty;
6. every remaining open question has a concrete reopen condition tied to a new source or comparison, not an indefinite instruction to search more.
