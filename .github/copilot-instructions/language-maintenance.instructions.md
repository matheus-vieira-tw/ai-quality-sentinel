---
applyTo: "**"
description: "Instructions for maintaining multilingual documentation folders (en-US, pt-BR, es-ES). Use when updating or adding content to language-specific folders."
---

# Language Folder Maintenance

## Overview
This project maintains documentation in multiple languages: English (en-US), Portuguese (pt-BR), and Spanish (es-ES). Each language has its own folder with README.md and POC/ subfolder.

## Guidelines
- When updating content in one language folder, ensure equivalent updates are made in the other language folders to maintain consistency.
- Use the main README.md in the root as the source of truth for project description.
- For POC-specific changes, update the POC/README.md in each language folder accordingly.
- If adding new features or sections, translate and add them to all language folders.
- Commit changes to all affected language folders in the same commit to keep them synchronized.

## Structure
- en-US/: English documentation
- pt-BR/: Portuguese documentation
- es-ES/: Spanish documentation

Each folder contains:
- README.md: Main project overview
- POC/README.md: Proof of Concept details
- ROADMAP/: Roadmap files