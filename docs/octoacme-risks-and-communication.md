# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner (assign to appropriate role based on risk type)
- Mitigation plan
- Status

### Role-Specific Risk Ownership:
- **QA Lead**: Quality risks, test coverage gaps, defect trends
- **DevOps Engineer**: Infrastructure risks, deployment issues, security vulnerabilities
- **UX Designer**: Usability risks, accessibility concerns, design inconsistencies
- **Product Manager**: Scope risks, feature priority conflicts, market timing
- **Project Manager**: Schedule risks, resource constraints, dependency delays
- **Sponsor/Stakeholder**: Business risks, budget overruns, strategic misalignment

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

## Communication Templates
Weekly Status Template:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:

Incident Communication
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled

## Escalation Paths
- Team-level -> PM -> Product Lead -> Sponsor/Stakeholder
- For security incidents, follow the security incident runbook and notify Security on-call
- For infrastructure/deployment issues: DevOps Engineer -> Engineering Lead -> Sponsor/Stakeholder
- For quality issues: QA Lead -> Product Manager -> Sponsor/Stakeholder
- For design/UX concerns: UX Designer -> Product Manager -> Sponsor/Stakeholder

### Escalation Guidelines:
- Escalate early when blockers impact timeline or quality
- Provide context, impact assessment, and proposed solutions
- Document escalation decisions in the project communication log
- Sponsor/Stakeholder provides final decision on scope, budget, or timeline trade-offs
