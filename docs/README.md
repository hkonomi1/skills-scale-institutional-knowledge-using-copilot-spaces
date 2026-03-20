# OctoAcme Project Management Processes

This document provides a brief overview of the project management processes used by OctoAcme. For full details, see the other files in this `docs/` folder.

## Lifecycle

Projects follow a five-stage lifecycle: **Initiation → Planning → Execution → Release → Close/Retrospective**. Work advances through a formal decision gate only once success metrics are agreed upon, stakeholders have aligned on priority, and team availability is confirmed.

## Guiding Principles

- **Customer-first** – decisions are grounded in user and business value.
- **Iterative delivery** – ship in small increments and learn continuously.
- **Clear ownership** – the PM owns delivery; the Product Lead/PdM owns outcomes.
- **Data-informed decisions** – use metrics and evidence, not opinion alone.
- **Psychological safety** – team members surface risks and disagreements openly.

## Key Artifacts

| Artifact | Purpose |
|---|---|
| Project charter / one-pager | Problem statement, SMART goal, success metrics, stakeholders, timeline, risks |
| Roadmap & release plan | Milestone sequencing and scope commitments |
| Sprint / iteration backlog | Prioritised, estimated work items for the current cycle |
| Acceptance criteria & Definition of Done | Shared quality bar for every item |
| Risk register | Impact, likelihood, owner, mitigation, and current status |
| Retrospective notes & action items | Learnings converted to owned backlog items with due dates |

## Roles & Responsibilities

| Role | Core Responsibilities |
|---|---|
| **Project Manager (PM)** | Plans, timelines, risk/dependency management, meetings, status reporting |
| **Product Manager (PdM) / Product Lead** | Vision, prioritisation, success metrics, trade-offs, stakeholder alignment |
| **Developers** | Design, build, test features; estimation; documentation; surface technical risks |
| **QA / Testing** | Validate acceptance criteria and overall quality |
| **Stakeholders** | Provide input, review demos, approve key decisions |

## Communication & Cadence

The team maintains a **single source of truth** for project status. The standard weekly status update includes: progress since last update, next steps, risks/blockers, and asks/decisions needed.

| Ritual | Frequency | Focus |
|---|---|---|
| Standup | Daily | Blockers and cross-team dependencies |
| Delivery sync | Weekly | Progress review and risk discussion |
| Sprint / milestone demo | Per sprint | Working software, stakeholder feedback |
| PM–PdM alignment | Weekly | Roadmap and priority alignment |
| Stakeholder update | Monthly | High-level progress, decisions, risks |

**Escalation path:** team triage → PM → Product Lead → sponsor (when business impact requires).

## Quality Assurance

**Project board workflow:** Backlog → Ready → In Progress → In Review → QA → Done

**PR discipline:**
- Prefer small, focused pull requests.
- Include a link to the related issue and acceptance criteria in the PR description.
- CI checks (tests + lint) must pass before review begins.
- At least one approval is required before merging.

**Testing expectations:**
- Unit tests for all new logic.
- Integration tests where component boundaries are exercised.
- End-to-end smoke tests for critical flows before each release.
- Security scanning in CI; manual QA for feature acceptance when appropriate.

**Release gates:** acceptance criteria met · CI/security checks passing · release notes and rollback plan prepared · staging smoke tests passed · production deployment (prefer automated pipelines) · post-deploy verification · stakeholder and support announcements · retrospective scheduled.
