# Evidence and Provenance Policy

This corpus separates **what was observed**, **what kind of source supports it**, **how far the claim is justified**, and **how the repository should treat the record**. These are different questions. A catalogue record for a book, an archival note about an engraver, a direct frontispiece image and a project inference can support different claims at different resolutions.

The formal ontology is in [`schema/ONTOLOGY.md`](../schema/ONTOLOGY.md). Canonical records validate against [`schema/record.schema.json`](../schema/record.schema.json).

## 1. Three independent axes

### A. Evidence basis

`evidence_basis` records what kind of evidence supports the claim.

- `primary_direct` — the relevant object, page, plate, scan, transcription, advertisement or review was directly inspected.
- `primary_derivative` — a trustworthy reproduction or derivative image of the primary item was inspected.
- `institutional_catalogue` — library, museum, archive or authority metadata was inspected, but the relevant object/image was not directly controlled for the claim in question.
- `market_catalogue` — auction/dealer description or market image.
- `correspondence` — archive/library/museum/curator correspondence.
- `secondary_scholarship` — modern scholarly reconstruction.
- `research_derived` — project inference, synthesis, comparison or calculation.
- `mixed` — more than one evidence basis materially supports the claim.

Evidence basis is descriptive. It is not itself a confidence ranking. A market photograph can directly establish a composition, while an institutional catalogue may establish only title and date.

### B. Assertion status

`assertion_status` records how far the particular claim goes.

- `established` — supported at the stated claim granularity.
- `probable` — best current explanation but not yet demonstrated.
- `possible` — live hypothesis with positive reason to test.
- `unresolved` — evidence does not yet discriminate.
- `bounded_negative` — a defined search returned no result; this is never universal absence.
- `disconfirmed` — a previous claim is contradicted by stronger evidence.

### C. Lifecycle status

`lifecycle_status` records repository treatment, not truth status.

- `canonical` — loaded into the current synthesis and expected to validate against the current schema.
- `active` — live research input not yet canonicalised.
- `frozen` — evidential snapshot or closed analytical branch retained without silent rewriting.
- `quarantined` — discovery, experimental, operational or out-of-scope material excluded from canonical queries.
- `superseded` — replaced by a named canonical dataset/record but retained for auditability.

The file-level lifecycle is recorded in `data/dataset_manifest.csv`.

## 2. Mapping legacy `evidence_status` values

Older files used one field for several concepts. During canonicalisation, decompose rather than copy the old string mechanically.

- legacy `verified_primary` normally maps to `evidence_basis=primary_direct`; the assertion can still be `established`, `probable` or `unresolved` depending on the claim.
- legacy `verified_catalogue` maps to `evidence_basis=institutional_catalogue`.
- legacy `reported_correspondence` maps to `evidence_basis=correspondence`.
- legacy `research_inference` maps to `evidence_basis=research_derived` and must carry an explicit assertion status.
- legacy `unresolved` maps to `assertion_status=unresolved`, not to an evidence basis.
- mixed strings such as `verified_catalogue_plus_web_image` must be decomposed claim by claim. The catalogue may establish a signature while the derivative image supports only a probable design identification.

## 3. Claim granularity

A source should be attached to the smallest claim it actually supports.

Examples:

- A catalogue entry can verify title, imprint, date, signature and catalogued contributors.
- A librarian's report that a box contains many Tyroff engravings can verify the existence of that holdings cluster, but not the identity of every plate.
- A cropped image can verify composition-level iconographic features, but may be insufficient to establish front-matter placement or binding sequence.
- A full digital copy can support placement, sequence and copy-specific state, but does not automatically establish the chronology of plate alteration across other copies.
- A dated engraver signature can be transcribed from a catalogue without proving that two impressions came from the same physical matrix.

Recommended `claim_scope` values include `programme_identity`, `design_identity`, `matrix_identity`, `matrix_state_identity`, `host_pairing`, `copy_state`, `agent_identity`, `imprint_resolution`, `production_relation`, `custody_relation`, `publication_transition`, `historiographical_prior_art` and `historiographical_gap`.

## 4. Programme, design and plate identity

Do not collapse identity levels.

`programme identity != design identity != matrix identity != matrix-state identity != impression identity != copy identity`

In particular:

- a shared motto does not establish the same design;
- the same design does not establish the same physical plate;
- the same matrix can have multiple states;
- the same host issue can survive in copies with different frontispiece configurations;
- a detached or inserted frontispiece can preserve a design while its original host relation remains unresolved.

Use the strongest justified relationship:

- `same_design_as` — compositional identity only;
- `same_matrix_as` — physical matrix identity demonstrated or strongly evidenced;
- `variant_state_of` — same matrix with a distinct state established;
- `derived_from_design` — one design demonstrably adapts another;
- `probable_relation` — similarity worth testing;
- `no_relation_established` — co-presence in the corpus only.

Matrix identity should eventually be tested through dimensions, line-level details, lettering, damage/wear, plate marks, re-engraving/retouching, signatures and copy chronology.

