# [Project Name] Development Context

> This file provides context for AI assistants (like Claude) to understand your project's specific needs, values, and patterns.
> Customize all sections marked with [brackets] for your project.

## Project Overview

**Project**: [Your project name]
**Type**: [Campaign tool / Organizing platform / Mutual aid system / etc.]
**Status**: [Planning / Active development / Production]
**Team Size**: [Individual / Small team / Large organization]

## Mission & Values

### Project Mission
[Clear statement of why this project exists and what change it seeks to create]

### Movement Alignment
[How this project serves movement goals and challenges existing power structures]

### Core Values
- **Community Ownership**: [How you ensure community control]
- **Privacy & Security**: [Your approach to protecting users]
- **Accessibility**: [Commitment to inclusive design]
- **Transparency**: [How you maintain democratic accountability]

## Users & Stakeholders

### Primary Users
- **[User Type 1]**: [Their needs and context]
- **[User Type 2]**: [Their needs and context]

### Key Stakeholders
- **[Stakeholder 1]**: [Relationship and considerations]
- **[Stakeholder 2]**: [Relationship and considerations]

### Power Dynamics
[Important context about power relationships, surveillance concerns, or political considerations]

## Technical Context

### Technology Stack
```yaml
Frontend: [Your choices]
Backend: [Your choices]
Database: [Your choices]
Hosting: [Your choices]
Security: [Your approach]
```

### Key Technical Decisions
[Reference to tasks/decisions.md for detailed rationale]
- **[Decision 1]**: [Brief reason]
- **[Decision 2]**: [Brief reason]

### Infrastructure Principles
- [Principle 1 - e.g., "Self-hosted over corporate platforms when feasible"]
- [Principle 2 - e.g., "Canadian data residency for privacy compliance"]

## Development Workflow

### Documentation Structure
- **Active work**: `/tasks/todo.md`
- **Decisions log**: `/tasks/decisions.md`
- **Security reviews**: `/tasks/security.md`
- **Completed work**: `/tasks/archive/`

### Task Management
- Follow patterns in `organizational-patterns.md`
- User story driven development
- Security reviews per feature
- Regular documentation updates

### Code Standards
```javascript
// Prefer clarity over cleverness
// Comment the WHY, not the WHAT
// Consider accessibility in every component
// Security is not optional
```

## Domain-Specific Patterns

### [Pattern Category 1]
[Specific patterns or approaches unique to your domain]

### [Pattern Category 2]
[Additional patterns relevant to your project type]

## Security & Privacy

### Threat Model
- **Primary threats**: [Main security concerns]
- **Secondary concerns**: [Additional considerations]
- **Acceptable risks**: [Documented trade-offs]

### Privacy Approach
- [Data minimization strategies]
- [User consent patterns]
- [Retention policies]

### Security Practices
- Regular dependency audits
- Security review checklist in `/tasks/security.md`
- Incident response plan: [Location or brief description]

## Communication Guidelines

### With Users
- [Tone and approach]
- [Language considerations]
- [Accessibility requirements]

### With Contributors
- [Collaboration style]
- [Decision-making process]
- [Conflict resolution approach]

### Documentation Style
- Plain language explanations
- Multiple examples where helpful
- Progressive disclosure of complexity
- Always consider newcomers

## Constraints & Considerations

### Technical Constraints
- [Resource limitations]
- [Platform requirements]
- [Performance targets]

### Legal/Compliance
- [Relevant legislation - e.g., PIPEDA, CASL]
- [Sector-specific requirements]
- [Compliance documentation location]

### Timeline Pressures
- [Any urgent deadlines]
- [Campaign cycles]
- [Grant requirements]

## Common Tasks

### For Development
1. Check `/tasks/todo.md` for current work
2. Document decisions in `/tasks/decisions.md`
3. Run security checklist for new features
4. Update documentation as you code

### For Maintenance
1. Weekly dependency audits
2. Monthly security reviews
3. Quarterly documentation updates
4. Annual architecture review

### For Onboarding
1. Read this file first
2. Review `/tasks/decisions.md` for context
3. Check recent entries in `/tasks/archive/`
4. Set up development environment per README

## Anti-Patterns to Avoid

### Technical Anti-Patterns
- [Specific to your domain]
- [Based on past learnings]

### Process Anti-Patterns
- Hero developer syndrome
- Documentation debt
- Security as afterthought
- Feature creep without user validation

### Movement Anti-Patterns
- Surveillance features disguised as analytics
- Data hoarding beyond necessity
- Closed-source dependencies for core features
- Platform lock-in without exit strategy

## Getting Help

### Internal Resources
- Team contacts: [How to reach team members]
- Documentation: [Key documents beyond this file]
- Decision history: `/tasks/decisions.md`

### External Resources
- [Relevant movement tech communities]
- [Domain-specific resources]
- [Security resources]

## Contributing Guidelines

### Code Contributions
1. Read relevant documentation first
2. Follow existing patterns
3. Include tests for new features
4. Update documentation
5. Consider security implications

### Documentation Contributions
1. Maintain plain language
2. Include examples
3. Consider newcomers
4. Update table of contents

---

*This document is part of the movement project template. It should evolve with your project while maintaining alignment with movement values.*

*Last Updated: [Date]*
*Template Version: 1.0*