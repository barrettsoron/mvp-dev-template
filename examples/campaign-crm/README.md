# Campaign CRM Example

This example shows how the movement project template adapts to a political campaign CRM system.

## Domain Context

**Project Type**: Campaign Relationship Management System
**Users**: Campaign staff, volunteers, candidates
**Timeline**: Tied to election cycles
**Key Constraints**: Electoral law compliance, volunteer coordination, temporal urgency

## Template Adaptations

### 1. Threat Model Adjustments

The security threat model for campaign tools emphasizes:
- **Primary Threats**: 
  - Opposition research and infiltration
  - Donor/volunteer list theft
  - Disinformation attacks
- **Compliance Requirements**:
  - Electoral finance laws
  - Privacy legislation (PIPEDA/CASL)
  - Contribution limit tracking

### 2. Documentation Structure

```
tasks/
├── README.md                    # Standard template
├── todo.md                      # Sprint-based during campaign
├── decisions.md                 # Technical decisions
├── security.md                  # Enhanced security checklist
├── compliance/                  # Campaign-specific addition
│   ├── elections-canada.md      # Federal requirements
│   └── privacy-compliance.md    # CASL/PIPEDA checklist
├── phases/                      # Campaign-specific addition
│   ├── pre-campaign.md         # Setup phase tasks
│   ├── campaign-period.md      # Active campaign tasks
│   └── post-campaign.md        # Wrap-up and archival
└── archive/
```

### 3. Task Management Adaptations

Campaign CRMs use modified task tracking:

```markdown
# todo.md - Campaign Version

## Active Sprint: GOTV Prep
_Sept 15-22 - Goal: Ready for Get Out The Vote phase_

### 🚀 In Progress
- [ ] Implement canvassing quick-entry form
  - **Acceptance**: 15-second entry on mobile
  - **Campaign Priority**: CRITICAL for door knocking
  - **Assignee**: Ana
  - **Deadline**: Sept 18 (canvassing starts Sept 19)
```

### 4. Decision Documentation

Campaign-specific decisions include electoral context:

```markdown
## 2024-08-15: Donation Processing Integration

**Context**: Need to track donations for Elections Canada compliance

**Decision**: Integrate with [Payment processor] for automatic limit tracking

**Compliance Notes**: 
- Individual contribution limit: $1,675
- Real-time tracking required
- Receipts must be immediate

**Review Date**: Post-campaign (cannot change mid-campaign)
```

### 5. Security Enhancements

Campaign CRMs require additional security measures:

- Volunteer access controls (temporary, limited scope)
- Opponent research protection
- Rapid response procedures
- Data retention policies (7 years for financial)

### 6. User Story Patterns

Campaign-specific user stories:

```markdown
As a canvasser
I need to quickly enter contact information at the door
So that I can maintain conversation flow and cover more ground

Acceptance Criteria:
- [ ] Entry takes < 15 seconds
- [ ] Works offline
- [ ] Syncs when connected
- [ ] Handles French names correctly
```

## Implementation Timeline

### Pre-Campaign Phase (Months -6 to -3)
- Build core infrastructure
- Import existing supporter lists
- Train core team
- Security hardening

### Campaign Launch (Month -3)
- Volunteer onboarding features
- Rapid data entry tools
- Compliance reporting

### Active Campaign (Months -3 to 0)
- Daily todo sprints
- Quick response features
- Performance optimization
- GOTV preparation

### Election Period (Final 36 days)
- Feature freeze
- Stability focus
- Rapid issue response
- GOTV execution

### Post-Campaign (Months 0 to +2)
- Data archival
- Compliance reporting
- Lessons learned
- System handoff

## Specific File Examples

### CLAUDE.md Adaptation

```markdown
# Campaign CRM Development Context

## Project Overview
**Project**: VoteForward CRM
**Type**: Federal campaign management system
**Status**: Pre-campaign development
**Election Date**: October 20, 2025

## Movement Context
Progressive campaign challenging incumbent. Focus on:
- Grassroots mobilization
- Small-dollar fundraising
- Volunteer coordination
- Multilingual outreach

## Compliance Requirements
- Elections Canada contribution limits
- CASL compliance for communications
- Financial reporting deadlines
- Bilingual requirements

[Rest follows template pattern...]
```

### Security Checklist Additions

```markdown
## Campaign-Specific Security

### Volunteer Access
- [ ] Temporary access tokens implemented
- [ ] Role-based permissions (canvasser vs staff)
- [ ] Automatic access expiration
- [ ] Activity logging for all volunteers

### Opposition Research Protection
- [ ] Donor lists encrypted
- [ ] Strategy documents access-controlled
- [ ] Communication plans protected
- [ ] Voter ID data segregated
```

## Lessons from Real Campaigns

### What Works
1. **Temporal documentation** - Clear phase-based organization
2. **Rapid task cycles** - Daily updates during campaign
3. **Compliance first** - Built into every feature
4. **Volunteer-friendly** - Assume high turnover

### Common Pitfalls
1. **Over-engineering** - Campaigns need simple, working tools
2. **Ignoring mobile** - Most volunteers use phones
3. **Complex security** - Balance protection with usability
4. **Poor handoff** - Document for post-campaign transfer

### Key Metrics
- Contact entry time: < 30 seconds
- Volunteer onboarding: < 10 minutes
- System uptime: 99.9% during campaign
- Compliance accuracy: 100% required

---

*This example demonstrates how the movement project template adapts to the specific needs of campaign technology while maintaining core organizational patterns.*