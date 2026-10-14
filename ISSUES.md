

## Needs input (Auto Continue)
*Left by Auto Continue 2026-10-14 — decide these, then clear CONSIDERATIONS.md.*
- **Merge `main` into `pr-186`: which decompilation wins?** Main's #222–#225/#228 re-decompile functions this branch already has (94 conflict hunks over 8 files; `5BF94.c` alone has 49), and this branch split `6E644.c` into hasm + `6F014.c`. Merge aborted. See `.atelier/views/merge-main-conflicts.html`. Pick: (a) keep pr-186's versions, (b) prefer main's per function, or (c) don't merge. Retried 2026-10-14 with (a): it fails to compile, because main's auto-merged shared headers retype structs this branch uses elsewhere (`func_8006CE70_t`→`SVECTOR`, `func_800CF0E8_t`→`actionEffectRequest`, `vs_action_t.flagsE`, actor `unk16C`/`unk12C`), with errors in `30DB0.c`, `40564.c` and `44F14.c`. So (a) also needs a type-model choice.
