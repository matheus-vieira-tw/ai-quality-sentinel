# Proof of Concept (POC): The Context Bridge

## 1. POC Scope
The objective of the POC is to demonstrate that an AI can identify when code submitted via a Pull Request (PR) does not meet the acceptance criteria defined in a Jira task.

## 2. Test Scenario
- **Input A:** A Jira ticket (e.g. "Create login endpoint with 2FA validation").
- **Input B:** A code diff (e.g. code that creates login but omits 2FA).
- **Expected output:** An AI report stating: "Quality risk: the code implements login, but the 2FA logic mentioned in acceptance criterion 2 is missing."

## 3. Simplified Architecture
1. **Mock Data:** JSONs simulating Jira and GitHub APIs.
2. **LLM Prompting:** Use Few-Shot Prompting to teach the AI how to compare requirements against code.
3. **Interface:** A simple dashboard (Streamlit or static Markdown) comparing "Expected" vs. "Delivered".

## 4. Success Metrics for the POC
- Accuracy in identifying "Requirement Gaps" above 80%.
- Analysis time under 30 seconds per ticket/PR.

## Next Steps

- [Roadmap: Building the POC (Phase 1)](ROADMAP/README.md)
- [Roadmap: Scaling to Production (Phase 2+)](ROADMAP/after-poc-roadmap.md)