## 5. Person and firm authority control

Do not normalise Weigel-family names prematurely. Nürnberg archival/catalogue evidence creates collision risk among Christoph Weigel d. Ä., Johann Christoph Weigel, their widows, heirs and later Tyroff successors.

Store separately:

1. the literal imprint or source form;
2. the catalogue authority assignment;
3. the project's current person/firm resolution;
4. the assertion status and source for that resolution.

Publisher succession should be encoded as dated relationships among people/firms rather than treated as spelling variants of one publisher. A high-confidence resolution of `C. Weigels Witwe` to one widow remains an assertion unless the literal source explicitly names her.

## 6. Correspondence policy

Connected research correspondence is used as a discovery and provenance layer. For this public repository:

- retain institution, date, attachment title if useful, and a sanitised factual note;
- omit personal email addresses, message IDs, signatures and full private correspondence;
- set `evidence_basis=correspondence` until independently promoted;
- do not redistribute unpublished scans or attachments unless rights and purpose are clear;
- a correspondence-derived fact can still have `assertion_status=established` at the narrow level of “institution X reported Y”, while the historical proposition Y may remain probable or unresolved.

## 7. Market and volatile web evidence

Market records can preserve unique copy photographs and therefore have real evidentiary value. They are nevertheless volatile.

- Preserve stable item IDs, dates and image URLs where possible.
- Distinguish description-level claims from image-level observations.
- When the market image proves composition but not a production signature, record exactly that split.
- Canonicalise the observation, not the dealer's interpretation.
- Keep raw web-discovery datasets outside canonical queries once their useful observations have been promoted.

## 8. Negative evidence

Negative searches are valuable but bounded. Record the search scope, date and query environment. Prefer:

> “The searchable 22-volume index and supplements returned no Eccard/Eckhart/Döderlein name hit.”

rather than:

> “Köhler never cited Eccard or Döderlein.”

Use `assertion_status=bounded_negative` and state the reopen condition.

## 9. Full-sweep and canonicalisation rule

Discovery should preserve the complete returned set before thematic selection. Selection, deduplication and promotion happen later.

The canonicalisation sequence is:

1. preserve raw discovery/control datasets;
2. identify stable record keys;
3. merge overlapping records without deleting source-specific literal fields;
4. promote claim-specific observations into canonical records;
5. mark absorbed datasets `superseded` in `data/dataset_manifest.csv`;
6. freeze closed contextual branches or quarantine operational/experimental material;
7. keep every open question tied to a concrete new-source or comparison condition.

## 10. Freeze rule

A question is frozen when additional generic searching is unlikely to change the present conclusion and a new class of evidence is required. Examples include:

- a design-level transition already fixed by direct controls on adjacent years, while matrix identity remains a separate open question;
- a bounded citation search whose next escalation requires a page-level concordance or archival source;
- a historiographical comparator whose purpose is to delimit prior art rather than to enlarge the core corpus.

Frozen does not mean “certain forever”. It means the project has specified what evidence would justify reopening the branch.

## 11. Manual-escalation / keep-moving rule

The project must not spend disproportionate research time fighting a digital front end, viewer cache, blocked PDF route, OCR endpoint, page-number mapper or other technical access problem when the remaining historical question is narrow and a human can close it cheaply.

The single operational queue for these cases is [`docs/MANUAL_DOWNLOAD_AND_INSPECTION_LOG.md`](MANUAL_DOWNLOAD_AND_INSPECTION_LOG.md). Do not create parallel ad hoc lists in chat or other notes.

Escalate a source to the manual queue when **all** of the following are true:

1. the historical target is already sharply bounded (specific page, plate, paragraph, keyword set or small page range);
2. automated access has become materially more expensive than the historical reasoning itself;
3. a user action such as one click, one download, a small OCR pass, or a few screenshots is likely to close the gap;
4. failure to perform that manual action does not prevent productive work on other branches.

For every escalation, record:

`source + stable carrier/ID + exact target + smallest useful user action + expected evidentiary upgrade + status`.

Examples of acceptable requests:

- `download this one PDF and OCR pp. 611–672`;
- `open p. 23 and screenshot the paragraph beginning X`;
- `search this auction catalogue for Prange / Lambert / Schäffer and return hit pages only`;
- `capture the bottom 20% of this plate to resolve the engraver signature`.

Avoid requests such as `read this whole book`, `browse the archive`, or `see if anything interesting appears` unless discovery genuinely cannot be bounded further.

### Research-behaviour rule

Once a manual escalation has been logged:

- **do not stall the main sweep waiting for it**;
- do not repeatedly retry the same hostile viewer unless a genuinely new automated route appears;
- continue with the highest-value branches that can be advanced automatically;
- preserve the unresolved claim at its current evidence status;
- when the user later supplies the page/OCR/image, promote only the claims actually closed by that material and mark the queue item `done_user`;
- if automation later closes it first, mark `resolved_no_manual_needed` and remove the burden from the user.

Operational principle:

> **Escalate cheap human closure; automate everything else; keep the research moving.**
