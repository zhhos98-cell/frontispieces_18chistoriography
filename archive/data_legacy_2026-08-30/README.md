# Legacy and quarantined data — 2026-08-30

This directory contains data files removed from the active `data/` layer during frozen-repository cleanup.

Selection rule: only files whose `data/dataset_manifest.csv` lifecycle state was already `superseded` or `quarantined` were moved here. No canonical, active, or frozen contextual dataset was removed.

Superseded files have an explicit canonical replacement or were merged into canonical records. Quarantined files are discovery, locator, experimental, or volatile web layers that should not be loaded as historical evidence without renewed source-specific promotion.

The files remain unchanged at blob level; only their repository paths changed. Git history preserves all prior locations.
