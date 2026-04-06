> Related to: #6

# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## QA Lead

### Role Summary
The QA Lead owns test strategy, coordinating manual and automated testing efforts to ensure features meet acceptance criteria and quality standards prior to release.

### Responsibilities
- Define and maintain the overall QA strategy for a project
- Create and review test plans and test cases
- Coordinate automated test coverage and manual testing activities
- Triage and communicate test failures and risks
- Report testing status and quality metrics to PM and PdM

### Goals
- Minimize production defects and regressions
- Ensure acceptance criteria are testable and verified
- Accelerate feedback loops between development and QA

### Typical Communication
- Test plans and summaries in project docs
- QA status updates in weekly delivery syncs
- CI test results and issue triage in PRs and issue trackers

### Interaction with existing roles
- PM: Receives release timelines and communicates testing risks/needs
- PdM: Confirms acceptance criteria and validates user-facing quality
- Developers: Coordinates on testability, reproductions, and fixes
- Stakeholders: Provides high-level QA readiness updates

---

## UX/UI Designer

### Role Summary
The UX/UI Designer drives user-centered design, ensuring features are usable, accessible, and aligned with product goals.

### Responsibilities
- Create and iterate on wireframes, mockups, and prototypes
- Collaborate with PdM and developers to define acceptance criteria tied to UX
- Conduct usability testing and accessibility reviews
- Maintain design system artifacts and component guidance

### Goals
- Deliver intuitive, accessible user experiences
- Reduce rework due to unclear or untested UX assumptions
- Ensure design consistency across the product

### Typical Communication
- Design artifacts (Figma links, mockups) in design tickets
- UX findings in planning and demo meetings
- Accessibility notes in PRs or QA handoffs

### Interaction with existing roles
- PM/PdM: Aligns on scope, priorities, and user needs
- Developers: Provides assets, acceptance criteria, and clarifications
- QA Lead: Provides UX-focused test cases and acceptance criteria
- Stakeholders: Shares design rationale and usability outcomes

---

## Technical Writer

### Role Summary
The Technical Writer produces user-facing and internal documentation that clarifies feature behavior, runbooks, and onboarding materials.

### Responsibilities
- Draft and maintain release notes, user guides, and internal runbooks
- Collaborate with PdM, Developers, and Support to ensure accuracy
- Create or update API docs and examples when needed
- Ensure documentation is accessible and discoverable in repo

### Goals
- Reduce support load by providing clear documentation
- Improve onboarding and knowledge transfer for new team members
- Preserve institutional knowledge in accessible formats

### Typical Communication
- Doc PRs and review comments
- Coordination during release planning and handoffs
- Updates to docs/ or external help sites

### Interaction with existing roles
- PM/PdM: Receives feature intent and acceptance criteria for accurate docs
- Developers: Gathers technical details and examples
- Support Lead: Incorporates known FAQs and support notes
- Stakeholders: Validates customer-facing messaging when needed

---

## Release Manager

### Role Summary
The Release Manager coordinates release preparation, deployment cadence, and post-release verification to ensure smooth deliveries.

### Responsibilities
- Maintain the release schedule and deployment checklist
- Coordinate cross-team readiness (QA, Ops, Support)
- Approve release readiness and trigger deployments as per policy
- Lead post-deploy verification and rollback if necessary

### Goals
- Reduce release failures and rollbacks
- Ensure predictable, low-risk deployments
- Maintain clear communication of release status to stakeholders

### Typical Communication
- Release notes and readiness status in project docs
- Deployment notifications to stakeholders and support channels
- Post-release verification reports

### Interaction with existing roles
- PM: Aligns on release timing and scope
- QA Lead: Confirms test coverage and readiness
- Developers: Ensures code and CI pipelines are release-ready
- Support Lead: Prepares support and monitoring for release window

---

## Support Lead

### Role Summary
The Support Lead serves as the primary escalation point for customers and internal teams during incidents and post-release operations.

### Responsibilities
- Triage incoming support issues and create runbooks for common problems
- Communicate customer-impacting issues to PM and Release Manager
- Maintain support handover documentation and FAQs
- Coordinate with engineering during incident response

### Goals
- Minimize customer impact through fast triage and resolution
- Capture reproducible bugs and escalate appropriately
- Improve product reliability through feedback loops

### Typical Communication
- Support tickets and incident summaries
- Handoff notes to engineering and release teams
- Post-incident retrospectives and action items

### Interaction with existing roles
- PM/PdM: Communicates customer-impacting trends and priorities
- Developers: Provides reproducible steps and logs for fixes
- Release Manager: Coordinates on release-related support windows
- QA Lead: Shares frequently seen issues and suggests test cases

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

