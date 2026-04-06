# OctoAcme Project Management Overview

<!-- Related to: #6 -->

## Purpose
Provide a concise, shareable introduction to how OctoAcme runs projects so new teammates can quickly understand our approach, roles, and key artifacts.

## Scope
Applies to all cross-functional projects that deliver product features, services, or integrations.

## Principles
- Customer-first: prioritize customer value and usability.
- Iterative delivery: deliver small, testable increments.
- Clear ownership: each project has a named Project Manager (PM) and Product Lead.
- Data-informed decisions: measure impact and iterate based on evidence.
- Psychological safety: encourage feedback and learning.

## Core Roles
- **Project Manager (PM)**: coordinates delivery, schedules, risk, and communications.
- **Product Manager (PdM)**: defines outcomes, prioritizes backlog, and measures success.
- **Developers**: implement features, collaborate on design and testability.
- **QA/Testing**: validate quality and acceptance criteria.
- **Stakeholders**: provide inputs and approvals.
- **QA Lead**: owns the test strategy, coordinates QA efforts, and provides release readiness sign-off.
- **UX/UI Designer**: ensures intuitive, accessible designs and collaborates with PdM and Developers on user stories.
- **Technical Writer**: produces and maintains documentation for features, processes, and APIs.
- **Release Manager**: coordinates release windows, deployment activities, and go/no-go decisions.
- **Support Lead**: manages support escalations, surfaces customer feedback, and liaises with delivery teams.

> **Note:** Expanding Core Roles to include QA Lead, UX/UI Designer, Technical Writer, Release Manager, and Support Lead improves clarity of ownership during handoffs, reduces ambiguity at key transitions (development → QA → release → support), and ensures accountability is distributed across the full delivery lifecycle. See [octoacme-roles-and-personas.md](octoacme-roles-and-personas.md) for full role definitions.

## Key Artifacts
- Project Charter / One-pager
- Roadmap and Release Plan
- Sprint/Iteration Backlog
- Acceptance Criteria & Definition of Done
- Risk Register
- Retrospective notes and action items

## Lifecycle (high-level)
1. Initiation: problem statement, stakeholders, high-level timeline.
2. Planning: scope, resources, milestones, dependencies.
3. Execution: build, test, review, iterate.
4. Release: deploy, verify, announce.
5. Close & Retrospective: capture learnings and next steps.

## Communication Cadence
- Weekly sync between PM + PdM
- Twice-weekly standups for delivery team (or as agreed)
- Monthly stakeholder updates
- Ad-hoc escalations as needed

## How to use these docs
- Keep the Project Charter updated in the project repo.
- Add process-specific docs into `.copilot/` if you want Copilot Spaces to use them as context.
