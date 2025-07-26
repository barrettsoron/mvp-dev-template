# Setup Guide: Adapting the Movement Project Template

This guide walks you through adapting this template to your specific project needs while maintaining movement values and organizational patterns.

## Prerequisites

Before starting:
- Clear understanding of your project's domain and goals
- Identified user communities and their needs
- Basic threat model (who/what are you protecting against)
- Team structure and decision-making process

## Step-by-Step Setup Process

### Step 1: Initial Template Copy

```bash
# Copy the template to your project directory
cp -r /path/to/movement-project-template /path/to/your-project

# Initialize git repository
cd /path/to/your-project
git init
git add .
git commit -m "Initial commit from movement project template"
```

### Step 2: Domain Context Assessment

Answer these questions to guide your adaptation:

**Project Type**:
- [ ] Campaign/Electoral tool
- [ ] Community organizing platform
- [ ] Mutual aid coordination
- [ ] Union organizing tool
- [ ] Advocacy/Education site
- [ ] Other: ___________

**Primary Users**:
- [ ] Organizers/Staff
- [ ] Volunteers
- [ ] Community members
- [ ] General public
- [ ] Coalition partners

**Security Context**:
- [ ] High-risk (state surveillance concern)
- [ ] Medium-risk (corporate/employer surveillance)
- [ ] Low-risk (public organizing)

**Scale Expectations**:
- [ ] Individual/Small team (1-5 people)
- [ ] Medium organization (5-50 people)
- [ ] Large organization/Coalition (50+ people)

### Step 3: Customize Core Files

#### 3.1 Project README.md

Replace the template README with your project-specific version:

```markdown
# [Your Project Name]

[One-line description aligned with movement values]

## About This Project

### Mission
[Why this project exists - connect to movement goals]

### Who We Serve
[Specific communities and their needs]

### Core Values
- [Adapted from template values]
- [Specific to your domain]

## Getting Started
[Project-specific setup instructions]

## Documentation
- See `/tasks/README.md` for our documentation structure
- Current work tracked in `/tasks/todo.md`
- Technical decisions in `/tasks/decisions.md`
```

#### 3.2 CLAUDE.md (AI Context File)

Create from template, customizing:

```markdown
# [Project Name] AI Assistant Context

## Project Overview
[Brief description of project purpose and domain]

## Movement Context
[Specific political/organizing context]
[Key stakeholders and power dynamics]

## Technical Context
[Technology stack choices]
[Infrastructure decisions]
[Security requirements]

## Working Principles
1. [Domain-specific principles]
2. [Adapted from template]

## Documentation Standards
- Follow patterns in organizational-patterns.md
- Maintain decision log in tasks/decisions.md
- Security reviews via tasks/security.md

## Domain-Specific Patterns
[Patterns unique to your project type]
```

#### 3.3 Task Documentation Structure

Set up your `/tasks/` directory:

1. **tasks/README.md** - Keep the template version, it's domain-agnostic

2. **tasks/todo.md** - Initialize with your first tasks:
```markdown
# Current Development Tasks

## Active Sprint: [Sprint Name]
_[Dates] - [Sprint Goal]_

### In Progress
- [ ] Initial setup and configuration
  - Acceptance: Development environment running
  - Assignee: [Name]
  
### Planned
- [ ] First user story implementation
  - Acceptance: [Specific criteria]
  - Estimate: [Time]

### Blocked
_None_

## Backlog
[Future tasks from your planning]
```

3. **tasks/decisions.md** - Start your decision log:
```markdown
# Technical Decisions Log

## YYYY-MM-DD: Project Technology Stack

**Decision**: [Specific choices made]

**Context**: [Why these choices for this domain]

**Options Considered**:
1. Option A - [Pros/Cons]
2. Option B - [Pros/Cons]

**Rationale**: [Why this serves our users/movement]

**Review Date**: [When to reassess]
```

### Step 4: Select and Study Examples

