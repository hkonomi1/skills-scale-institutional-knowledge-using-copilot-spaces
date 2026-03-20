# OctoAcme Project Management Processes

This document provides a brief overview of the project management processes used by OctoAcme. For full details, see the other files in this `docs/` folder.

## Table of Contents

### Lifecycle Docs
| Document | Purpose |
|---|---|
| [Project Initiation](./octoacme-project-initiation.md) | Charter, problem statement, success metrics |
| [Project Planning](./octoacme-project-planning.md) | Backlog, milestones, estimation, Definition of Done |
| [Execution & Tracking](./octoacme-execution-and-tracking.md) | Day-to-day workflows, metrics, escalation |
| [Risk Management & Communication](./octoacme-risks-and-communication.md) | Risk lifecycle, stakeholder comms, escalation paths |
| [Release & Deployment](./octoacme-release-and-deployment.md) | Release gates, deployment, post-deploy verification |
| [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) | Retro cadence, action items, process improvement |
| [Roles & Personas](./octoacme-roles-and-personas.md) | Role definitions and responsibilities |

### Templates
| Template | When to Use |
|---|---|
| [Weekly Status Update](./templates/weekly-status-update-template.md) | Every week during active delivery — fill in and share with stakeholders |
| [Risk Register](./templates/risk-register-template.md) | Start of planning; update at every weekly delivery sync |
| [Decision Log](./templates/decision-log-template.md) | Whenever a significant project decision is made |

### Checklists
| Checklist | When to Use |
|---|---|
| [Definition of Done](./checklists/definition-of-done-checklist.md) | Before marking any work item as Done |

## How to Use the Templates & Checklists

- **Weekly Status Update** – Copy the template at the start of each week. Complete each section before the delivery sync and share with relevant stakeholders.
- **Risk Register** – Create one register per project at planning time. Add rows as new risks emerge and update status at every weekly delivery sync.
- **Decision Log** – Append a row whenever a key architectural, scope, or process decision is made. Link to the relevant issue or PR for full context.
- **Definition of Done** – Review the checklist before moving any work item to *Done*. All applicable items must be checked before the item is considered complete.

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
| Sprint / iteration backlog | Prioritized, estimated work items for the current cycle |
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

**Release gates:**
- Acceptance criteria met
- CI/security checks passing
- Release notes and rollback plan prepared
- Staging smoke tests passed
- Production deployment (prefer automated pipelines)
- Post-deploy verification
- Stakeholder and support announcements
- Retrospective scheduled
