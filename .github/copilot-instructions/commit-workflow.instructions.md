---
applyTo: "**"
description: "When user asks to commit, use the commit-workflow skill and confirm required points with ask tool before committing."
---

# Commit Request Workflow

When the user asks to create a commit, follow the numbered steps below in order and stop at the first failed check.

## Step 1: Validate Skill File

1. **Load and follow `.github/skills/commit-workflow/SKILL.md`.**
	- If the file is missing, invalid, partially corrupted, or contains unexpected content, notify the user with the specific issue, request clarification only if the issue is unclear, and abort the commit process immediately.

## Step 2: Validate Commit Message

2. **MANDATORY: Validate the commit header and body together.** The header must use `type(scope): description` and stay at 50 characters or fewer; the body must explain what changed and why in 1-2 sentences unless the commit is a minor typo or formatting fix.
	- If the header exceeds 50 characters, provide an error message and suggest a revised version before proceeding.
	- If the commit body is empty or invalid, prompt the user to provide a brief 1-2 sentence explanation before proceeding.

## Step 3: Confirm with Ask Tool

3. Use the ask tool to validate the correctness of the following required points: type, scope, description, and body. Ensure each point meets the criteria in step 2 before committing.
	- If the ask tool cannot retrieve required points or the user input is invalid, prompt the user to provide the missing information.
	- If the ask tool returns incomplete data or data that does not meet the criteria in step 2, clarify the missing or incorrect fields with the user before proceeding.
	- If the ask tool provides contradictory data for the required points, notify the user and request clarification.
	- If the ask tool encounters a technical failure, such as a timeout or inability to retrieve data, notify the user of the specific issue and abort the commit process.
	- If the user provides partial input, validate the provided fields and prompt for the missing ones.
	- If the user provides invalid input three times while supplying missing information, abort the commit process and notify the user.

## Step 4: Confirm Formatting

4. Confirm formatting compliance: Use conventional commits in the form `type(scope): description`. Ensure a blank line appears before the body only when the commit message has a multi-line body. If the commit message is valid but incorrectly formatted, notify the user and request a reformatted commit message. Example: `feat(api): add commit validation`.

## Step 5: Confirm User Approval

5. Obtain explicit user confirmation before proceeding with the commit.
6. If the user provides a valid commit message but refuses to confirm, notify the user that confirmation is required and abort the process.
7. If the user refuses to provide the missing information or fails to confirm, abort the commit process and notify the user.
8. Do not commit unless all prior validation steps pass and explicit user confirmation is received.
