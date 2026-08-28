# Current handoff

Current research-state closure:

[`docs/ROUND_CLOSURE_AND_HANDOFF_WINCKELMANN_TEXTUAL_VISUAL_PRODUCTION_2026-08-28_1626.md`](docs/ROUND_CLOSURE_AND_HANDOFF_WINCKELMANN_TEXTUAL_VISUAL_PRODUCTION_2026-08-28_1626.md)

Priority 1 is **in progress**. Completed current-turn checkpoints:

1. [`docs/WINCKELMANN_1664_STADEN_PAIRWISE_CONCORDANCE_BATCH1_P142_P168_P179_2026-08-28.md`](docs/WINCKELMANN_1664_STADEN_PAIRWISE_CONCORDANCE_BATCH1_P142_P168_P179_2026-08-28.md)
   - companion data: [`data/winckelmann_1664_staden_pairwise_matrix_control_batch1_2026-08-28.csv`](data/winckelmann_1664_staden_pairwise_matrix_control_batch1_2026-08-28.csv)
2. [`docs/WINCKELMANN_1664_STADEN_PAIRWISE_SOURCE_CONTROL_BATCH2_P140_P143_P144_P155_P157_P158_2026-08-28.md`](docs/WINCKELMANN_1664_STADEN_PAIRWISE_SOURCE_CONTROL_BATCH2_P140_P143_P144_P155_P157_P158_2026-08-28.md)
   - companion data: [`data/winckelmann_1664_staden_pairwise_source_control_batch2_2026-08-28.csv`](data/winckelmann_1664_staden_pairwise_source_control_batch2_2026-08-28.csv)

Resume from direct 1664 raster recovery for **p.168 and p.179**, using the now-identified JCB/Internet Archive, GDZ `PPN829199152`, and Münster `urn:nbn:de:hbz:6:1-15914` routes; use p.142 as a positive-control overlay. GDZ platform-level research confirms its digitized works expose IIIF manifests, but the target manifest has not yet been recovered through the current fetch layer. This remains an assistant-side retrieval problem, not a user-action item.

If raster recovery remains blocked, continue source-side resolution for the remaining seed rows while preserving the same evidence hierarchy. Six further source-side rows are now tied to specific 1557 Brasiliana/BBM records:

- p.140 → `Aldeia tupinambá fortificada`, ID `45.000.008.047.136`;
- p.143 → `Mulheres tupinambá fabricando cauim`, ID `45.000.008.047.146`;
- p.144 → `Dança ao redor da ibirapema`, ID `45.000.008.047.166`;
- p.155 → `Execução do cativo`, ID `45.000.008.047.168`;
- p.157 → `Esquartejamento do corpo do cativo executado`, ID `45.000.008.047.169`;
- p.158 → `Mulheres e crianças tupinambás se alimentando das vísceras do cativo executado`, ID `45.000.008.047.170`.

Important current guardrail: do **not** restore the earlier bulk claim that all 32 Staden-section images in Winckelmann 1664 are verified impressions from the same 1557 matrices. The repository treats the JCB bulk attribution as conflicted by Obermeier's `some / portion` reconstruction and requires item-level matrix comparison. Neither Batch 1 nor Batch 2 has promoted any new `same_matrix` identity.

Current diagnostic gains from Batch 1:

- p.142: JCB item-level record controls 1664 image dimensions `10.5 × 10.8 cm` and gives an original-woodcut catalogue attribution; direct defect concordance still pending.
- p.168: the 1557 Ubatuba source image visibly carries `uwatibi`; JCB/IA reports names eliminated in 1664; matrix identity and removal mechanism remain open.
- p.179: the 1557 shipwreck source visibly carries multiple geographic labels, including `S. vin` and `S. maro`; JCB/IA reports names eliminated in 1664; matrix identity and removal mechanism remain open.

User-action rule: anything that genuinely requires the user's direct intervention must be logged centrally in [`docs/USER_ACTION_LOG.md`](docs/USER_ACTION_LOG.md). Do not scatter such requests across chat or research notes, and do not escalate an item to the user before normal assistant-side retrieval routes have been exhausted.

Short restart instruction for a new chat:

`继续 frontispieces repo。先读 CURRENT_HANDOFF.md，再读它指向的 Batch 1/Batch 2 checkpoints；优先继续 p.168/p.179 的 1664 direct raster recovery，以 p.142 为 positive control；若 raster 路径继续受阻，就继续把剩余 seed rows 锁到具体 1557 source records；维持 32-fold same-matrix guardrail；进度随时同步 main；需要用户亲自处理的事项统一记入 docs/USER_ACTION_LOG.md。`