Review relevant examples from `/examples/` directory:

#### For Campaign/Electoral Tools:
- Study campaign-crm example
- Note: Electoral law compliance, temporal nature, volunteer coordination

#### For Mutual Aid Platforms:
- Study mutual-aid-platform example  
- Note: Privacy emphasis, resource distribution, community autonomy

#### For Union Tools:
- Study union-website example
- Note: Security hardening, member democracy, employer surveillance

### Step 5: Implement Security Baseline

1. **Create .claudeignore** from template
2. **Initialize security.md** with your threat model:

```markdown
# Security Review Process

## Threat Model
**Primary Threats**:
- [Specific to your domain]

**Secondary Concerns**:
- [Lower priority but still important]

## Security Checklist
[Adapted from template for your needs]

## Review Schedule
- Weekly: [Specific checks]
- Monthly: [Broader review]
- Per Release: [Full audit]
```

### Step 6: Establish Workflows

#### Daily Workflow
```bash
# Start of day
- Review tasks/todo.md
- Check for blockers
- Update task status

# During development  
- Document decisions as they happen
- Note security considerations
- Consider user impact

# End of day
- Update task progress
- Note any decisions made
- Identify tomorrow's priorities
```

#### Weekly Workflow
- Archive completed tasks with learnings
- Review and update documentation
- Security dependency check
- Team sync on decisions

### Step 7: Domain-Specific Adaptations

Based on your project type, add specific patterns:

#### Campaign Tools Need:
- Temporal documentation (pre/during/post campaign)
- Volunteer onboarding guides
- Compliance checklists
- Rapid response procedures

#### Mutual Aid Platforms Need:
- Resource distribution protocols
- Community safety guidelines
- Privacy-first data handling
- Distributed decision making

#### Union Tools Need:
- Legal compliance tracking
- Member democracy features
- Strike/action preparedness
- Employer surveillance countermeasures

### Step 8: Create Your First Feature

Follow this process:

1. **Write User Story**
```markdown
As a [user type]
I need [capability]
So that [movement goal]

Acceptance Criteria:
- [ ] Specific testable criteria
- [ ] Accessibility requirement
- [ ] Privacy consideration
```

2. **Break Into Tasks** (add to todo.md)
3. **Document Decisions** (update decisions.md)
4. **Implement with Comments**
5. **Security Review**
6. **Archive Learnings**

## Customization Examples

### Example 1: Campaign CRM Adaptation

**Key Adaptations**:
- Added electoral district data structure
- Temporal task tracking (pre/during/post election)
- Volunteer shift management patterns
- Donation compliance workflows

**File Structure Additions**:
```
tasks/
├── compliance/
│   ├── elections-canada.md
│   └── privacy-legislation.md
├── volunteer-guide.md
└── campaign-phases.md
```

### Example 2: Mutual Aid Platform Adaptation

**Key Adaptations**:
- Anonymous request system design
- Resource matching algorithms
- Community verification patterns
- Distribution equity tracking

**File Structure Additions**:
```
tasks/
├── privacy/
│   ├── anonymization.md
│   └── data-minimization.md
├── community-safety.md
└── resource-protocols.md
```

## Common Pitfalls to Avoid

### 1. Over-Customization
Keep core workflows intact - they're based on proven patterns

### 2. Under-Documentation
Better to over-document initially and prune later

### 3. Ignoring Security
Security-as-process means starting from day one

### 4. Solo Decision Making
Document decisions even in small teams

## Getting Help

### When Stuck:
1. Review organizational-patterns.md for workflow guidance
2. Check examples/ for similar projects
3. Return to movement values for direction
4. Document the challenge for future reference

### Contributing Back:
When you discover patterns that work:
1. Document them thoroughly
2. Abstract from your specific domain
3. Consider contributing to template
4. Share with movement community

---

*Remember: The template is a starting point. Your domain expertise and movement knowledge will shape it into something powerful for your community.*