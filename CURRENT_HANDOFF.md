# Current handoff

## Canonical state

**RESEARCH CLOSED — 2026-08-30.**

Read first:

1. [`FINAL_CLOSURE_2026-08-30.md`](FINAL_CLOSURE_2026-08-30.md)
2. [`CLOSURE_STATE_2026-08-30.json`](CLOSURE_STATE_2026-08-30.json)
3. [`docs/USER_ACTION_LOG.md`](docs/USER_ACTION_LOG.md)
4. [`docs/WINCKELMANN_1664_DIRECT_RASTER_MATRIX_STATE_CLOSURE_P142_P168_P179_2026-08-30.md`](docs/WINCKELMANN_1664_DIRECT_RASTER_MATRIX_STATE_CLOSURE_P142_P168_P179_2026-08-30.md)
5. [`docs/WINCKELMANN_1684_HORN_CARRIER_FIREWALL_AND_DIRECT_IMAGE_BOUNDARY_2026-08-30.md`](docs/WINCKELMANN_1684_HORN_CARRIER_FIREWALL_AND_DIRECT_IMAGE_BOUNDARY_2026-08-30.md)

Older dated checkpoints remain research provenance. If an older `CURRENT`, `Priority`, `OPEN`, `next round`, or handoff instruction conflicts with the files above, this closure state controls.

## Current operational status

- **Research programme:** CLOSED.
- **Public-web discovery:** CLOSED.
- **Generic expansion:** STOP.
- **Active blocking user actions:** NONE.
- **Logged user actions:** UA-001 DONE; UA-002 DONE.
- **Canonical core research queue:** FROZEN.
- **Canonical colour research queue:** FROZEN.
- **Archive/direct-object residuals:** bounded, dormant, source-triggered only.
- **Stale discovery PRs:** none should remain open; historical branches may remain as provenance.

No further broad research round is justified by the current evidence state.

## Priority 1 — Winckelmann 1664 / Staden: CLOSED

The former `UA-001` raster task is complete.

Key correction:

**1664 p.168 is not the 1557 Ubatuba / `uwatibi` plate.** The correct source is the 1557 Igarassu battle plate:

`[Combate entre portugueses e índios caetés em Igarassu]`, Brasiliana / BBM ID `45000008047.28`.

Direct-raster result:

- p.168 → `same_matrix_as_1557 = HIGH_CONFIDENCE_DIRECT_RASTER`;
- p.179 → `same_matrix_as_1557 = HIGH_CONFIDENCE_DIRECT_RASTER`;
- selective lettering-state differences are directly observed in both cases;
- exact physical mechanism remains unspecified;
- p.142 direct 1664 raster is controlled as positive control.

Do **not** restore a bulk `32 same matrices` claim from these two pairwise promotions.

The Münster second copy is only an optional confirmatory state test.

## Priority 3 — Winckelmann 1684 Oldenburg Horn: CLOSED AT CARRIER LIMIT

The former `UA-002` full-scan task is complete.

Direct scan result:

- digital PDF pp.25–27 are the main Wunderhorn foldout sequence;
- the fully opened image at PDF p.26 is explicitly labelled `Nach dem Originalholzschnitt durchgezeichnet von Fr. Schohusen 1912.`;
- therefore the principal Horn image in the digitized `GE IX B 70 A` copy is a **1912 tracing after the original woodcut**, not an original 1684 impression;
- no genuine 1684 main Wunderhorn impression survives in this digitized carrier;
- other historical image apparatus in the volume does not repair that absence.

Comparison result:

- Jacobaeus 1696 Tab. XVI shows strong broad concordance with the traced 1684 visual tradition;
- `1696 derived_from 1684 print` remains **strong scholarly reported / not directly proven** because the available 1684 image is second-order and Jacobaeus also had object access;
- the reported heraldic discrepancy remains controlled at scholarly/transmission level, but this specific carrier cannot establish it by direct observation of an extant 1684 main-Horn impression.

