# Community Organizing Toolkit Example

This example shows how the movement project template adapts to a multi-purpose organizing toolkit used by various community groups.

## Domain Context

**Project Type**: Flexible Organizing Platform
**Users**: Community organizers, volunteers, coalition members
**Timeline**: Continuous with campaign cycles
**Key Constraints**: Multiple group needs, coalition governance, resource sharing

## Template Adaptations

### 1. Threat Model Adjustments

Organizing toolkits face diverse threats:
- **Primary Threats**:
  - State surveillance of movements
  - Corporate opposition research  
  - Infiltration and disruption
  - Data breaches affecting multiple groups
- **Protection Needs**:
  - Coalition member autonomy
  - Campaign strategy security
  - Volunteer safety
  - Action planning confidentiality

### 2. Documentation Structure

```
tasks/
├── README.md                    # Standard template
├── todo.md                      # Feature requests from groups
├── decisions.md                 # Technical decisions
├── security.md                  # Multi-threat security model
├── coalition/                   # Toolkit-specific addition
│   ├── governance.md           # Multi-org decision making
│   ├── data-boundaries.md      # Inter-group data isolation
│   └── resource-sharing.md     # Shared resource protocols
├── features/                    # Toolkit-specific addition
│   ├── event-organizing.md     # Event management module
│   ├── phone-banking.md        # Call tool documentation
│   ├── canvassing.md          # Door knocking features
│   └── petition-tools.md       # Campaign petition system
├── integrations/               # Toolkit-specific addition
│   ├── messaging-apis.md       # SMS/email integration
│   ├── mapping-services.md     # Geographic organizing
│   └── payment-processing.md   # Donation handling
└── archive/
```

### 3. Task Management Adaptations

Toolkit development balances multiple group needs:

```markdown
# todo.md - Organizing Toolkit Version

## Active Sprint: Climate Action Features
_Feb 1-14 - Goal: Ready for March climate mobilization_

### 🚀 In Progress
- [ ] Multi-group event coordination system
  - **Acceptance**: Groups can co-host while maintaining autonomy
  - **Requested By**: Climate Coalition (5 groups)
  - **Data Isolation**: Each group sees only their volunteers
  - **Assignee**: Sam
  - **Coalition Review**: Feb 7

### 📋 Feature Request Queue
Priority based on coalition voting:
1. Accessibility improvements (8 groups requesting)
2. Multilingual support expansion (6 groups)
3. Advanced mapping features (4 groups)
```

### 4. Decision Documentation

Decisions require coalition input:

```markdown
## 2025-01-20: Data Sharing Between Coalition Members

**Context**: Groups want to share volunteer pools for joint actions

**Decision**: Opt-in sharing with granular permissions

**Coalition Process**:
- Proposed at January coalition meeting
- 2-week comment period
- 12 groups in favor, 2 abstentions
- No blocks

**Implementation**:
- Volunteers must consent to each share
- Groups can share: capacity only, contact info, or full profile
- Sharing agreements expire after set time
- Full audit trail maintained

**Review**: After first joint action using system
```

### 5. Multi-Tenancy Patterns

Organizing toolkits need sophisticated isolation:

- Group-level data boundaries
- Shared resource pools (with permissions)
- Coalition-wide features vs group-specific
- Volunteer consent management across groups
- Independent security policies per group

### 6. User Story Patterns

Multi-stakeholder user stories:

```markdown
As a coalition coordinator
I need to organize a city-wide day of action
So that multiple groups can mobilize while maintaining autonomy

Acceptance Criteria:
- [ ] Central event page with group-specific signup
- [ ] Each group manages own volunteers
- [ ] Shared messaging with group customization
- [ ] Aggregate reporting without individual data
- [ ] Post-action data remains with each group
```

## Implementation Patterns

### Core Architecture

#### Multi-Tenant Design
```markdown
## Data Architecture
1. Shared infrastructure, isolated data
2. Group-specific schemas
3. Coalition-wide shared tables
4. Granular permission system
5. Audit trails across boundaries

## Key Principles
- Data sovereignty per group
- Explicit consent for sharing
- No central data aggregation
- Groups can fully export/leave
- Infrastructure collectively owned
```

#### Feature Modularity
```markdown
## Module System
Core Platform:
- User authentication
- Permission management
- Data import/export
- Basic reporting

Optional Modules:
- Event organizing
- Phone banking
- Canvassing
- Petition management
- Email campaigns
- SMS broadcasts
- Donation processing

Groups enable only what they need
```

