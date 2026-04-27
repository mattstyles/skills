---
name: git:q
description: Use when the user wants to quickly ship a small change, fix, or chore — creates a branch, commits, and opens a PR in one go
argument-hint: [description]
---

# Git Quick Ship Skill

Quickly create a branch, commit changes, and open a pull request in a single flow. Designed for small changes and fixes where a full manual workflow is overkill.

## Usage

`/git:q <description>` - Ship changes with the given description
`/git:q` - Analyze changes automatically

## Instructions

- If on `main`, run `/git:branch` to create a branch (use `$ARGUMENTS` to derive the name)
- Run `/git:commit` to stage, commit, and push changes
- Run `/git:pr` to open a pull request
- Ask the user if they want to merge once checks pass
  - If yes: watch with `gh pr checks <number> --watch`, then `gh pr merge <number> --merge --delete-branch`
  - If no: leave the PR open

## Arguments

- `$ARGUMENTS` - Optional description of the change (used across each skill invocation)
