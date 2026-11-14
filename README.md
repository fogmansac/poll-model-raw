# poll-model-raw

Immutable raw downloads for the poll-model project.

- Files are never edited after download.
- `MANIFEST.json` records the source URL, fetch date, SHA-256 and licence for each file.

## Attribution

- Silver Bulletin data: credit Nate Silver and/or Silver Bulletin.
- FiveThirtyEight (538) data: CC BY 4.0.
- Wikipedia-derived data: CC BY-SA.

## Removals from the otherwise immutable tree

The raw tree is otherwise immutable. CC-60 (2026-11-14) deliberately removed `electoral_vote/` (3 files) and `openelections/` (3 files) from the working tree: neither is read by anything in the project, `electoral_vote/` has no stated licence (treated as all rights reserved, and the same 2026 polls are held under CC BY 4.0 from `electionsusa/`), and `openelections/` held only repository metadata and a sample README. Their records moved to the `removed_files` array in `MANIFEST.json`. The files remain in this repo's git history; this is not a history rewrite.
