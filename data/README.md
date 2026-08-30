# Data layer

Repository status is controlled by `../CLOSURE_STATE_2026-08-30.json` and `../FINAL_CLOSURE_2026-08-30.md`. Dataset lifecycle and load policy are controlled by `dataset_manifest.csv`.

## Authority order

1. `canonical/` — canonical ontology-compliant entities, witnesses, annual host census, historiography claims, bounded research questions, and the canonical colour extension.
2. Root-level retained datasets — contextual, copy/network, comparator, or frozen method layers that remain analytically useful but are not substitutes for canonical entities/witnesses.
3. `../archive/data_legacy_2026-08-30/` — superseded or quarantined discovery/legacy datasets retained only for provenance, recovery, or explicitly stated reopen conditions.

A manifest lifecycle value such as `active` describes the retained dataset's analytical role; it does **not** mean that the closed repository has an active generic research queue. Repository-level closure takes precedence over older operational wording.

Do not load archived legacy files alongside their canonical replacements unless performing a migration/provenance audit. Follow each row's `canonical_target`, `action`, and `reopen_rule` in `dataset_manifest.csv`.
