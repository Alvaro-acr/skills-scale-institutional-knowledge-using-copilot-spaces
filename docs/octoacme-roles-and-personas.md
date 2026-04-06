# OctoAcme Personas

<!-- Related to: #6 -->

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
The QA Lead owns the overall test strategy for a project or product area. They coordinate manual and automated quality assurance activities, define testing standards, and ensure that acceptance criteria are verified before features move to release.

### Responsibilities
- Define and maintain the overall test strategy and test plan
- Coordinate manual and automated QA efforts across the team
- Review acceptance criteria and ensure testability before development begins
- Track defect trends and surface quality risks to PM and PdM
- Liaise with the Release Manager to confirm release readiness
- Coach Developers on writing testable code and effective unit/integration tests

### Goals
- Prevent regressions and ensure consistent quality across releases
- Reduce the cost of defects by shifting testing left
- Provide clear, actionable quality metrics to stakeholders

### Typical Communication
- Sprint planning and backlog refinement sessions
- Test plan reviews with Developers and PdM
- Pre-release readiness sign-off with Release Manager
- Defect triage meetings with PM and Developers

### Interaction with Existing Roles
- **PM**: Reports quality status and escalates blocking defects that threaten the schedule.
- **PdM**: Validates acceptance criteria and confirms that features meet the Definition of Done.
- **Developers**: Collaborates on test coverage requirements, reviews PRs for testability, and coordinates fix-verification cycles.
- **QA (team members)**: Directs test case creation and execution; reviews and approves test results.
- **Stakeholders**: Presents quality dashboards and risk summaries at milestone checkpoints.
- **Release Manager**: Provides final QA sign-off and communicates outstanding known issues before release.

---

## UX/UI Designer

### Role Summary
The UX/UI Designer ensures that product features are intuitive, accessible, and visually consistent. They collaborate closely with PdM and Developers to translate user needs into wireframes, prototypes, and final design assets.

### Responsibilities
- Conduct user research and translate insights into design requirements
- Create wireframes, mockups, and interactive prototypes
- Define and maintain the design system and component guidelines
- Participate in backlog refinement to flesh out user stories and acceptance criteria
- Review implemented features against approved designs and flag deviations
- Champion accessibility standards (e.g., WCAG) across all deliverables

### Goals
- Deliver a consistent, high-quality user experience that meets accessibility standards
- Reduce rework by validating designs before development begins
- Bridge the gap between user needs and technical implementation

### Typical Communication
- Design reviews and critique sessions with PdM and Developers
- Handoff documentation (design specs, asset exports) via design tool (e.g., Figma)
- Usability test debrief notes shared with the broader team

### Interaction with Existing Roles
- **PM**: Aligns design timelines with project milestones; flags design blockers that impact delivery.
- **PdM**: Collaborates on problem framing, user stories, and validates designs against product requirements.
- **Developers**: Provides annotated design specs, answers implementation questions, and reviews built UI for fidelity.
- **QA Lead**: Works together to define visual and interaction acceptance criteria, assists in exploratory testing of UI flows.
- **Stakeholders**: Presents design concepts and usability findings; incorporates feedback into iterations.

---

## Technical Writer

### Role Summary
The Technical Writer produces clear, accurate documentation for internal teams and external audiences. They capture process changes, feature descriptions, API references, and user guides, ensuring that knowledge is preserved and accessible.

### Responsibilities
- Write and maintain user-facing documentation, release notes, and in-app help content
- Document internal processes, runbooks, and onboarding guides
- Collaborate with Developers and PdM to gather technical details for documentation
- Review PRs and release notes for completeness and clarity
- Establish and enforce documentation standards and templates
- Archive outdated content and manage the documentation versioning strategy

### Goals
- Ensure every shipped feature has corresponding, up-to-date documentation
- Reduce support burden by making self-service resources comprehensive and findable
- Maintain a single source of truth for processes and product knowledge

### Typical Communication
- Documentation review cycles tied to sprint releases
- Regular syncs with PdM for roadmap-driven documentation planning
- Async written feedback on PRs and release notes

### Interaction with Existing Roles
- **PM**: Coordinates documentation deliverables as part of release readiness criteria.
- **PdM**: Reviews feature specs to draft accurate documentation; confirms content reflects intended product behavior.
- **Developers**: Interviews for technical accuracy, reviews code comments and changelogs, and pairs on API documentation.
- **QA Lead**: Uses test plans and acceptance criteria as inputs to user documentation; flags documentation gaps found during QA.
- **Stakeholders**: Delivers release notes and product guides; incorporates stakeholder feedback on external-facing content.

---

## Release Manager

### Role Summary
The Release Manager coordinates release preparation, cross-team communication, and deployment activities. They own the release calendar, orchestrate go/no-go decisions, and ensure a smooth handoff from development and QA to production.

### Responsibilities
- Maintain the release calendar and communicate release windows to all stakeholders
- Define and enforce the release checklist and deployment runbook
- Facilitate go/no-go calls with PM, QA Lead, and Engineering leads
- Coordinate feature flags, rollout strategies, and rollback plans
- Ensure release notes and support documentation are ready before deployment
- Conduct post-release monitoring and lead incident response if needed

### Goals
- Deliver reliable, low-risk releases on schedule
- Minimize production incidents through rigorous pre-release validation
- Maintain a clear audit trail of what was released and when

### Typical Communication
- Release readiness reviews with PM, QA Lead, and Developers
- Pre/post-deployment status emails to stakeholders
- Incident reports and post-mortems as needed

### Interaction with Existing Roles
- **PM**: Aligns release schedule with project milestones and stakeholder commitments.
- **PdM**: Confirms feature scope and validates that release criteria meet product goals.
- **Developers**: Coordinates deployment activities, feature flag configuration, and hotfix procedures.
- **QA Lead**: Receives formal QA sign-off and outstanding issue list before proceeding with release.
- **Stakeholders**: Communicates release timelines, change summaries, and post-release status updates.

---

## Support Lead

### Role Summary
The Support Lead serves as the primary escalation point and feedback channel between the support team and the delivery organization. They ensure that customer-reported issues are triaged effectively and that product and engineering teams receive actionable feedback to prioritize fixes and improvements.

### Responsibilities
- Manage the support queue and triage incoming tickets by severity
- Escalate critical production issues to PM and Engineering as needed
- Represent the support perspective in sprint planning and backlog refinement
- Collaborate with Technical Writers to keep self-service resources accurate
- Track support metrics (volume, CSAT, time-to-resolution) and share trends
- Coordinate release communications to the support team to reduce reactive load

### Goals
- Minimize customer-impacting issues through proactive communication and documentation
- Reduce average time-to-resolution by improving escalation paths and knowledge bases
- Surface recurring themes from support data to inform product prioritization

### Typical Communication
- Regular syncs with PM to surface top support issues and recurring themes
- Release previews received from Release Manager to prepare the support team
- Cross-functional incident calls when severity warrants rapid escalation

### Interaction with Existing Roles
- **PM**: Provides support data and trending issues to inform prioritization and risk management.
- **PdM**: Shares customer pain points and feature feedback gathered from the support queue.
- **Developers**: Escalates reproduction steps for critical bugs; validates fixes before closing tickets.
- **QA Lead**: Coordinates on regression testing for bugs surfaced through support.
- **Stakeholders**: Reports support health metrics and contributes to post-incident reviews.
- **Release Manager**: Receives advance notice of release contents to brief the support team and update runbooks.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