#### Coalition Governance
```markdown
## Technical Governance Model
1. Feature requests via coalition meetings
2. Priority voting by active groups
3. Security reviews mandatory
4. Consensus for major changes
5. Individual groups can veto for their instance

## Implementation
- Governance dashboard for transparency
- Voting system for priorities
- Change request tracking
- Impact assessment tools
```

### Flexible Features

#### Event Organizing Module
```markdown
## Capabilities
- Public event pages
- Registration management
- Shift scheduling
- Resource coordination
- Multi-group co-hosting

## Privacy Options
- Anonymous registration
- Skill sharing (optional)
- Location fuzzing
- Capacity-only sharing
```

#### Communication Tools
```markdown
## Channels Supported
- Email (with pixel blocking)
- SMS (with opt-out)
- Signal integration
- Print walk lists

## Anti-Surveillance Features
- Message scheduling randomization
- Metadata minimization
- Encryption where possible
- No engagement tracking
```

#### Data Portability
```markdown
## Export Capabilities
- Full data export anytime
- Standard formats (CSV, JSON)
- Relationship preservation
- Media file inclusion
- Encrypted archives

## Import Support
- From other organizing tools
- Spreadsheet uploads
- API migrations
- Merge duplicate detection
```

## Specific File Examples

### CLAUDE.md Adaptation

```markdown
# Community Organizing Toolkit Development Context

## Project Overview
**Project**: People Power Platform
**Type**: Multi-tenant organizing toolkit
**Status**: Active development, 15 groups live
**Coalition**: Progressive Action Network

## Movement Context
Shared infrastructure for interconnected movements:
- Climate justice groups
- Housing organizations
- Labor solidarity
- Immigrant rights
- Indigenous sovereignty

## Technical Principles
- Data sovereignty per group
- Coalition governance model
- Anti-surveillance design
- Maximum flexibility
- Sustainable collectively

[Rest follows template...]
```

### Security Adaptations

```markdown
## Multi-Group Security Considerations

### Threat Modeling per Group Type
- [ ] Environmental: Corporate espionage risk
- [ ] Housing: Landlord surveillance
- [ ] Labor: Employer monitoring
- [ ] Immigration: State surveillance
- [ ] Indigenous: State and corporate

### Cross-Group Security
- [ ] Data isolation verified
- [ ] Permission boundaries tested
- [ ] Audit trails functional
- [ ] Export capabilities secured
- [ ] Coalition agreements enforced
```

### Feature Decision Example

```markdown
## 2025-02-01: Phone Banking System Design

**Context**: Multiple groups need phonebanking for different campaigns

**Requirements Gathered**:
- Climate groups: Persuasion scripts
- Housing orgs: Tenant check-ins
- Labor: Member mobilization

**Decision**: Flexible script system with templates

**Features**:
- Custom fields per campaign
- Disposition tracking
- Shift scheduling
- Results isolation per group
- No call recording (privacy)

**Rejected Options**:
- Predictive dialer (too aggressive)
- AI sentiment analysis (surveillance risk)
```

## Lessons from Coalition Tools

### What Works
1. **Flexibility first** - Groups have different needs
2. **Governance systems** - Technical democracy required
3. **Modular architecture** - Not everyone needs everything
4. **Data boundaries** - Clear isolation with sharing options
5. **Sustainability planning** - Collective funding models

### Common Challenges
1. **Feature creep** - Groups want everything
2. **Governance overhead** - Decisions take time
3. **Security complexity** - Multiple threat models
4. **Resource allocation** - Who pays for what
5. **Technical debt** - Customization accumulation

### Success Metrics
- Groups actively using platform
- Cross-group collaborations
- Data sovereignty maintained
- Security incidents: 0
- Feature adoption rates
- Coalition health scores

## Scaling Patterns

### From 5 to 50 Groups
- Automated onboarding
- Template libraries
- Peer support networks
- Dedicated coalition staff
- Tiered governance model

### Resource Sustainability
- Per-group contributions
- Foundation funding
- Volunteer dev programs
- Training exchanges
- Shared infrastructure costs

---

*This example shows how organizing toolkits require flexible architecture, sophisticated governance, and deep commitment to movement autonomy while enabling powerful collaboration.*