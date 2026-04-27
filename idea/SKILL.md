---
name: idea
description: Capture a rough idea — the problem and a suggested solution — before it's ready for a full PRD. Use when the user has a half-formed thought, wants to jot down a concept, or says "I have an idea", "we should...", "what if we...".
argument-hint: "<description of the idea>"
---

# Idea

Capture an idea for: `$ARGUMENTS`

Ideas are low-friction and ephemeral. Their only purpose is to record a problem and a rough solution direction so it can later inform a PRD. Not every idea becomes reality — that's fine.

## How to capture

1. If `$ARGUMENTS` provides enough detail to fill both sections (problem and solution), write the file directly — no interview needed.

2. If the input is thin (just a title or single sentence), ask up to two sharpening questions:
   - What problem does this solve? Who's affected, what's broken or missing?
   - Do you have a rough solution in mind?

   Do NOT over-interview. If the user gives a short answer, that's fine — capture what they have.

3. Determine the next available number by checking existing files in `docs/ideas/`. Use the format `NNN` (zero-padded to 3 digits).

4. Write the file to `docs/ideas/NNN-slug.md` using the template at `${CLAUDE_SKILL_DIR}/references/template.md`. The slug should be short kebab-case derived from the idea.

5. Confirm the file was written and stop. Do NOT offer to start a PRD, invoke gorilla, or take any next step.

## Boundaries

- No codebase exploration — ideas are about the problem space, not the code
- No frontmatter, no metadata, no cross-references
- No beads creation
- No follow-on actions — write the file and stop
