> Related to: #6

# OctoAcme — Role Interactions and Handoff Checklists

This document provides a role interaction matrix and handoff checklists for the expanded set of personas defined in [octoacme-roles-and-personas.md](octoacme-roles-and-personas.md). Use these to clarify responsibilities, reduce handoff gaps, and improve accountability across planning, execution, and release.

---

## Role Interaction Matrix

The table below summarizes typical artifacts and handoff triggers between roles. Rows represent the **sender** (originating role); columns represent the **receiver**.

| From \ To | PM | PdM | Developers | QA Lead | UX/UI Designer | Tech Writer | Release Manager | Support Lead | Stakeholders |
|---|---|---|---|---|---|---|---|---|---|
| **PM** | - | Project brief, priorities | Milestones, schedule | Test schedule needs | Design priorities | Doc needs | Release window | Support expectations | Status updates |
| **PdM** | Requirements & success metrics | - | Acceptance criteria, priorities | Acceptance criteria | UX input | Release notes input | Release scope | Customer impact | Approval requests |
| **Developers** | Implementation updates | Technical constraints | - | Feature ready, build | Design clarifications | API changes | Build artifacts | Repro steps | Demo |
| **QA Lead** | Test plan, quality risks | Test results summary | Bugs, reproduction steps | - | UX test cases | Docs updates needed | Test pass/fail, readiness | Incident handoff | QA readiness |
| **UX/UI Designer** | Design rationale | UX requirements | Assets & asset specs | UX test cases | - | Copy for UI | Design release notes | UX issues | Design signoff |
| **Technical Writer** | Docs needs | Release notes drafts | API docs, usage | Docs for test flows | UI copy | - | Docs for release | Support FAQs | Documentation deliverables |
| **Release Manager** | Release schedule | Release scope | Deployable artifacts | Test status | Release assets | Release notes | - | Support window | Release notifications |
| **Support Lead** | Support trends | Customer feedback | Repro steps | Known issues | UX feedback | Support docs | Post-release issues | - | Customer escalations |
| **Stakeholders** | Approvals | Strategic direction | Feature feedback | Quality concerns | UX acceptance | Customer-facing messaging | Release approvals | Major incidents | - |

---

## Handoff Checklists

### QA Lead — Development → QA Handoff

- [ ] Verify feature has clear acceptance criteria and Definition of Done (DoD)
- [ ] Receive testable build or deployment artifact
- [ ] Confirm automated tests are included; schedule manual test sessions
- [ ] Log test plan and assign test cases
- [ ] Report initial test results and risk summary to PM/PdM

### QA Lead — QA → Release Handoff

- [ ] Confirm all blocking defects are resolved or formally accepted as known risks
- [ ] Provide final test summary report to PM and Release Manager
- [ ] Verify regression suite has passed in CI
- [ ] Confirm acceptance criteria sign-off with PdM
- [ ] Hand off any open low-severity issues with triage notes to Support Lead

---

### Release Manager — QA → Release Handoff

- [ ] Confirm all blocking issues resolved or mitigated
- [ ] Verify smoke tests and post-deploy checks are defined
- [ ] Coordinate deployment window and communication plan
- [ ] Confirm rollback plan and backups are in place
- [ ] Announce pre-release readiness to stakeholders and support

### Release Manager — Release → Post-Release Handoff

- [ ] Execute post-deploy verification steps and log results
- [ ] Notify stakeholders and Support Lead of deployment outcome
- [ ] Confirm monitoring dashboards and alerts are active
- [ ] Initiate rollback if critical issues are detected
- [ ] Archive release notes and update deployment log

---

### Technical Writer — Planning → Development Handoff

- [ ] Review feature specs and acceptance criteria for documentation needs
- [ ] Identify user-facing changes requiring release notes or user guide updates
- [ ] Coordinate with PdM on messaging and terminology
- [ ] Create draft documentation outline or stub in repo

### Technical Writer — Release Handoff

- [ ] Finalize and review release notes with PM and PdM
- [ ] Publish or merge updated user guides, runbooks, and API docs
- [ ] Share documentation links with Support Lead for FAQs and handover docs
- [ ] Confirm all doc changes are discoverable in the docs/ folder or help site

---

### Support Lead — Release → Support Handoff

- [ ] Review release notes and known issues list from Release Manager
- [ ] Update support runbooks and FAQs based on new feature changes
- [ ] Brief support team on customer-impacting changes and escalation paths
- [ ] Confirm monitoring and alerting are in place for the release window
- [ ] Log any incoming issues post-release and route to engineering as needed

### Support Lead — Incident Response Handoff

- [ ] Triage incident and capture reproducible steps and affected scope
- [ ] Escalate to engineering (Developers/Release Manager) with logs and repro steps
- [ ] Communicate customer impact and status to PM/PdM and Stakeholders
- [ ] Coordinate resolution updates until incident is closed
- [ ] Produce post-incident summary and action items for retrospective

---

### UX/UI Designer — Planning → Development Handoff

- [ ] Deliver finalized wireframes, mockups, or prototypes to Developers
- [ ] Document UX acceptance criteria and accessibility requirements
- [ ] Confirm design system components or assets are available
- [ ] Conduct a design walkthrough with Developers and QA Lead
- [ ] Note any open UX questions or deferred decisions for follow-up

### UX/UI Designer — QA Handoff

- [ ] Provide UX-specific test cases covering usability and accessibility
- [ ] Review QA findings related to visual or interaction regressions
- [ ] Sign off on UX acceptance criteria with QA Lead and PdM
- [ ] Flag any design deviations found during testing for PM/PdM awareness
