# OctoAcme Project Management Processes

## Overview

OctoAcme employs a structured, customer-centric project management framework designed to ensure consistent, repeatable execution across all cross-functional projects. This document provides a comprehensive overview of our project management processes, roles, and key practices.

## Core Principles

- **Customer-first**: Prioritize customer value and usability in every decision
- **Iterative delivery**: Deliver small, testable increments to gather feedback early
- **Clear ownership**: Each project has a named Project Manager (PM) and Product Lead
- **Data-informed decisions**: Measure impact and iterate based on evidence
- **Psychological safety**: Encourage feedback, learning, and continuous improvement

## Key Roles & Responsibilities

### Project Manager (PM)
Coordinates delivery activities, manages schedules, risks, and communications to enable the team to deliver on commitments efficiently.
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Product Manager (PdM)
Defines what should be built to deliver customer and business value. Owns the product vision, prioritizes the backlog, and measures outcomes.
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Developers
Design, build, test, and deliver software components that meet acceptance criteria and quality standards.
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### QA/Testing
Validate quality and ensure that features meet acceptance criteria before release.
- Conduct unit, integration, and end-to-end testing
- Verify acceptance criteria are met
- Perform security and performance validation
- Document test results and defects

## Project Lifecycle

OctoAcme projects follow a five-phase lifecycle:

### 1. Initiation
Validate business need, identify stakeholders, and create a lightweight plan to authorize work.

**Key Deliverables:**
- Project One-pager (Problem, Goal, Success Metrics)
- Stakeholder list & communication plan
- High-level timeline and key milestones
- Initial risk list
- Resource needs and rough effort estimate

**Decision Gate:** Move to planning when success metrics are clear, stakeholders agree on priority, and team availability is confirmed.

### 2. Planning
Turn an approved initiative into an actionable plan and backlog for delivery.

**Key Activities:**
- Kickoff meeting with stakeholders and delivery team
- Create prioritized backlog with acceptance criteria
- Estimate scope (T-shirt sizing or story points)
- Define Definition of Done (DoD)
- Identify dependencies and integration points
- Create release plan and milestone map

### 3. Execution & Tracking
Manage day-to-day execution and track progress toward project milestones.

**Team Rhythm:**
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

**Quality & Testing:**
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

**PR Workflow:**
- Small PRs (≤ 400 lines when possible)
- Include issue link and acceptance criteria in PR description
- Run automated tests and linting in CI before requesting review
- Require at least one approval before merging

### 4. Release & Deployment
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

**Pre-Release Requirements:**
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback/mitigation plan documented
- Smoke tests prepared

**Deployment Process:**
- Deploy to staging and run smoke tests
- Deploy to production (automated pipeline preferred)
- Run post-deploy verifications
- Announce release to stakeholders and support

### 5. Retrospective & Continuous Improvement
Capture learnings and convert them into actionable improvements.

**Retrospective Structure:**
- What went well
- What could be improved
- Action items (owner, due date)
- Follow-up on previous action items

**Action Item Management:**
- Add action items to the project backlog or issues with clear owners and timelines
- Review outstanding actions in the weekly PM sync
- Measure impact of action items and celebrate improvements

## Risk Management & Communication

### Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

**Risk Lifecycle:**
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduce via actions and contingency plans
- Monitor: review at weekly syncs and update status

### Communication Cadence
- **Weekly sync:** Project Manager + Product Manager
- **Twice-weekly standups:** Delivery team (or as agreed)
- **Monthly updates:** Stakeholder briefings
- **Ad-hoc escalations:** As needed

### Escalation Paths
- Team-level → PM → Product Lead → Sponsor
- For security incidents, follow the security incident runbook and notify Security on-call

## Key Artifacts

Every OctoAcme project maintains:
- **Project Charter / One-pager:** Problem, Goal, Success Metrics
- **Roadmap and Release Plan:** Milestones and delivery timeline
- **Sprint/Iteration Backlog:** Prioritized work with acceptance criteria
- **Acceptance Criteria & Definition of Done:** Quality standards
- **Risk Register:** Active risk tracking and mitigation
- **Retrospective notes and action items:** Learnings and improvements

## How to Use These Process Docs

1. **Keep the Project Charter updated** in your project repository
2. **Reference process-specific docs** in `.copilot/` when using Copilot Spaces for context
3. **Adapt templates** to fit your team's specific needs while maintaining alignment with OctoAcme principles
4. **Document deviations** from standard processes with clear rationale
5. **Share learnings** back to the central documentation to continuously improve our processes

## Additional Resources

For detailed guidance on each phase, refer to:
- [Project Management Overview](octoacme-project-management-overview.md)
- [Project Initiation Guide](octoacme-project-initiation.md)
- [Project Planning](octoacme-project-planning.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Risk Management & Communication](octoacme-risks-and-communication.md)
- [Release & Deployment Guide](octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
- [Roles and Personas](octoacme-roles-and-personas.md)