No further user action is required. Reopen only if another 1684 copy preserving the original main Wunderhorn woodcut, or another securely dated seventeenth-century production witness, appears for a load-bearing claim.

## Other Winckelmann modules

Closed modules:

- p.136 provenance + pp.18/74 source models: [`docs/WINCKELMANN_1664_P136_PROVENANCE_AND_P18_P74_SOURCE_MODEL_CLOSURE_2026-08-30.md`](docs/WINCKELMANN_1664_P136_PROVENANCE_AND_P18_P74_SOURCE_MODEL_CLOSURE_2026-08-30.md)
- 1671 two maps / cartographic ancestry: [`docs/WINCKELMANN_1671_TWO_MAPS_AND_CARTOGRAPHIC_SOURCE_ANCESTRY_CLOSURE_2026-08-30.md`](docs/WINCKELMANN_1671_TWO_MAPS_AND_CARTOGRAPHIC_SOURCE_ANCESTRY_CLOSURE_2026-08-30.md)
- 1684 Horn carrier audit: [`docs/WINCKELMANN_1684_HORN_CARRIER_FIREWALL_AND_DIRECT_IMAGE_BOUNDARY_2026-08-30.md`](docs/WINCKELMANN_1684_HORN_CARRIER_FIREWALL_AND_DIRECT_IMAGE_BOUNDARY_2026-08-30.md)
- Hessian planned visual apparatus: [`docs/WINCKELMANN_HESSIAN_PLANNED_VISUAL_APPARATUS_SOURCE_BOUNDARY_CLOSURE_2026-08-30.md`](docs/WINCKELMANN_HESSIAN_PLANNED_VISUAL_APPARATUS_SOURCE_BOUNDARY_CLOSURE_2026-08-30.md)
- 1754 p.377 / Bernhard source boundary: [`docs/WINCKELMANN_1754_P377_DIRECT_OBJECT_SOURCE_BOUNDARY_CLOSURE_2026-08-30.md`](docs/WINCKELMANN_1754_P377_DIRECT_OBJECT_SOURCE_BOUNDARY_CLOSURE_2026-08-30.md)
- Marburg `Ms.309`: [`docs/WINCKELMANN_MARBURG_MS309_OPEN_WEB_CLOSURE_AND_ARCHIVE_ONLY_STATUS_2026-08-30.md`](docs/WINCKELMANN_MARBURG_MS309_OPEN_WEB_CLOSURE_AND_ARCHIVE_ONLY_STATUS_2026-08-30.md)

## Canonical lifecycle rule

`data/canonical/research_questions.jsonl` and `data/canonical/colour_research_questions.jsonl` are frozen.

This does not turn unresolved/probable claims into established facts. It means their remaining tests are bounded object/archive/copy refinements rather than current discovery obligations.

`unresolved assertion ≠ active research obligation`.

## Dormant archive/library upgrades

Reopen only when the actual source or a load-bearing writing need appears:

- Münster ULB 1664 p.168 / p.179 second-copy state confirmation;
- LB Oldenburg `Cim I 204`, ff.543r–552v;
- UB Marburg `Ms.309`, Kalliope `DE-611-HS-3888458`;
- 1754 sixth part pp.376–378 if a direct seam check is required;
- direct Bernhard/Winkelmann manuscript alignment;
- another 1684 Horn copy preserving the original main woodcut, if one appears and the claim becomes load-bearing.

## Restart rule

For any future chat:

`先读 FINAL_CLOSURE_2026-08-30.md、CLOSURE_STATE_2026-08-30.json 和 docs/USER_ACTION_LOG.md。frontispieces 当前状态为 CLOSED。UA-001、UA-002 均已完成。只有新的直接图像/实物、已锁定档案材料、会改变论证的一手材料、或写作时暴露出的 load-bearing source gap 才允许重开具体分支；不要恢复旧 Priority queue 或 generic web sweep。`
