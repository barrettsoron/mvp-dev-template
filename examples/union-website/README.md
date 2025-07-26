# Union Website Example

This example shows how the movement project template adapts to a union local's digital infrastructure needs.

## Domain Context

**Project Type**: Union Local Website & Member Portal
**Users**: Union members, stewards, executive, public
**Timeline**: Ongoing with surge periods (negotiations, strikes)
**Key Constraints**: Member privacy, employer surveillance, democratic governance

## Template Adaptations

### 1. Threat Model Adjustments

Union digital infrastructure faces specific threats:
- **Primary Threats**:
  - Employer surveillance of organizing
  - Union busting consultants
  - Member data exposure
  - Strike preparation secrecy
- **Protection Needs**:
  - Bargaining strategy confidentiality
  - Member contact lists security
  - Strike fund information
  - Organizing campaign protection

### 2. Documentation Structure

```
tasks/
├── README.md                    # Standard template
├── todo.md                      # Regular work + campaign surges
├── decisions.md                 # Technical decisions
├── security.md                  # Enhanced for employer surveillance
├── governance/                  # Union-specific addition
│   ├── member-democracy.md     # Democratic feature requirements
│   ├── executive-access.md     # Role-based permissions
│   └── local-bylaws.md         # Technical implementation of bylaws
├── campaigns/                   # Union-specific addition
│   ├── bargaining-prep.md      # Negotiation period features
│   ├── strike-readiness.md     # Strike communication systems
│   └── organizing-tools.md     # New member recruitment
├── compliance/                  # Union-specific addition
│   ├── labor-law.md           # Labor relations board requirements
│   └── financial-reporting.md  # Union financial transparency
└── archive/
```

### 3. Task Management Adaptations

Union projects have regular work + campaign surges:

```markdown
# todo.md - Union Version

## Current Focus: Bargaining Preparation
_Jan 15-31 - Goal: Secure member portal ready for negotiations_

### 🚀 In Progress
- [ ] Implement secure document vault for bargaining committee
  - **Acceptance**: End-to-end encryption, executive-only access
  - **Security**: No employer access possible
  - **Assignee**: Jordan
  - **Labor Sensitivity**: HIGH - contains strategy docs

### 📋 Ready to Start
- [ ] Anonymous workplace issue reporting system
  - **Acceptance**: Members can report without identification
  - **Purpose**: Document contract violations safely
  - **Privacy**: IP anonymization required
```

### 4. Decision Documentation

Union-specific decisions consider labor law and democracy:

```markdown
## 2024-12-10: Member Voting System

**Context**: Need secure, transparent voting for contract ratification

**Decision**: Build custom voting system vs use third-party

**Labor Law Consideration**: 
- Must maintain vote secrecy
- Requires auditable results
- Members only, verified against good standing

**Democratic Principles**:
- One member, one vote
- Transparent counting process
- Results verifiable by scrutineers

**Implementation**: Custom system with paper trail option
```

### 5. Security Enhancements

Union websites require special security measures:

- Member-only sections with strong authentication
- Employer IP blocking during sensitive periods
- Encrypted communication for organizing
- Secure document storage for grievances
- Anonymous reporting systems

### 6. User Story Patterns

Union-specific user stories:

```markdown
As a shop steward
I need to privately document workplace violations
So that we can build grievances without employer retaliation

Acceptance Criteria:
- [ ] Mobile-friendly incident reporting
- [ ] Photo evidence upload capability
- [ ] Timestamp verification
- [ ] Encryption at rest
- [ ] Access limited to grievance committee
```

## Implementation Patterns

### Core Features

#### Member Portal Design
```markdown
## Access Levels
1. Public - Basic union info
2. Member - Verified members only
3. Steward - Workplace representatives
4. Executive - Elected leadership
5. Staff - Union employees

## Verification Without Surveillance
- Member number + custom password
- No employer email addresses
- Optional 2FA via personal device
- Regular access audits
```

#### Strike Communication System
```markdown
## Requirements
1. Rapid broadcast capability
2. Works without employer networks
3. Picket line coordination
4. Strike pay administration
5. Encrypted leadership channels

## Implementation
- SMS for critical updates
- App works offline
- Mesh networking capability
- Paper backup systems
```

