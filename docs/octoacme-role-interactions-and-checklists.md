# OctoAcme Role Interactions & Handoff Checklists

> Related to: #6

This document provides a Role Interaction Matrix summarizing handoff points between roles, and handoff checklists for each of the expanded personas introduced in [octoacme-roles-and-personas.md](./octoacme-roles-and-personas.md).

---

## Role Interaction Matrix

The table below shows typical handoff artifacts or triggers between roles. Rows represent the **Sender** (the role initiating the handoff); columns represent the **Receiver** (the role accepting the handoff).

| Sender → Receiver | PM | PdM | Developers | QA Lead | UX/UI Designer | Technical Writer | Release Manager | Support Lead | Stakeholders |
|---|---|---|---|---|---|---|---|---|---|
| **PM** | — | Weekly sync, schedule updates | Sprint goals, priorities | Timeline constraints, risk flags | Design milestone dates | Doc milestone dates | Release schedule, go/no-go input | Support readiness dates | Status reports, escalations |
| **PdM** | Roadmap updates, trade-off decisions | — | Feature specs, acceptance criteria | Acceptance criteria, Definition of Done | User research, feature briefs | Feature context for docs | Product readiness sign-off | Roadmap visibility, feedback requests | Stakeholder briefings, roadmap |
| **Developers** | Blockers, estimates, progress | Demo-ready features, technical constraints | — | Feature ready → QA Lead: test plan, acceptance criteria, build artifacts | Design questions, implementation feedback | Technical accuracy review requests | Build artifacts, deployment notes | Bug context for escalations | — |
| **QA Lead** | Test summary, release readiness risk | Acceptance criteria gaps, quality findings | Defect reports, re-test requests | — | UI/UX defect reports | Documentation review for test accuracy | Release readiness sign-off, outstanding defects list | Known issues list, regression findings | — |
| **UX/UI Designer** | Design status, blockers | Design solutions, usability findings | Annotated specs, assets, Figma links | Design intent docs for UI testing | — | Design change log for release notes | — | — | Design review presentations |
| **Technical Writer** | Doc milestone status | Draft docs for accuracy review | Technical review requests | Docs included in release checklist | UI copy review | — | Release notes draft | Support knowledge base updates | External doc review requests |
| **Release Manager** | Deployment status, go/no-go decision | Release confirmation | Deployment coordination, rollback plan | QA sign-off request | — | Release notes approval | — | Pre-release briefing, post-release summary | Deployment notifications |
| **Support Lead** | Escalation alerts, SLA risk | Customer feedback, pain points | Bug context and reproduction steps | Defect patterns, regression trends | UX friction reports | Knowledge base gaps | Post-release incident reports | — | Customer satisfaction summaries |
| **Stakeholders** | Approvals, strategic direction | Product feedback, priorities | — | — | Design approvals | Doc approvals | — | — | — |

---

## Handoff Checklists

### QA Lead Handoff Checklist

**Development → QA (Feature enters testing)**
- [ ] Acceptance criteria documented and shared by PdM
- [ ] Test plan created and reviewed
- [ ] Build artifacts deployed to test environment
- [ ] Developer available for defect triage and questions
- [ ] Automated test suite passing before manual QA begins

**QA → Release Manager (Release readiness)**
- [ ] All acceptance criteria validated and signed off
- [ ] Critical and high-severity defects resolved or risk-accepted with PM
- [ ] Regression test suite passing
- [ ] Known issues list prepared and shared with Support Lead
- [ ] QA release readiness sign-off communicated to Release Manager

---

### Release Manager Handoff Checklist

**Planning → Release Preparation**
- [ ] Release schedule confirmed with PM and PdM
- [ ] Release checklist created and shared with team
- [ ] Feature flags and configuration changes documented
- [ ] Rollback plan defined and reviewed with Developers

**QA → Release (Go/No-Go)**
- [ ] QA Lead release readiness sign-off received
- [ ] All deployment artifacts (build, scripts, configs) validated
- [ ] Release communication drafted (stakeholders, support team)
- [ ] Deployment window confirmed and communicated

**Release → Post-Release**
- [ ] Deployment completed and verified in production
- [ ] Post-release monitoring alerts confirmed active
- [ ] Post-release summary distributed to stakeholders
- [ ] Support Lead briefed on changes and any known issues
- [ ] Hotfix process confirmed and on standby if needed

---

### Technical Writer Handoff Checklist

**Development → Documentation**
- [ ] Feature context received from PdM and Developers
- [ ] Technical review of draft docs requested and completed
- [ ] Screenshots and UI copy validated with UX/UI Designer
- [ ] Docs reviewed for accuracy against final acceptance criteria

**Documentation → Release**
- [ ] Release notes drafted and approved by PM and PdM
- [ ] User-facing docs updated and reviewed
- [ ] Internal process docs updated if workflows changed
- [ ] Documentation included in the release readiness checklist

**Release → Support**
- [ ] Knowledge base articles updated with new feature information
- [ ] Support Lead notified of new or updated documentation
- [ ] Known limitations and workarounds documented

---

### Support Lead Handoff Checklist

**Release → Support Readiness**
- [ ] Pre-release briefing received from Release Manager
- [ ] Known issues list reviewed and added to internal knowledge base
- [ ] Support team trained on new features and changes
- [ ] Escalation paths confirmed with PM and Developers

**Support → Product (Feedback Loop)**
- [ ] Weekly support summary prepared with issue trends and SLA metrics
- [ ] High-priority customer pain points escalated to PdM for backlog consideration
- [ ] Recurring defects shared with QA Lead for coverage improvement
- [ ] Customer satisfaction data shared with PM and stakeholders

---

### UX/UI Designer Handoff Checklist

**Planning → Design**
- [ ] Feature brief and user research received from PdM
- [ ] Design scope and timeline confirmed with PM
- [ ] Existing design system components identified for reuse

**Design → Development**
- [ ] Wireframes and mockups reviewed and approved by PdM
- [ ] Annotated specs and assets published in design tool (e.g., Figma)
- [ ] Developer handoff meeting held to walk through design intent
- [ ] Accessibility requirements documented and communicated

**Development → QA (Design Validation)**
- [ ] Design intent documentation shared with QA Lead
- [ ] UI/UX acceptance criteria defined for QA testing
- [ ] Design review of implemented feature completed
- [ ] Feedback on implementation gaps communicated to Developers
