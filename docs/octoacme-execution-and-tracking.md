# OctoAcme — Execution & Tracking

<!-- Related to: #6 -->

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

### QA Lead Responsibilities in Execution
The QA Lead plays a central role during execution by owning the test plan and coordinating testing activities across the team:
- **With Developers**: Reviews PRs for testability, aligns on acceptance criteria early, and coordinates fix-verification cycles to keep defects from blocking progress.
- **With the Release Manager**: Provides a formal QA sign-off (go/no-go recommendation) including a list of known issues and their severity before any release proceeds.
- **Escalation**: Unresolved critical defects are surfaced to the PM for prioritization; the QA Lead maintains a live defect tracker visible to all stakeholders.

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
- [ ] Roles and handoff checklist completed (all new personas acknowledged; handoff artifacts documented per [octoacme-role-interactions-and-checklists.md](octoacme-role-interactions-and-checklists.md))
