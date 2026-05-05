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
4. Construct your commit message using the following XML structure. Ensure the header (type(scope): description) is 50 characters or less.
5. If the message has body or footer, format it with blank lines: header\n\nbody\n\nfooter.
6. Present the generated commit message to the user and ask for explicit confirmation before proceeding.
7. Only after the user confirms, run the following command in your integrated terminal:

```bash
git commit -m "type(scope): description"
```

### Commit Message Structure

```xml
<commit-message>
	<type>feat|fix|docs|style|refactor|perf|test|build|ci|chore|revert</type>
	<scope>()</scope>
	<description>A short, imperative summary of the change</description>
	<body>(optional: more detailed explanation)</body>
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
	<body>Optional. Use for additional context. Separate from header with a blank line.</body>
	<footer>Use for breaking changes or issue references. Separate from body with a blank line.</footer>
</validation>
```

### Final Step

```xml
<final-step>
	<cmd>git commit -m "full commit message"</cmd>
	<note>Construct the full message with proper formatting: header\n\nbody\n\nfooter. Replace with your constructed message.</note>
</final-step>
```