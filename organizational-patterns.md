# Organizational Patterns for Movement Technology

This document outlines the core workflows and principles that make movement technology projects sustainable, democratic, and effective.

## Core Workflow Patterns

### 1. Decision Documentation Pattern

**Purpose**: Create institutional memory and democratic accountability

**Structure**:
```yaml
Date: YYYY-MM-DD
Decision: What was decided
Context: Why this decision was needed
Options_Considered:
  - Option A with pros/cons
  - Option B with pros/cons
Rationale: Why we chose this option
Impact: How this affects users/community
Review_Date: When to revisit this decision
```

**Key Principles**:
- Document decisions AS they happen, not after
- Include dissenting opinions and concerns
- Set review dates for major decisions
- Link to relevant user stories or issues

**Example Applications**:
- Technology stack choices
- Data storage decisions
- API design patterns
- Security trade-offs

### 2. Task Management Cascade

**Purpose**: Connect strategic vision to daily work

**Three-Layer System**:

#### Strategic Layer (high-level-tasks.md)
- User story driven development
- Long-term roadmap planning
- Cross-functional dependencies
- Resource estimation

#### Tactical Layer (todo.md)
- Current sprint/week tasks
- Concrete, actionable items
- Single responsibility focus
- Clear acceptance criteria

#### Archive Layer (archive/)
- Completed work documentation
- Lessons learned capture
- Performance metrics
- Future reference material

**Workflow**:
1. Strategic planning creates user stories
2. User stories decompose into tasks
3. Tasks get pulled into current todo
4. Completed tasks move to archive with learnings

### 3. Security-as-Process Pattern

**Purpose**: Iterative security improvement without perfection paralysis

**Regular Review Cycle**:
```bash
# Weekly: Dependency checks
npm audit / pip check / bundler audit

# Monthly: Access review
- Who has access to what?
- Are permissions still appropriate?
- Any terminated team members?

# Quarterly: Full security audit
/security command or manual checklist
- Credential exposure scan
- Input validation review
- Authentication flow check
- Data handling practices
```

**Security Decision Framework**:
1. **Threat Model First**: Who are we protecting against?
2. **Movement Context**: State surveillance vs corporate extraction
3. **User Impact**: Security vs usability trade-offs
4. **Implementation Cost**: Perfect vs good enough
5. **Review Schedule**: When to reassess

### 4. Documentation Rhythm

**Purpose**: Keep documentation alive and useful

**Daily**:
- Update todo.md with progress
- Note any blockers or decisions

**Weekly**:
- Archive completed tasks
- Update technical decisions
- Review security alerts

**Per Feature**:
- Document in user story format
- Include acceptance criteria
- Note accessibility requirements
- Consider privacy implications

**Per Release**:
- Update CHANGELOG.md
- Review all documentation
- Archive old decisions
- Plan next cycle

## Movement-Specific Patterns

### 1. Community Ownership Pattern

**Documentation Approach**:
- Plain language explanations
- Multiple examples
- Visual diagrams where helpful
- Glossary of technical terms

**Code Practices**:
- Extensive inline comments
- Example usage in every module
- Setup scripts that explain themselves
- Error messages that educate

### 2. Coalition Technology Pattern

**When Multiple Organizations Share Infrastructure**:

**Governance Documentation**:
```yaml
Coalition_Members:
  - Organization A (role/responsibilities)
  - Organization B (role/responsibilities)
  
Decision_Process:
  Minor_Changes: Single org approval
  Major_Changes: Consensus required
  Emergency_Fixes: Any org can act
  
Data_Ownership:
  - Each org owns their data
  - Shared data requires agreement
  - Export rights guaranteed
```

**Technical Implementation**:
- Multi-tenant architecture docs
- Data isolation strategies
- Permission system design
- Audit trail requirements

### 3. Campaign Urgency Pattern

**Balancing Speed with Sustainability**:

**Pre-Campaign**:
- Build robust foundation
- Document everything
- Train multiple people
- Create runbooks

**During Campaign**:
- Quick decisions with documentation
- Daily standups
- Defer non-critical improvements
- Focus on user-facing features

**Post-Campaign**:
- Technical debt paydown
- Documentation cleanup
- Knowledge transfer
- Archive campaign-specific code

### 4. Privacy-First Development Pattern

**Every Feature Considers**:
1. What data is actually needed?
2. How long must we keep it?
3. Who needs access?
4. Can it be anonymized?
5. Export/deletion capabilities?

**Documentation Requirements**:
- Data flow diagrams
- Retention policy matrices
- Access control lists
- Anonymization strategies

## Anti-Patterns to Avoid

### 1. Hero Developer Pattern
**Problem**: One person knows everything
**Solution**: Pair programming, documentation requirements, rotation

### 2. Perfect is the Enemy Pattern
**Problem**: Waiting for perfect security/features
**Solution**: Iterative improvement, documented trade-offs

### 3. Technical Solutionism Pattern
**Problem**: Building tech for tech's sake
**Solution**: User story driven, community feedback loops

### 4. Extraction Creep Pattern
**Problem**: Gradually adding surveillance features
**Solution**: Regular values alignment reviews, community oversight

## Adaptation Guidelines

### For Different Domains

**Campaign Tools**:
- Emphasis on temporal documentation
- Rapid iteration patterns
- Compliance checklists
- Volunteer onboarding

**Mutual Aid Platforms**:
- Privacy-first patterns
- Distributed governance docs
- Resource sharing protocols
- Community safety practices

**Union Organizing Tools**:
- Security hardening emphasis
- Legal compliance tracking
- Member democracy features
- Strike preparation modes

**Community Websites**:
- Accessibility-first patterns
- Multilingual considerations
- Sustainable hosting docs
- Community moderation

### For Different Scales

**Individual Projects**:
- Simplified todo tracking
- Personal decision journal
- Basic security checklist

**Small Teams**:
- Shared documentation
- Review processes
- Knowledge sharing

**Large Organizations**:
- Formal governance
- Audit trails
- Training programs

## Success Indicators

### Technical Health
- Documentation stays current
- New team members onboard quickly
- Security improves over time
- Technical debt stays manageable

### Movement Alignment
- Communities own their data
- Features serve organizing needs
- Privacy preserved by default
- Democratic participation enabled

### Sustainability
- Multiple people can maintain
- Knowledge is preserved
- Burnout is prevented
- Growth is possible

---

*These patterns emerge from movement technology practice. Adapt them to your context while maintaining their democratic spirit.*