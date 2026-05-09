# Claude Code Instructions for FROID_NS

This repository uses FROID as the cold semantic record.

Do not read the full namespace unless explicitly asked. Prefer minimal context.

## Operating rules

1. Treat `namespace/` as the FROID cold record.
2. Treat committed FOLIOs as authoritative semantic context.
3. Do not infer global rules from isolated files.
4. When working on a NODE_ID or NODE_TAG, load only:
   - the selected FOLIO
   - its FLIO_REF
   - directly referenced rules
   - required vocabulary
   - the most recent ADR or BUG artifact if relevant
5. Stop walking links when a referenced rule is not active for the current task.
6. Report what was included and what was deliberately excluded.
7. Prefer creating candidate ADR/FOLIO notes for uncited implementation decisions.
8. Do not rewrite committed FOLIOs in place; propose supersession.

## Context loading

Default index:

`namespace/00-00-00.00-00-00.00-00-00.idx`

Before realizing code, compile a small context packet rather than reading the entire namespace.

## Working areas

`.claude/` is local working state and should not be treated as FROID source.