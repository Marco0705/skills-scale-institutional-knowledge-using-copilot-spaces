# OctoAcme — Execution & Tracking

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
  - **UX Designer** reviews PRs for design implementation accuracy and accessibility

### Design Handoff & Implementation
- **UX Designer** provides design specs, prototypes, and acceptance criteria before development starts
- Developers collaborate with UX during implementation for clarifications
- Design QA occurs during PR review to ensure fidelity to design specifications

## Quality & Testing
- Unit tests for new logic (owned by **Developers**)
- Integration tests where applicable (owned by **Developers**)
- End-to-end smoke tests for critical flows before release (coordinated by **QA Lead**)
- Security scanning in CI (monitored by **DevOps/Platform Engineer**)
- Manual QA for feature acceptance when needed (led by **QA Lead**)
- Usability testing and accessibility validation (led by **UX Designer**)

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
