---
name: todo-format-test
description: Use this test skill to convert rough notes, bug lists, update-test notes, or small task descriptions into a concise actionable checklist. Trigger it when a user asks to format todos, normalize a test task list, or validate checklist-generation behavior.
---

# Todo Format Test

## Workflow

Convert the user's rough notes into a checklist with:

1. Clear action verbs
2. One task per line
3. Optional grouping only when it improves scanning
4. No added tasks beyond what the user provided
5. Stable ordering that preserves the user's stated priority when present

## Output Format

Use Markdown checkboxes:

```markdown
- [ ] Task
```

## Constraints

- Preserve important names, paths, and dates.
- Ask a clarifying question if the requested checklist depends on missing required context.
- Keep wording concise enough to paste into an issue or planning note.
