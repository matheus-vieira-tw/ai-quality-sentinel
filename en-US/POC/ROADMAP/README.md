# Roadmap: Building the POC (Phase 1)

## Setup & Design (Day 1-2)
- [ ] **Persona Definition:** Create the profile of the "Detailed Reviewer" (the AI voice).
- [ ] **Test Dataset:** Select 5 anonymized real examples of good/bad tickets and matching code.
- [ ] **Model Choice:** Configure access to the model via AI/works™ (or GPT-4/Claude for initial testing).

## Development (Day 3-5)
- [ ] **Extraction Module:** Script to read ticket text (Markdown/JSON).
- [ ] **Code Analysis Module:** Script to process `.diff` or `.py/.js` files.
- [ ] **Prompt Engineering:** Create the system prompt that instructs the AI to be a rigorous quality auditor.
- [ ] **Output Validation:** Create a response template (e.g. Quality Traffic Light - Green/Yellow/Red).

## Demonstration (Day 6-7)
- [ ] **Video Recording:** Demo comparing a quick human review with the AI's deeper analysis.
- [ ] **Results Documentation:** Table of "Before vs After" using the tool.
