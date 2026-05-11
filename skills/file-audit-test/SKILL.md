---
name: file-audit-test
description: Use this test skill to perform a lightweight audit of one or more files or directories. Trigger it when a user asks to inspect test fixtures, summarize local project files, check file organization, or verify that file-reading workflows are working.
---

# File Audit Test

## Workflow

1. Identify the file or directory scope from the user request.
2. Read only the files needed to answer the request.
3. Report the result as:
   - `scope`: inspected path or pattern
   - `files`: count or short list of relevant files
   - `notes`: concise observations

## Audit Focus

- Missing expected files
- Obvious naming or placement issues
- Empty files or stub-only content
- Basic structure mismatches

## Constraints

- Do not make edits unless the user explicitly asks.
- Do not include unrelated files in the report.
- Keep findings factual and directly tied to inspected paths.
