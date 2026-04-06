# OctoAcme — Role Interactions and Handoff Checklists

<!-- Related to: #6 -->

This document provides a Role Interaction Matrix and per-persona handoff checklists to make cross-role coordination explicit and repeatable. It is a companion to [octoacme-roles-and-personas.md](octoacme-roles-and-personas.md).

---

## Role Interaction Matrix

The table below shows typical handoff artifacts or triggers between sender roles (rows) and receiver roles (columns). A cell is empty where no regular direct handoff is expected.

| **Sender → Receiver** | PM | PdM | Developers | QA Lead | UX/UI Designer | Technical Writer | Release Manager | Support Lead | Stakeholders |
|---|---|---|---|---|---|---|---|---|---|
| **PM** | — | Schedule and scope updates | Sprint goals and priority queue | Risk blockers requiring QA attention | Design timeline alignment | Documentation milestone confirmation | Release calendar alignment | Support volume and trending issues | Status report, escalations |
| **PdM** | Roadmap priorities, trade-off decisions | — | Feature specs, acceptance criteria | Testability review of acceptance criteria | Product requirements, user research findings | Feature brief for documentation | Release scope confirmation | Customer feedback for backlog | Roadmap briefing |
| **Developers** | Blockers and schedule risks | Technical feasibility feedback | — | Feature ready → QA Lead: test plan, acceptance criteria, PR link | Design implementation questions | Code comments, changelog entries | Deployment runbook updates, feature flag status | Bug reproduction steps | Demo walkthrough |
| **QA Lead** | Defect severity report, go/no-go recommendation | Acceptance criteria gaps | Defect reports, fix-verification requests | — | UI/UX test cases for visual acceptance | Documentation gaps found during QA | QA sign-off, known-issues list | Regression test results for customer-reported bugs | Quality dashboard summary |
| **UX/UI Designer** | Design blockers impacting schedule | Design review, validated user flows | Design specs, annotated assets, Figma links | Visual and interaction acceptance criteria | — | Design decision rationale for docs | N/A | N/A | Prototype walkthroughs, usability findings |
| **Technical Writer** | Documentation readiness status | Content review requests | API docs review requests, changelog drafts | Test plan and acceptance criteria review for accuracy | Design terminology alignment | — | Release notes draft | Runbook and FAQ updates | Release notes (external) |
| **Release Manager** | Go/no-go decision, post-release status | Release scope final confirmation | Deployment instructions, rollback plan | QA sign-off request | N/A | Release notes final review | — | Advance release summary for support team briefing | Release announcement |
| **Support Lead** | Top support issues, CSAT trends | Customer pain points, feature improvement feedback | Critical bug reports with reproduction steps | Regression test requests for support-surfaced bugs | N/A | Runbook and FAQ gap reports | Post-release incident feedback | — | Escalation reports |
| **Stakeholders** | Approvals, strategic inputs | Business priorities | N/A | N/A | Feedback on UX prototypes | Content feedback (external docs) | Release approval | N/A | — |

---

## Handoff Checklists

### QA Lead Handoff Checklist

#### Planning → Development
- [ ] Test plan reviewed and approved alongside the sprint plan
- [ ] Acceptance criteria confirmed to be testable (no ambiguous language)
- [ ] Test environment and data requirements communicated to Developers
- [ ] Automated test scaffolding or framework updates identified and scheduled

#### Development → QA
- [ ] PR link and feature branch shared with QA Lead
- [ ] Acceptance criteria and scope confirmed unchanged (or delta communicated)
- [ ] Developer-written unit/integration tests reviewed and passing
- [ ] Test cases for manual/exploratory QA prepared and reviewed
- [ ] Defect tracking labels/board column configured for the sprint

#### QA → Release
- [ ] All critical and high-severity defects resolved or formally accepted as known issues
- [ ] Test execution summary (pass/fail rates, coverage) documented
- [ ] Regression suite executed and results shared
- [ ] QA sign-off issued (or escalated to PM if blockers remain)
- [ ] Known-issues list provided to Release Manager and Support Lead

---

### Release Manager Handoff Checklist

#### Planning → Execution
- [ ] Release calendar published and communicated to all stakeholders
- [ ] Deployment runbook reviewed and updated for this release
- [ ] Feature flag strategy and rollout plan confirmed with Developers
- [ ] Rollback plan documented and tested

#### QA → Release
- [ ] QA sign-off received from QA Lead
- [ ] Known-issues list reviewed; severity and business impact assessed
- [ ] Go/no-go call facilitated with PM, QA Lead, and Engineering lead
- [ ] Release notes reviewed and approved (Technical Writer sign-off)
- [ ] Support Lead briefed on release contents and potential impact areas

#### Release → Post-Release
- [ ] Deployment completed and smoke tests passed in production
- [ ] Post-release monitoring dashboards checked (errors, latency, usage)
- [ ] Stakeholder release announcement sent
- [ ] Post-mortem or release retrospective scheduled (if applicable)
- [ ] Incident report filed if production issues were encountered

---

### Technical Writer Handoff Checklist

#### Planning → Development
- [ ] Documentation scope agreed for the sprint (which features require docs)
- [ ] Draft outlines or stubs created in the documentation repository
- [ ] Dependencies on PdM or Developer interviews scheduled

#### Development → Documentation
- [ ] Feature specs and acceptance criteria reviewed for documentation accuracy
- [ ] Technical interviews with Developers completed; open questions resolved
- [ ] Draft documentation reviewed by at least one Developer and one PdM for accuracy
- [ ] Screenshots, diagrams, or code samples sourced and approved

#### Documentation → Release
- [ ] Release notes drafted, reviewed, and approved by PM and PdM
- [ ] User-facing documentation published or queued for publish on release date
- [ ] Internal runbooks, playbooks, and onboarding guides updated
- [ ] Documentation versioning confirmed (if multiple product versions are maintained)
- [ ] Support Lead notified of new/updated documentation

---

### Support Lead Handoff Checklist

#### Release → Support (Pre-Release)
- [ ] Release summary received from Release Manager
- [ ] Known-issues list reviewed with Support team; expected ticket topics identified
- [ ] Internal FAQ and runbook updated based on release contents
- [ ] Support team briefed on new features, changes, and potential impact areas
- [ ] Escalation path confirmed with Engineering and PM for severity-1 issues

#### Active Support → Delivery Team
- [ ] Recurring support issues aggregated and prioritized by impact
- [ ] Top issues communicated to PM and PdM in weekly sync
- [ ] Reproduction steps documented for escalated bugs before handoff to Developers
- [ ] Resolution updates shared back to affected customers once fixes are deployed
- [ ] CSAT and volume trends presented at monthly stakeholder review

---

### UX/UI Designer Handoff Checklist

#### Discovery → Planning
- [ ] User research findings summarized and shared with PdM and PM
- [ ] Design requirements documented and linked to relevant user stories
- [ ] Accessibility requirements (e.g., WCAG level) agreed upon with the team

#### Design → Development
- [ ] Final wireframes/mockups approved by PdM and PM
- [ ] Design specs exported (e.g., Figma link with inspect-ready layers)
- [ ] Component inventory reviewed against the design system (reuse vs. new components identified)
- [ ] Interaction notes and edge cases documented in the design file
- [ ] Assets (icons, images) exported in required formats and handed off

#### Development → Design Review
- [ ] Implemented UI reviewed against approved designs
- [ ] Deviations from design specs documented and resolved (or accepted with rationale)
- [ ] Accessibility audit passed (automated scan + manual keyboard/screen-reader check)
- [ ] Visual acceptance criteria signed off before QA begins
