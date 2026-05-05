---
applyTo: "**"
description: "When user asks to commit, use the commit-workflow skill and confirm required points with ask tool before committing."
---

# Commit Request Workflow

When the user asks to create a commit:

1. Load and follow `.github/skills/commit-workflow/SKILL.md`.
2. **MANDATORY: Count the ENTIRE header character-by-character. The sum of type(scope): description must be ≤ 50 chars. Reject and revise if longer.**
3. **MANDATORY: Include a body explaining WHAT changed and WHY (required for most commits, except trivial fixes).**
4. Use ask tool to confirm required points before committing.
5. Respect conventional commit format with proper blank lines for multi-line messages.
6. Do not commit without explicit user confirmation.
