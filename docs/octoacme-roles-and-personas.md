# OctoAcme Personas

> Related to: #6

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
The QA Lead owns the overall test strategy for the project, coordinates manual and automated quality assurance activities, and serves as the primary liaison between the engineering team and release readiness.

### Responsibilities
- Define and maintain the test strategy, test plans, and acceptance criteria
- Coordinate manual and automated QA efforts across the team
- Review and triage defects, prioritizing severity and resolution
- Validate that features meet the Definition of Done before handoff to Release Manager
- Report testing outcomes, coverage metrics, and outstanding risks to the PM and PdM

### Goals
- Ensure all features meet quality standards before release
- Reduce defect escape rate to production
- Improve test coverage and automation over time

### Typical Communication
- Sprint-level test plans and QA summaries shared with PM and PdM
- Defect triage sessions with Developers
- Release readiness sign-off with Release Manager

### Interaction with existing roles
- **PM**: Provides testing status, flags risks, and requests timeline adjustments when quality gates are at risk.
- **PdM**: Aligns on acceptance criteria and validates that delivered features match product intent.
- **Developers**: Collaborates on test coverage, reviews code for testability, and coordinates defect resolution.
- **QA**: The QA Lead guides and coordinates the broader QA function; other QA contributors report testing results to the QA Lead.
- **Stakeholders**: Communicates release readiness and any outstanding quality risks prior to deployment.

---

## UX/UI Designer

### Role Summary
The UX/UI Designer ensures that features are usable, accessible, and visually consistent. They collaborate closely with the Product Manager and Developers to translate requirements into clear interface designs and prototypes.

### Responsibilities
- Create wireframes, mockups, and interactive prototypes
- Define and maintain design guidelines and component standards
- Collaborate with PdM on user research and usability testing
- Provide developers with design specifications and assets
- Participate in acceptance reviews to validate implementation against design intent

### Goals
- Deliver intuitive, accessible, and delightful user experiences
- Reduce rework caused by ambiguous or late-stage design changes
- Maintain a consistent design language across the product

### Typical Communication
- Design reviews and critiques with PdM and Developers
- Handoff specs and annotated mockups in the design tool (e.g., Figma)
- Usability findings and recommendations shared with the team

### Interaction with existing roles
- **PM**: Aligns on design timelines and flags any scope creep affecting design deliverables.
- **PdM**: Translates product requirements and user research into design solutions; validates designs against user goals.
- **Developers**: Provides detailed specifications and assets; answers implementation questions during development.
- **QA**: Shares design intent documentation so QA can validate UI consistency and accessibility in testing.
- **Stakeholders**: Presents prototypes and design rationale for stakeholder review and approval.

---

## Technical Writer

### Role Summary
The Technical Writer is responsible for creating and maintaining clear, accurate documentation for internal teams and end users. They ensure that processes, features, and workflows are well-documented across the project lifecycle.

### Responsibilities
- Author and maintain user guides, API docs, process docs, and release notes
- Collaborate with Developers and PdM to capture feature changes and technical details
- Review docs for accuracy, completeness, and consistency with the style guide
- Coordinate documentation reviews and sign-offs before each release
- Track documentation gaps and create issues for content updates

### Goals
- Ensure all shipped features have accurate, up-to-date documentation
- Reduce support load by providing clear self-service content
- Maintain a consistent voice and structure across all documentation

### Typical Communication
- Documentation review requests sent to Developers, PdM, and QA Lead
- Release notes drafts shared with PM and PdM for approval
- Style guide and documentation standards communicated to the broader team

### Interaction with existing roles
- **PM**: Aligns on documentation milestones within the project schedule.
- **PdM**: Interviews for feature context and validates that documentation accurately reflects product intent.
- **Developers**: Reviews technical accuracy of implementation-level docs and release notes.
- **QA**: Coordinates to ensure documentation is included in the release readiness checklist.
- **Stakeholders**: Shares external-facing docs for approval before publication.

---

## Release Manager

### Role Summary
The Release Manager coordinates all activities required to safely and reliably deploy software. They own the release checklist, manage communication around deployments, and serve as the final gatekeeper before production releases.

### Responsibilities
- Maintain and execute the release checklist for each deployment
- Coordinate go/no-go decisions with PM, QA Lead, and Developers
- Manage release communication to stakeholders and support teams
- Track post-release stability and coordinate hotfix processes if needed
- Document release history and deployment artifacts

### Goals
- Achieve consistent, low-risk deployments
- Minimize production incidents caused by release failures
- Maintain clear audit trails for all releases

### Typical Communication
- Release readiness meetings with PM, QA Lead, and Developers
- Deployment notifications and post-release summaries to stakeholders
- Incident and hotfix coordination reports as needed

### Interaction with existing roles
- **PM**: Aligns on release timelines and communicates any risks that may delay deployment.
- **PdM**: Confirms product readiness and that acceptance criteria have been met before release.
- **Developers**: Coordinates build artifacts, deployment scripts, and feature flag configurations.
- **QA**: Receives QA sign-off as a prerequisite for proceeding with the release.
- **Stakeholders**: Distributes pre-release notifications and post-release summaries.

---

## Support Lead

### Role Summary
The Support Lead serves as the primary escalation point for customer-facing issues and acts as the feedback channel between the support team and the delivery team. They ensure that customer pain points are surfaced, prioritized, and resolved.

### Responsibilities
- Triage and escalate high-priority support issues to the PM and engineering team
- Maintain a knowledge base of known issues and workarounds
- Collaborate with the Release Manager to prepare support teams for upcoming releases
- Provide voice-of-customer feedback to PdM for backlog refinement
- Track support SLAs and report on trends and recurring issues

### Goals
- Reduce time-to-resolution for customer-reported issues
- Improve customer satisfaction through timely, accurate support
- Feed real-world usage insights back into the product roadmap

### Typical Communication
- Weekly support summary reports shared with PM and PdM
- Escalation alerts for critical issues sent directly to PM and Release Manager
- Feedback sessions with PdM for backlog input

### Interaction with existing roles
- **PM**: Escalates time-sensitive issues and aligns on resolution priorities.
- **PdM**: Shares customer feedback, usage trends, and pain points to inform roadmap decisions.
- **Developers**: Coordinates on bug investigations and provides context from customer reports.
- **QA**: Shares patterns in customer-reported defects to improve test coverage.
- **Stakeholders**: Provides customer satisfaction metrics and notable support incidents in stakeholder updates.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

