# Current handoff

Current research-state closure:

[`docs/ROUND_CLOSURE_AND_HANDOFF_WINCKELMANN_TEXTUAL_VISUAL_PRODUCTION_2026-08-28_1626.md`](docs/ROUND_CLOSURE_AND_HANDOFF_WINCKELMANN_TEXTUAL_VISUAL_PRODUCTION_2026-08-28_1626.md)

Priority 1 is now **in progress**. First pairwise-control batch:

[`docs/WINCKELMANN_1664_STADEN_PAIRWISE_CONCORDANCE_BATCH1_P142_P168_P179_2026-08-28.md`](docs/WINCKELMANN_1664_STADEN_PAIRWISE_CONCORDANCE_BATCH1_P142_P168_P179_2026-08-28.md)

Companion data:

[`data/winckelmann_1664_staden_pairwise_matrix_control_batch1_2026-08-28.csv`](data/winckelmann_1664_staden_pairwise_matrix_control_batch1_2026-08-28.csv)

Resume from direct 1664 raster recovery for **p.168 and p.179**, using the now-identified JCB/Internet Archive, GDZ `PPN829199152`, and Münster `urn:nbn:de:hbz:6:1-15914` routes; use p.142 as a positive-control overlay. After these three, expand the same protocol to pp.140, 143, 144, 155, 157 and 158.

Important current guardrail: do **not** restore the earlier bulk claim that all 32 Staden-section images in Winckelmann 1664 are verified impressions from the same 1557 matrices. The repository now treats the JCB bulk attribution as conflicted by Obermeier's `some / portion` reconstruction and requires item-level matrix comparison. Batch 1 has **not** promoted any new `same_matrix` identity.

Current diagnostic gains:

- p.142: JCB item-level record controls 1664 image dimensions `10.5 × 10.8 cm` and gives an original-woodcut catalogue attribution; direct defect concordance still pending.
- p.168: the 1557 Ubatuba source image visibly carries `uwatibi`; JCB/IA reports names eliminated in 1664; matrix identity and removal mechanism remain open.
- p.179: the 1557 shipwreck source visibly carries multiple geographic labels, including `S. vin` and `S. maro`; JCB/IA reports names eliminated in 1664; matrix identity and removal mechanism remain open.

User-action rule: anything that genuinely requires the user's direct intervention must be logged centrally in [`docs/USER_ACTION_LOG.md`](docs/USER_ACTION_LOG.md). Do not scatter such requests across chat or research notes, and do not escalate an item to the user before normal assistant-side retrieval routes have been exhausted.

Short restart instruction for a new chat:

`继续 frontispieces repo。先读 CURRENT_HANDOFF.md，再读它指向的 Batch 1 checkpoint；从 p.168/p.179 的 1664 direct raster recovery 继续，以 p.142 为 positive control；维持 32-fold same-matrix guardrail；进度随时同步 main；需要用户亲自处理的事项统一记入 docs/USER_ACTION_LOG.md。`
