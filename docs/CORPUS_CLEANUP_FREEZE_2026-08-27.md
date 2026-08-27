# Corpus cleanup, merge and freeze — 2026-08-27

## Result

The repository has moved from discovery accumulation to a controlled canonical corpus.

The cleanup does **not** delete legacy research files. It separates canonical data from active contextual material, frozen analytical branches, quarantined discovery/experimental data and superseded snapshots. This preserves provenance while preventing old or overlapping files from silently competing with the current synthesis.

## 1. Ontology frozen

Canonical identity hierarchy:

`programme -> design -> matrix -> matrix_state -> impression -> host_issue -> copy`

with `witness` as the source-backed occurrence tying these levels together.

Supporting entities:

- `host_work`
- `agent`
- `source`
- `assertion`
- `historiography_claim`
- `lead`

The governing rule is:

`programme identity != design identity != matrix identity != matrix-state identity != impression identity != host identity != copy identity`

See `schema/ONTOLOGY.md` and the revised `schema/record.schema.json`.

## 2. Evidence model cleaned

The legacy `evidence_status` field mixed different logical dimensions. The current model separates:

1. `evidence_basis` — what kind of evidence supports the claim;
2. `assertion_status` — how far the claim is justified;
3. `lifecycle_status` — how the repository should treat the record/dataset.

See `docs/EVIDENCE_POLICY.md`.

## 3. Canonical data layer

### `data/canonical/entities.jsonl`

18 canonical/active entities and assertions covering:

- the Historia/Genealogia/Heraldica programme;
- Type A/B/C designs;
- major host works/regimes;
- Weigel/Tyroff/Gatterer/Raspe authorities;
- the current high-confidence but non-literal resolution of `C. Weigels Witwe`.

One legacy relationship-direction error was corrected during migration: Barbara Sibylla Weigel is encoded as `child_of` Christoph Weigel d. Ä., not as his parent.

### `data/canonical/frontispiece_witnesses.jsonl`

25 claim-specific witness records.

This file merges the two overlapping composition-control datasets by record identity and evidentiary strength rather than by filename/date assumptions. It also promotes later controls that had entered the annual census but not both composition files.

Important merged gains include:

- 1736 Type A direct market-image control;
- 1747 Type C structural control;
- 1749 Type C control;
- two independent 1756 Type C copies;
- 1757 final numbered annual Type C control;
- 1759 Type A re-hosting;
- 1762 `M. Turoff fec. 1755` separated into signature evidence versus probable design pairing.

### `data/canonical/annual_host_census.csv`

43 host-year/regime rows from 1723 through the 1767 cumulative transition.

This replaces `data/wappenkalender_witness_census.csv` as the annual chronological spine. The older file is retained as a superseded discovery-era snapshot because several rows had become stale as new direct market-image controls were added.

### `data/canonical/historiography_claims.jsonl`

9 claim-level historiographical boundaries covering:

- Araújo on Gatterer, visual evidence and media;
- Palmer on long-duration frontispiece prototypes/reuse;
- Jung on transmedial reuse and host-dependent meaning;
- Heringman/Lake on antiquarian media ecologies;
- Betti on physical plate provenance/custody/repair/reprinting;
- Bowen/Imhof on longitudinal single-matrix histories;
- extra-illustration/thickening scholarship;
- Miller/Gierl on Göttingen material evidence and historical sciences;
- the remaining bounded project-specific gap.

### `data/canonical/research_questions.jsonl`

10 bounded questions with explicit reopen conditions.

Two are already frozen:

- Type B -> Type C design replacement boundary at 1746/1747;
- final generic historiographical sweep.

Seven core object/network questions remain active:

1. 1725 programme adoption;
2. 1739/1740 Type B entry;
3. early/late Type A physical matrix continuity;
4. Type C matrix/state sequence and `fec. 1755`;
5. 1767–1776 late copy-level frontispiece persistence;
6. Weigel/Tyroff/Raspe frontispiece-stock custody;
7. issue-level resolution of `C. Weigels Witwe`.

One additional axis, `colour`, is recorded as deferred and has not been allowed to destabilise this closing pass.

## 4. Lifecycle classification of the 27 legacy data files

See `data/dataset_manifest.csv` for file-level decisions.

Current counts:

- **9 active** legacy datasets: still useful contextual/core-network inputs;
- **7 superseded** datasets: absorbed into canonical files and retained as snapshots;
- **6 frozen** datasets: analytically closed extensions/comparators;
- **5 quarantined** datasets: operational locators, discovery inventories, experimental census or volatile web layer.

No legacy file has been physically deleted. Lifecycle controls determine whether it should enter a canonical query.

## 5. Major merge decisions

### Overlapping composition controls

`frontispiece_composition_control_1726_1765_2026-08-26.jsonl` and `frontispiece_composition_control_1728_1751_2026-08-26.jsonl` are both superseded.

The narrower-named file was actually later-edited and contained unique later evidence. Therefore the merge used source-backed record-level union rather than “new filename wins” or “wider range wins.”

### Weigel authority files

`weigel_firm_authority_control_2026-08-26.jsonl` and `weigel_publisher_authority_overrides_2026-08-26.jsonl` are merged into canonical agents plus an explicit imprint-resolution assertion.

Literal imprint, catalogue authority assignment and project person resolution remain separate.

### Research leads

`research_leads.csv` is quarantined as an operational mixed queue. Closed leads, open questions, bounded negatives and historiography no longer coexist as if they were one evidence table.

Live questions are promoted into `data/canonical/research_questions.jsonl`.

## 6. Historiography: what is now frozen as prior art

The final sweep removes several broad novelty claims.

The project should not claim novelty simply for showing that:

- frontispieces or engravings can do epistemic work;
- visual and material media shape historical evidence;
- frontispiece prototypes recur and vary over decades;
- reused designs change meaning in new hosts;
- copperplates have long custody, repair, alteration and reprinting histories;
- one physical plate can be followed longitudinally through multiple states;
- owners remake books through extra-illustration;
- Göttingen systematised material evidence and auxiliary historical sciences.

See `docs/HISTORIOGRAPHY_FINAL_SWEEP_2026-08-27.md`.

## 7. Remaining defensible opening

The strongest current opening is the specific transition between an already-existing Nürnberg material information infrastructure and its later re-hosting/re-specification within the Gatterer/Göttingen historical-science environment.

The pre-Göttingen apparatus includes:

- annual genealogy/heraldry calendars;
- armorial plates and genealogical tables;
- recurrent threshold programmes;
- publisher-held reusable copper stock;
- historical modules and advertising;
- cross-format extraction/recomposition;
- copy-level augmentation, omission and insertion.

The key question is therefore not whether Göttingen “invented” visual/material evidence. It is whether and how an older commercial/serial apparatus that already made historical materials portable, modular and comparable was **selectively captured, re-hosted and epistemically re-specified** inside a new institutional and methodological programme.

This is currently a bounded hypothesis, not a conclusion assumed by the data model.

## 8. Stop rules

The generic web sweep is closed.

Do not reopen broad searches for `frontispiece`, `visual evidence`, `plate reuse`, `extra-illustration` or `Gatterer images` unless a result directly overlaps the project-specific object/network.

Open object questions only when their explicit `reopen_rule` is met. This should prevent another expansion cycle in which contextual comparators accumulate faster than the core claim changes.

## 9. Deferred next axis

`Colour` is preserved as the next analytical branch. The first move should be ontological rather than interpretive: distinguish hand-colouring, printed colour, tincture keys/conventions, fidelity claims, classificatory colour, copy-specific colouring and later intervention before asking how colour intersects with Göttingen historical method and controversy.
