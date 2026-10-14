# Issues — rood-reverse

## Open

## Resolved
- [x] **Merge `main` into `pr-186`: which decompilation wins?** — Merged per decision (b): main's version wherever main decompiled a function (incl. its 10 `6E644` functions ported into this branch's split units), this branch's 28 extra functions kept and adapted to main's types; shared structs reconciled field by field, keeping the finer layout where only one side's code relied on it. `make remake`: ✔ All files match. pr-186 is well ahead of main (95 `INCLUDE_ASM` left vs main's 987). *(resolved 2026-10-14)*