#### Democratic Features
```markdown
## Digital Democracy Tools
1. Secure voting systems
2. Motion tracking
3. Meeting minutes access
4. Financial transparency
5. Bylaw-compliant processes

## Transparency + Security
- Public financial summaries
- Detailed reports for members only
- Redacted minutes for sensitive topics
- Audit trails for all changes
```

### Labor-Specific Security

#### Protecting Organizing
```
DURING ORGANIZING CAMPAIGNS:
✓ Enhanced access logging
✓ IP blocking for employer ranges
✓ Encrypted organizer communications
✓ Automatic data expiration
✓ Legal hold capabilities

NEVER:
✗ Log individual page views
✗ Track member behavior
✗ Share data with employers
✗ Allow management access
✗ Compromise member privacy
```

#### Bargaining Security
```markdown
## Negotiation Period Protocols
1. Bargaining team secure vault
2. Strategy documents encryption
3. Proposal version control
4. Secure survey systems
5. Media embargo enforcement

## Technical Implementation
- Separate infrastructure for sensitive docs
- Air-gapped systems for critical data
- Regular security sweeps
- Access sunset after ratification
```

## Specific File Examples

### CLAUDE.md Adaptation

```markdown
# Union Local 123 Website Development Context

## Project Overview
**Project**: Local 123 Digital Infrastructure
**Type**: Union member portal and public website
**Status**: Ongoing maintenance + bargaining prep
**Members**: 2,400 across 15 worksites

## Movement Context
Industrial union representing healthcare workers:
- Current contract expires March 2025
- History of employer surveillance
- Strong democratic traditions
- Multilingual membership (EN/FR/Punjabi)

## Security Requirements
- Employer surveillance resistance
- Member privacy protection
- Bargaining strategy confidentiality
- Strike readiness systems
- Democratic transparency balance

[Rest follows template...]
```

### Security Checklist Additions

```markdown
## Union-Specific Security

### Member Protection
- [ ] Employer IP ranges blocked
- [ ] No work email requirements
- [ ] Anonymous reporting functional
- [ ] Access logs for executives only
- [ ] Regular penetration testing

### Democratic Systems
- [ ] Voting system audited
- [ ] Vote secrecy maintained
- [ ] Results transparency
- [ ] Scrutineer access provided
- [ ] Paper trail capability

### Strike Preparedness
- [ ] Communication system tested
- [ ] Works without employer network
- [ ] Picket coordination secure
- [ ] Strike fund access protected
```

### Decision Example

```markdown
## 2025-01-05: Employer Network Independence

**Context**: Members report employer blocking union site

**Decision**: Multi-channel access strategy

**Implementation**:
1. Primary: Standard web hosting
2. Mirror: Tor hidden service
3. Backup: Email-based system
4. Emergency: SMS gateway
5. Ultimate: Paper systems

**Rationale**: Employers cannot block all channels
**Cost**: Higher complexity accepted for resilience
```

## Lessons from Union Tech

### What Works
1. **Member-first design** - Not just "users"
2. **Democracy built-in** - Technical bylaws compliance
3. **Security culture** - Assume employer surveillance
4. **Solidarity features** - Cross-workplace communication
5. **Paper backups** - Not everyone is digital

### Common Challenges
1. **Multi-generational users** - Wide skill range
2. **Employer blocking** - Need resilient access
3. **Legal requirements** - Labor law compliance
4. **Resource constraints** - Union budgets tight
5. **Volunteer maintenance** - Plan for sustainability

### Success Metrics
- Member portal adoption rate
- Successful votes conducted
- Grievances filed digitally
- Security incidents: 0
- Strike communication reach: 100%

## Collective Bargaining Adaptations

During negotiations:
- Enhanced security protocols
- Rapid feature development
- Member survey systems
- Proposal comparison tools
- Ratification vote preparation

## Strike Mode Features

When job action authorized:
- Public website → Strike headquarters
- Member portal → Picket coordination
- Maximum security enabled
- Real-time communication priority
- Post-strike data archival

---

*This example demonstrates how union digital infrastructure requires special attention to member democracy, employer surveillance resistance, and collective action support.*