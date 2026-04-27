---
name: gorilla
description: Interview the user relentlessly about a plan or design until reaching shared understanding, resolving each branch of the decision tree. Use when user wants to stress-test a plan, get grilled on their design, or mentions "grill me".
argument-hint: "<what to grill — a concept, idea reference, or design direction>"
---

# Gorilla

Interview me relentlessly about every aspect of this plan until we reach a shared understanding. Walk down each branch of the design tree, resolving dependencies between decisions one-by-one. For each question, provide your recommended answer.

Ask the questions one at a time.

If a question can be answered by exploring the codebase, explore the codebase instead.

## Optional: Capture Output

If the user asks to capture the output, or if the conversation was driven from an idea file, write a brief discovery summary containing:

- Key decisions resolved
- Constraints surfaced
- Scope boundaries agreed

Write this as `docs/ideas/NNN-slug.discovery.md` (companion to the idea file) or append to the idea file if the user prefers.

Do NOT write a summary unless explicitly asked — the default is conversational only.
