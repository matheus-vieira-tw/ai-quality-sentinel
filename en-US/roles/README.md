# Team Roles (Hackathon Version) - AI/Quality Sentinel

This guide simplifies team structure for a hackathon with up to 3 people.
The goal is to accelerate decisions, reduce overhead, and focus on delivering value.

## Main Project Page

For the AI/Quality Sentinel overview (problem, solution, and goals), use:
- [Project README (en-US)](../README.md)

## Recommended Structure (up to 3 people)

In a hackathon, one person can take on more than one role. The distribution below works well to move the POC forward without a strict FE/BE split:

| Person | Main focus | Combined roles |
|---|---|---|
| Person 1 | Product and prioritization | Product Owner + Scrum Master |
| Person 2 | Development (generalist) | Core implementation + integrations |
| Person 3 | Development (generalist) | Core implementation + practical QA |

## Minimum Responsibilities by Workstream

### 1. Product and Prioritization
- Define the minimum hackathon scope (MVP).
- Prioritize backlog items by demo impact.
- Keep alignment between problem, solution, and final demo.

References:
- [Product Owner](product-owner.md)
- [Scrum Master](scrum-master.md)

### 2. Core Development (Person 2)
- Implement core services and business rules for the POC.
- Integrate required data and flows for the demo.
- Ensure end-to-end functionality for critical scenarios.

Reference:
- [Backend (.NET)](backend-dotnet.md)

### 3. Core Development + Quality (Person 3)
- Share core implementation with Person 2 (no fixed FE/BE boundary).
- Define and run a fast quality checklist for critical flows.
- Cover the essentials with tests (or a test script) to reduce demo risk.

References:
- [QA](qa.md)
- [Frontend (React/Angular)](frontend-react-angular.md)

## Contribution Map by Role

This section explains how each role can accelerate AI/Quality Sentinel in a hackathon context.

### Product Owner (PO)
- Translates the quality problem into clear MVP goals.
- Defines demo success criteria (what must work to show impact).
- Keeps focus on business value and avoids scope that will not be demonstrated.

Reference:
- [Product Owner](product-owner.md)

### Scrum Master (SM)
- Quickly removes blockers (dependencies, pending decisions, alignment issues).
- Organizes workflow to keep the team productive with low overhead.
- Maintains a short cadence for follow-up and plan adjustment.

Reference:
- [Scrum Master](scrum-master.md)

### Quality Assurance (QA)
- Defines a minimum quality checklist for the most critical flows.
- Validates whether MVP acceptance criteria are truly met.
- Helps reduce presentation risk with scenario-based validation.

Reference:
- [QA](qa.md)

### Backend Developer (.NET)
- Implements core services and business rules.
- Connects integrations needed to demonstrate the full cycle (intention -> execution -> standard).
- Establishes a technical foundation to scale the POC after the hackathon.

Reference:
- [Backend (.NET)](backend-dotnet.md)

### Frontend Developer (React/Angular)
- Builds a minimum experience to communicate value clearly.
- Translates technical outputs into understandable views for judges and stakeholders.
- Supports the demo narrative if there is time to evolve the interface.

Reference:
- [Frontend (React/Angular)](frontend-react-angular.md)

### Additional Specialists (when available)
- DevOps: speeds up setup, automation, and environment stability.
- Data: improves input quality and result interpretation.
- Security: reduces exposure risks and supports good practices from the POC stage.

Reference:
- [Additional Specialists](additional-specialists.md)

## Quick References for All Roles

- [Product Owner](product-owner.md)
- [Scrum Master](scrum-master.md)
- [QA](qa.md)
- [Backend (.NET)](backend-dotnet.md)
- [Frontend (React/Angular)](frontend-react-angular.md)
- [Additional Specialists](additional-specialists.md)

## Lightweight Working Rhythm (Suggestion)

- Short daily: 10 minutes to align blockers and next tasks.
- Technical checkpoint: 1 or 2 times per day to integrate frontend + backend.
- Final review: validate the demo script and fallback plan.

## What Not to Prioritize in the Hackathon

- Heavy ceremony processes.
- Broad test coverage outside critical flows.
- Large scope without demo-value validation.

## Interface in the Hackathon Context

- The interface can be minimal or even replaced by API/CLI flow in the first iteration.
- Prioritize first: business rules, integrations, and proof of value working.
- If time remains, evolve the interface to improve presentation storytelling.

## Current Team

- [Matheus Costa Vieira](mailto:matheus.vieira@thoughtworks.com) - Backend Development (.NET)

## Next Step

After validating this format in all language folders, keep future updates synchronized across en-US, pt-BR, and es-ES.
