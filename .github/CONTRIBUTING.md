# Contributing to AI/Quality Sentinel

Thank you for your interest in contributing to **AI/Quality Sentinel**! We welcome contributions from the community to help us improve our proof of concept for AI-driven software quality analysis.

## Table of Contents

- [Getting Started](#getting-started)
- [Development Workflow](#development-workflow)
- [Commit Guidelines](#commit-guidelines)
- [Pull Request Process](#pull-request-process)
- [Code Standards](#code-standards)
- [Multilingual Documentation](#multilingual-documentation)

## Getting Started

1. **Fork the repository** on GitHub
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/YOUR_USERNAME/ai-quality-sentinel.git
   cd ai-quality-sentinel
   ```
3. **Create a feature branch**:
   ```bash
   git checkout -b feature/your-feature-name
   ```

## Development Workflow

### Before You Start

- Check existing [Issues](https://github.com/matheusvieira/ai-quality-sentinel/issues) and [Pull Requests](https://github.com/matheusvieira/ai-quality-sentinel/pulls) to avoid duplicate work
- Create or comment on an issue to discuss your changes before starting work
- For major changes, please open an issue first to discuss the proposal

### Making Changes

1. Keep your changes focused and logically separate
2. Follow the code standards outlined in this guide
3. Update documentation as needed (including all language versions)
4. Test your changes thoroughly

## Commit Guidelines

We follow the **Conventional Commits** specification. This ensures clear, structured commit history.

### Commit Message Format

```
type(scope): description

body

footer
```

### Type

Must be one of the following:
- `feat` - A new feature
- `fix` - A bug fix
- `docs` - Documentation changes
- `style` - Code style changes (formatting, etc.)
- `refactor` - Code refactoring without feature/bug changes
- `perf` - Performance improvements
- `test` - Adding or updating tests
- `build` - Build system or dependency changes
- `ci` - CI/CD configuration changes
- `chore` - Other changes (e.g., .gitignore)
- `revert` - Reverting a previous commit

### Scope

Optional but recommended. Examples: `parser`, `docs`, `ui`, `core`

### Description

- Use the **imperative mood** ("add" not "added" or "adds")
- **CRITICAL**: The header (type(scope): description) must be **50 characters or less**
- Start with a capital letter
- No period at the end

### Body

Required for most commits (except trivial changes like typos).
- Explain **WHAT** changed and **WHY**
- Wrap at 72 characters
- Separate from header with a blank line

### Footer

Optional. Use for:
- Breaking changes: `BREAKING CHANGE: description`
- Issue references: `Closes #123` or `Fixes #456`

### Examples

✅ Good:
```
feat(parser): add array parsing support

Implement recursive array parsing with support for nested structures.
This enables the analyzer to detect array-related quality issues.

Closes #42
```

✅ Good (simple):
```
docs: update README with setup instructions
```

❌ Bad (header too long):
```
refactor(copilot-instructions): reorganize and improve instructions
```

## Pull Request Process

1. **Update your branch** with the latest main:
   ```bash
   git fetch origin
   git rebase origin/main
   ```

2. **Push your changes** to your fork:
   ```bash
   git push origin feature/your-feature-name
   ```

3. **Create a Pull Request** on GitHub:
   - Use the provided PR template
   - Link related issues
   - Provide clear description of changes
   - Ensure CI checks pass

4. **Review Process**:
   - At least one maintainer review required
   - Address review comments promptly
   - Update your branch if needed (rebase or new commits)

5. **Merge**:
   - Squash and merge (preferred) or regular merge
   - Delete your feature branch after merge

## Code Standards

### General

- Keep code clean and readable
- Follow the existing code style in the project
- Add comments for complex logic
- Keep functions/methods focused and small

### Documentation

- Write clear commit messages
- Document public APIs and functions
- Include examples where helpful
- Update README if behavior changes

### Multilingual Content

- Documentation is maintained in three languages:
  - English (en-US)
  - Portuguese (pt-BR)
  - Spanish (es-ES)

## Multilingual Documentation

When updating documentation:

1. **Update the main README** (root-level) first
2. **Update all language folders**:
   - `en-US/README.md`
   - `pt-BR/README.md`
   - `es-ES/README.md`

3. **Include POC updates** in `POC/README.md` for each language

4. **Keep consistency**:
   - Same structure across all languages
   - Accurate translations
   - All updates in the same commit

### Translation Tips

- Use clear, professional language
- Maintain technical accuracy
- Preserve the original intent and tone
- Have native speakers review if possible

## Questions or Need Help?

- **Issues**: Use GitHub Issues for questions or feature requests
- **Discussions**: Check existing discussions for similar topics
- **Maintainers**: Tag maintainers in issues for urgent matters

## Recognition

Contributors will be recognized in:
- The project README
- Release notes
- GitHub's contributors page

Thank you for contributing! 🚀
