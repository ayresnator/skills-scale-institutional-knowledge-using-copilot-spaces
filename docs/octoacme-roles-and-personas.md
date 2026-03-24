# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Release Manager

### Role Summary
The Release Manager coordinates release schedules, approvals, and artifact readiness. They act as the gatekeeper for production deployments, ensuring all pre-release requirements are met before any release proceeds.

### Responsibilities
- Own and maintain the release calendar and deployment windows
- Verify all pre-release criteria are satisfied (CI passing, smoke tests, release notes)
- Coordinate go/no-go decisions with relevant stakeholders
- Manage rollback procedures and communicate release status
- Track release metrics and post-deploy verification results

### Goals
- Ensure predictable, low-risk releases to production
- Reduce release-related incidents through thorough pre-release validation
- Maintain a clear audit trail of release decisions and approvals

### Typical Communication
- Release readiness meetings with PM, DevOps, and QA Lead
- Go/no-go announcements and post-release summaries
- Escalations to Project Manager when release criteria are not met

### Interaction with Existing Roles
- Works with **Project Managers** to align release windows with project milestones
- Coordinates with **DevOps Engineers** on deployment pipelines and rollback readiness
- Validates sign-off from **QA Lead** before approving releases
- Provides release summaries to **Product Managers** and stakeholders

---

## DevOps Engineer

### Role Summary
DevOps Engineers manage CI/CD pipelines, environments, and deployment automation. They bridge the gap between development and operations to enable fast, reliable, and repeatable delivery.

### Responsibilities
- Build and maintain CI/CD pipelines (build, test, deploy stages)
- Manage staging, pre-production, and production environments
- Implement infrastructure-as-code and configuration management
- Ensure monitoring, alerting, and observability are in place
- Support incident response with deployment-related tooling and rollback

### Goals
- Automate repetitive manual processes to reduce human error
- Maintain high availability and reliability of deployment infrastructure
- Enable developers to ship safely and quickly

### Typical Communication
- Technical syncs with development team on pipeline issues
- Release coordination with Release Manager
- Incident updates via on-call channels

### Interaction with Existing Roles
- Supports **Developers** by providing reliable CI/CD tooling and environment access
- Partners with **Release Manager** to execute and validate deployments
- Works with **Security Champion** to embed security scanning into pipelines
- Coordinates with **Project Manager** on environment availability and deployment scheduling

---

## QA Lead

### Role Summary
The QA Lead defines quality standards and coordinates testing efforts across the project. They ensure that acceptance criteria are validated and that quality gates are enforced before features reach production.

### Responsibilities
- Define and maintain the test strategy and quality standards
- Coordinate manual and automated testing efforts across the team
- Review and approve acceptance criteria for backlog items
- Manage regression and end-to-end test suites
- Report on test coverage, defect trends, and release readiness

### Goals
- Prevent defects from reaching production through rigorous validation
- Build a culture of quality ownership across the whole team
- Maintain a sustainable automated testing infrastructure

### Typical Communication
- Test plan reviews with Product Managers and Developers
- QA sign-off communications to Release Manager
- Defect triage sessions with the development team

### Interaction with Existing Roles
- Collaborates with **Developers** on testability, unit tests, and defect resolution
- Works with **Product Managers** to validate acceptance criteria and user stories
- Provides release readiness sign-off to the **Release Manager**
- Participates in planning sessions facilitated by **Project Managers**

---

## UX Designer

### Role Summary
UX Designers lead user research, wireframing, prototyping, and usability validation. They ensure that features are intuitive, accessible, and aligned with user needs before and during development.

### Responsibilities
- Conduct user research (interviews, surveys, usability tests)
- Create wireframes, prototypes, and design specifications
- Collaborate with Product Managers on feature definitions and user flows
- Review implemented features for design fidelity and usability
- Maintain and evolve the design system and style guide

### Goals
- Deliver user experiences that are intuitive and accessible
- Ground product decisions in validated user insights
- Reduce rework by resolving UX questions early in the planning cycle

### Typical Communication
- Design reviews and feedback sessions with development team
- User research readouts to Product Managers and stakeholders
- Async design feedback via prototyping tools and PR comments

### Interaction with Existing Roles
- Partners with **Product Managers** on problem definition, user flows, and prioritization
- Works with **Developers** to ensure design specifications are implemented accurately
- Shares usability findings with **Project Managers** that may affect scope or timeline
- Collaborates with **QA Lead** on usability acceptance criteria

---

## Security Champion

### Role Summary
The Security Champion advocates for secure development practices and acts as the primary point of contact for security-related concerns within the project team. They bridge the development team and any central security function.

### Responsibilities
- Review code and designs for common security vulnerabilities
- Ensure security scanning tools are integrated and monitored in CI
- Communicate security requirements and risk posture to the project team
- Triage and prioritize security findings from automated scans
- Lead security-related incident response tasks for the project

### Goals
- Reduce the risk of security incidents through proactive practices
- Embed security awareness into daily development workflows
- Ensure compliance with organizational security standards

### Typical Communication
- Security review notes during code review and design phases
- Risk escalations to Project Manager and central security team
- Incident response communications for security-related issues

### Interaction with Existing Roles
- Works with **Developers** to resolve vulnerabilities and promote secure coding practices
- Coordinates with **DevOps Engineers** to maintain security scanning in CI/CD pipelines
- Escalates unresolved security risks to **Project Managers** for risk register tracking
- Advises **Product Managers** on security trade-offs during prioritization

---

## Customer Success Manager

### Role Summary
The Customer Success Manager (CSM) bridges customer and user feedback to the project team. They ensure that customer insights, support trends, and satisfaction signals inform planning and prioritization decisions.

### Responsibilities
- Collect and synthesize customer feedback, support tickets, and satisfaction data
- Represent customer perspectives in planning and prioritization discussions
- Communicate upcoming changes, releases, and maintenance windows to customers
- Track adoption and success metrics post-release
- Escalate critical customer-impacting issues to the project team

### Goals
- Ensure customers experience measurable value from released features
- Close the feedback loop between customer insights and product decisions
- Maintain high customer satisfaction and reduce churn risk

### Typical Communication
- Quarterly business reviews and feedback summaries for Product Managers
- Release communication and change announcements to customer segments
- Escalations via Project Manager for urgent customer-impacting issues

### Interaction with Existing Roles
- Partners with **Product Managers** to surface customer insights that influence the roadmap
- Coordinates with **Project Managers** on communication timing for customer-facing releases
- Works with **Developers** and **QA Lead** to validate that customer-reported issues are resolved
- Provides post-release adoption data to the team to inform retrospectives

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

