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
  - **DevOps Engineer**: Ensures CI pipelines are running correctly, troubleshoots build failures
  - **QA Lead**: Reviews PRs for testability and test coverage before QA sign-off

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

### QA Lead Responsibilities
- Define test strategy and test plans for each sprint
- Coordinate manual testing efforts and exploratory testing
- Review acceptance criteria with Product Manager for testability
- Track and triage defects through resolution
- Provide QA sign-off on features before release
- Report quality metrics (defect rates, test coverage) to team

### DevOps Engineer Responsibilities
- Maintain CI/CD pipeline health and performance
- Configure automated testing in build pipelines
- Set up security scanning tools and monitor results
- Manage test environments (dev, staging, production)
- Implement deployment automation and rollback procedures
- Monitor production systems and coordinate incident response

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Cross-Role Handoffs and Accountability

Clear handoffs between roles ensure work flows smoothly and nothing falls through the cracks. Each handoff should include confirmation of completion criteria and acceptance by the receiving role.

### Key Handoffs:
- **Product Manager → UX Designer**: User requirements, business goals, and success metrics
  - *Accountability*: UX Designer confirms understanding of user needs and design constraints
  
- **UX Designer → Developer**: Design specifications, mockups, and interaction patterns
  - *Accountability*: Developer confirms design is implementable and asks clarifying questions before implementation
  
- **Developer → QA Lead**: Feature implementation complete, PR merged, ready for testing
  - *Accountability*: QA Lead verifies acceptance criteria are clear and test environment is ready
  
- **QA Lead → Product Manager**: Feature tested and QA approved for release
  - *Accountability*: Product Manager validates feature meets business requirements and accepts for release
  
- **Product Manager → DevOps Engineer**: Release approval and deployment request
  - *Accountability*: DevOps Engineer confirms deployment plan, timing, and rollback strategy
  
- **DevOps Engineer → Project Manager**: Deployment complete and production verified
  - *Accountability*: Project Manager updates stakeholders and closes release milestone
  
- **Project Manager → Sponsor/Stakeholder**: Milestone completion, status updates, decision requests
  - *Accountability*: Sponsor/Stakeholder provides timely decisions and approvals

### Handoff Checklist:
- [ ] Completion criteria clearly defined before work begins
- [ ] Receiving role confirms readiness to accept handoff
- [ ] Documentation or artifacts shared (designs, PRs, test reports)
- [ ] Issues or blockers flagged immediately, not at handoff time
- [ ] Handoff status visible on project board

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
- [ ] QA test plans created for each sprint/milestone
- [ ] Deployment pipelines tested and monitored
- [ ] Cross-role handoffs defined and tracked on project board
- [ ] Design specifications reviewed and approved before implementation
- [ ] Production monitoring and alerting configured by DevOps
- [ ] Stakeholder communication cadence established
