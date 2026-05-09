# Agent Instructions for FROID_NS

FROID_NS is a self-hosting namespace. Use FROID context selectively.

## Minimal-context policy

Do not load all files by default. For any task, identify:

- target NODE_ID / NODE_TAG
- task type: inspect, validate, realize, document, migrate
- active mode
- realization surface, if any
- required dependencies

Then load only the active context.

## Authority

FOLIO records are semantic source of truth. Realized code, prose, tests, and generated artifacts are outputs that should cite or trace back to FOLIO rules where possible.

## Change policy

Do not mutate committed FOLIO semantics silently.

For semantic changes:
1. describe the issue
2. identify affected FOLIOs
3. propose ADR/BUG/candidate supersession
4. wait for user confirmation before writing authoritative changes

## Preferred behavior

When generating artifacts:
- cite governing FOLIO rules when possible
- mark uncited realization decisions
- list assumptions
- keep output minimal and bounded to the selected task