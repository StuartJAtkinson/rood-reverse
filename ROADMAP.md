# Roadmap — rood-reverse

- [ ] **Raise the "fully linked" % shown in the README badges.** Next focus after the main merge (decided 2026-10-14). pr-186 decompiles far more than main (95 `INCLUDE_ASM` left vs 987) but keeps 57 hand-written asm (`hasm`) units vs main's 14; converting those to matching C is the likely lever for linked bytes.
