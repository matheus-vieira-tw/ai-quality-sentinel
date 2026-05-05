---
name: commit-workflow
description: 'Prompt and workflow for generating conventional commit messages using a structured XML format. Guides users to create standardized, descriptive commit messages in line with the Conventional Commits specification, including instructions, examples, and validation.'
---

### Instructions

```xml
	<description>This file contains a prompt template for generating conventional commit messages. It provides instructions, examples, and formatting guidelines to help users write standardized, descriptive commit messages in accordance with the Conventional Commits specification.</description>
```

### Workflow

**Follow these steps:**

1. Run `git status` to review changed files.
2. Run `git diff` or `git diff --cached` to inspect changes.
3. Stage your changes with `git add <file>`.
4. Construct your commit message using the following XML structure. 
   - **CRITICAL: The ENTIRE header (type(scope): description) must be 50 characters or less, including all spaces and punctuation.**
   - Count every character: `t-y-p-e-(-s-c-o-p-e-)-:- -d-e-s-c-r-i-p-t-i-o-n`
5. Validate the header length BEFORE presenting it. If over 50 chars, shorten the description or remove the scope.
6. If the message has body or footer, format it with blank lines: header\n\nbody\n\nfooter.
7. Present the generated commit message to the user and ask for explicit confirmation before proceeding.
8. Only after the user confirms, run the following command in your integrated terminal:

```bash
git commit -m "type(scope): description"
```

**Header Length Examples (50 char max):**
- ✅ `feat(parser): add array parsing` = 31 chars
- ✅ `refactor(core): reorganize logic` = 32 chars
- ❌ `refactor(copilot-instructions): reorganize and improve instructions` = 67 chars (TOO LONG)
- ✅ `refactor(copilot): improve workflow` = 34 chars (shortened version)

### Commit Message Structure

```xml
<commit-message>
	<type>feat|fix|docs|style|refactor|perf|test|build|ci|chore|revert</type>
	<scope>()</scope>
	<description>A short, imperative summary of the change</description>
	<body>required: Explain WHAT changed and WHY (unless it's a trivial docs/style fix)</body>
	<footer>(optional: e.g. BREAKING CHANGE: details, or issue references)</footer>
</commit-message>
```

### Examples

```xml
<examples>
	<example>feat(parser): add ability to parse arrays</example>
	<example>fix(ui): correct button alignment</example>
	<example>docs: update README with usage instructions</example>
	<example>refactor: improve performance of data processing</example>
	<example>chore: update dependencies</example>
	<example>feat!: enable email on signup</example>
</examples>
```

### Validation

```xml
<validation>
	<type>Must be one of the allowed types. See <reference>https://www.conventionalcommits.org/en/v1.0.0/#specification</reference></type>
	<scope>Optional, but recommended for clarity.</scope>
	<description>Required. Use the imperative mood (e.g., "add", not "added").</description>
	<header>The header (type(scope): description) must be 50 characters or less.</header>
	<body>Required for most commits. Explain WHAT changed and WHY. Only skip for trivial fixes (typos, formatting).</body>
	<footer>Optional. Use for breaking changes or issue references. Separate from body with a blank line.</footer>
</validation>
```

### Final Step

```xml
<final-step>
	<cmd>git commit -m "full commit message"</cmd>
	<note>Construct the full message with proper formatting: header\n\nbody\n\nfooter. Replace with your constructed message.</note>
</final-step>
```