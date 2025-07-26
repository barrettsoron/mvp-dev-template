# Documentation Structure

This directory contains all project documentation, organized to support democratic decision-making and sustainable development.

## Directory Structure

```
tasks/
├── README.md           # This file
├── todo.md            # Current work and active tasks
├── decisions.md       # Technical and design decisions log
├── security.md        # Security review process and findings
├── user-stories.md    # User stories and feature planning (optional)
├── high-level-tasks.md # Strategic roadmap (optional)
└── archive/           # Completed work with lessons learned
    └── [task-id]-[description].md
```

## Core Documents

### todo.md - Active Task Tracking
- **Purpose**: Track current sprint/week work
- **Updated**: Daily during active development
- **Contains**: Concrete, actionable tasks with clear acceptance criteria
- **Philosophy**: Keep it focused on NOW, archive completed work

### decisions.md - Decision Log
- **Purpose**: Create institutional memory and accountability
- **Updated**: As decisions are made
- **Contains**: Technical choices, rationale, and review dates
- **Philosophy**: Document WHY, not just WHAT

### security.md - Security Process
- **Purpose**: Iterative security improvement
- **Updated**: Per schedule (weekly/monthly/quarterly)
- **Contains**: Threat model, checklist, review history
- **Philosophy**: Security as ongoing process, not destination

### archive/ - Completed Work
- **Purpose**: Preserve lessons learned and implementation details
- **Updated**: When tasks are completed
- **Contains**: What was built, challenges faced, future considerations
- **Philosophy**: Build organizational knowledge over time

## Optional Documents

Based on your project needs, you may add:

### user-stories.md
For user story driven development:
```markdown
As a [user type]
I need [capability]
So that [goal/benefit]

Acceptance Criteria:
- [ ] Specific testable criteria
```

### high-level-tasks.md
For strategic planning and roadmaps:
- Phase-based development plans
- Cross-functional dependencies
- Resource planning

### [domain]-specific.md
Documents specific to your domain:
- `compliance.md` for regulatory requirements
- `accessibility.md` for detailed accessibility plans
- `api.md` for API documentation
- `deployment.md` for infrastructure details

## Documentation Standards

### 1. Plain Language
Write for your community, not just developers:
- Define technical terms on first use
- Include examples
- Explain impact on users

### 2. Decision Rationale
Always document:
- What problem you're solving
- Options you considered
- Why you chose this approach
- When to revisit the decision

### 3. Accessibility
In all documentation:
- Use clear heading structure
- Include alt text for images
- Write descriptive link text
- Consider screen reader users

### 4. Currency
Keep documentation alive:
- Update as you work
- Review regularly
- Archive outdated content
- Date significant updates

## Workflow Integration

### Daily Development
1. Check `todo.md` for current tasks
2. Update task status as you work
3. Document decisions in `decisions.md`
4. Note security considerations

### Weekly Review
1. Archive completed tasks
2. Update security checklist
3. Review and update documentation
4. Plan upcoming work

### Per Feature
1. Start with user story (if applicable)
2. Break into tasks in `todo.md`
3. Document technical decisions
4. Security review before completion
5. Archive with lessons learned

### Per Release
1. Review all documentation
2. Update CHANGELOG.md
3. Archive release-specific docs
4. Plan next iteration

## Writing Guidelines

### Task Descriptions
```markdown
- [ ] Implement user authentication
  - Acceptance: Users can sign up, log in, log out
  - Security: Review auth flow with checklist
  - Accessibility: Ensure form errors are announced
  - Estimate: 2 days
```

### Decision Entries
```markdown
## 2024-01-15: Authentication Method

**Decision**: Use OAuth with social providers

**Context**: Users expressed "password fatigue" in interviews

**Options Considered**:
1. Traditional email/password - Rejected due to user feedback
2. Magic links - Rejected due to email delivery issues
3. OAuth - Selected for user convenience

**Rationale**: Reduces friction while maintaining security

**Review Date**: 2024-07-15 (6 months)
```

### Archive Format
```markdown
# T001: Contact Management System

**Completed**: 2024-01-20
**Duration**: 2 weeks
**Team**: Ana, Bo, Carlos

## What We Built
[Description of feature]

## Challenges Faced
[Technical or organizational challenges]

## Lessons Learned
[What we'd do differently]

## Future Considerations
[Improvements or related work]
```

## Anti-Patterns to Avoid

### ❌ Documentation Debt
- Don't wait to document
- Don't assume you'll remember
- Don't skip "obvious" decisions

### ❌ Write-Only Documentation
- Review regularly
- Update when things change
- Delete when obsolete

### ❌ Developer-Only Language
- Consider all stakeholders
- Explain technical concepts
- Include user impact

### ❌ Perfect Documentation
- Start with something
- Iterate and improve
- Focus on usefulness

## Contributing to Documentation

### For Developers
1. Document as you code
2. Update tasks in real-time
3. Explain decisions clearly
4. Include security notes

### For Non-Developers
1. Review for clarity
2. Add user perspectives
3. Identify missing context
4. Suggest improvements

### For Project Leads
1. Ensure documentation happens
2. Review for completeness
3. Archive old content
4. Plan documentation work

---

*Documentation is infrastructure. Invest in it accordingly.*