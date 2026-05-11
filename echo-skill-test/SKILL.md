---
name: echo-skill-test
description: Use this test skill to verify explicit skill invocation, prompt routing, minimal response formatting, and update detection. Trigger it when a user asks to smoke test a skill, echo a short input, confirm the active skill, or validate that skill instructions are being loaded.
---

# Echo Skill Test

## Workflow

When invoked, produce a compact response with:

1. `skill`: `echo-skill-test`
2. `input`: the user's relevant test text, shortened only if it is long
3. `status`: `loaded`
4. `mode`: `update-check`

If no test text is provided, set `input` to `none`.

## Constraints

- Do not add extra explanation unless the user asks for it.
- Preserve the user's wording for short test inputs.
- Keep the response suitable for automated smoke-test comparison.
