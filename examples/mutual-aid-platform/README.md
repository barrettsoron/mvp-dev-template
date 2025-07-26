# Mutual Aid Platform Example

This example shows how the movement project template adapts to a community mutual aid coordination platform.

## Domain Context

**Project Type**: Mutual Aid Resource Coordination
**Users**: Community members, resource coordinators, aid recipients
**Timeline**: Ongoing, crisis-responsive
**Key Constraints**: Privacy protection, trust building, resource equity

## Template Adaptations

### 1. Threat Model Adjustments

Mutual aid platforms have unique security concerns:
- **Primary Threats**:
  - State surveillance of vulnerable populations
  - Bad actors exploiting aid systems
  - Privacy breaches affecting undocumented folks
- **Trust Requirements**:
  - Community verification without surveillance
  - Protecting recipient anonymity
  - Preventing resource hoarding

### 2. Documentation Structure

```
tasks/
├── README.md                    # Standard template
├── todo.md                      # Feature-based sprints
├── decisions.md                 # Technical decisions
├── security.md                  # Privacy-first security
├── privacy/                     # Mutual aid specific
│   ├── data-minimization.md    # What data we don't collect
│   ├── anonymization.md         # Identity protection strategies
│   └── consent-practices.md    # Respectful consent patterns
├── community/                   # Mutual aid specific
│   ├── safety-protocols.md     # Community safety practices
│   ├── equity-framework.md     # Resource distribution ethics
│   └── trust-building.md       # Verification without surveillance
└── archive/
```

### 3. Task Management Adaptations

Mutual aid platforms emphasize community needs:

```markdown
# todo.md - Mutual Aid Version

## Active Sprint: Winter Preparedness
_Nov 1-15 - Goal: Ready for cold weather needs_

### 🚀 In Progress
- [ ] Anonymous request system for undocumented neighbors
  - **Acceptance**: No PII required for basic needs
  - **Privacy**: IP addresses not logged
  - **Assignee**: Rosa
  - **Community Review**: Nov 5
```

### 4. Decision Documentation

Decisions center on community autonomy and privacy:

```markdown
## 2024-10-20: Request Verification Approach

**Context**: Need to prevent abuse while protecting vulnerable users

**Decision**: Community vouching system over ID verification

**Options Considered**:
1. Government ID - Rejected (excludes undocumented)
2. Phone verification - Rejected (excludes unhoused)
3. Community vouching - Selected

**Rationale**: 
- Builds on existing community trust networks
- Doesn't exclude vulnerable populations
- Prevents surveillance state cooperation

**Review Date**: After 3 months of usage
```

### 5. Privacy Enhancements

Mutual aid requires privacy-first design:

- Data minimization (collect only what's essential)
- Automatic data expiration
- No cooperation with law enforcement
- Anonymous request options
- Decentralized trust networks

### 6. User Story Patterns

Community-centered user stories:

```markdown
As a community member in need
I want to request help without revealing my immigration status
So that I can get support without fear of deportation

Acceptance Criteria:
- [ ] No mandatory identity fields
- [ ] Request possible without account
- [ ] Location can be approximate
- [ ] Communication through platform (no phone required)
```

## Implementation Patterns

### Core Features

#### Anonymous Request System
```markdown
## Design Principles
1. No mandatory personal information
2. Optional secure communication channel
3. Approximate location only (neighborhood level)
4. Time-limited data retention
5. No IP logging
```

#### Resource Matching
```markdown
## Equity Algorithm
1. Priority for repeated unmet needs
2. Geographic distribution fairness
3. Prevent single-user hoarding
4. Transparent matching criteria
5. Community override capability
```

#### Trust Networks
```markdown
## Vouching System
1. Existing members can vouch for new members
2. No central authority verification
3. Multiple vouch paths increase trust
4. Bad actor reporting without surveillance
5. Restorative justice for conflicts
```

### Privacy Practices

#### Data Collection Philosophy
```
COLLECT:
✓ What's needed for resource matching
✓ Approximate location (neighborhood)
✓ Resource types needed/offered
✓ Preferred contact method

DON'T COLLECT:
✗ Legal names
✗ Government IDs
✗ Immigration status
✗ Specific addresses
✗ Income information
✗ Employment details
```

#### Data Retention
- Request data: 90 days
- Message history: 30 days
- Account data: Until user deletion
- No permanent archives
- Automated purging

### Community Safety

#### Preventing Abuse
1. Rate limiting on requests
2. Community flagging system
3. Temporary suspensions (not bans)
4. Restorative justice process
5. No permanent blacklists

#### Building Trust
1. Transparent matching algorithm
2. Community meeting integration
3. Feedback without surveillance
4. Multiple verification paths
5. Gradual trust building

## Specific File Examples

### CLAUDE.md Adaptation

```markdown
# Mutual Aid Platform Development Context

## Project Overview
**Project**: Neighborhood Networks
**Type**: Mutual aid coordination platform
**Status**: Active development
**Communities Served**: East Vancouver neighborhoods

## Movement Context
Community-led response to housing crisis and pandemic impacts:
- Rent support networks
- Food distribution
- Medical supply sharing
- Skills exchange
- Crisis response

## Privacy Requirements
- No cooperation with law enforcement
- No data sharing with government
- Anonymous participation option
- Data minimization
- Community data ownership

[Rest follows template...]
```

### Security Checklist Additions

```markdown
## Mutual Aid Specific Security

### Privacy Protection
- [ ] Anonymous request pathway tested
- [ ] No IP logging verified
- [ ] Data expiration automated
- [ ] Encryption at rest implemented
- [ ] No analytics or tracking

### Community Safety
- [ ] Verification without surveillance
- [ ] Bad actor detection (not tracking)
- [ ] Resource equity algorithms
- [ ] Communication privacy protected
```

### Decision Example

```markdown
## 2024-11-01: Communication System Design

**Context**: Recipients need secure communication with donors

**Decision**: Built-in messaging over phone/email sharing

**Privacy Analysis**:
- Phone numbers expose users to harassment
- Email can be traced to identity
- Platform messaging can be anonymous
- Messages auto-delete after 30 days

**Implementation**: End-to-end encrypted messaging with ephemeral keys
```

## Lessons from Active Networks

### What Works
1. **Privacy first** - Build trust through protection
2. **Community ownership** - Decisions made collectively
3. **Flexible verification** - Multiple trust pathways
4. **Simple interfaces** - Accessible to all skill levels

### Common Challenges
1. **Balancing openness/safety** - Iterative approach needed
2. **Resource equity** - Transparent algorithms help
3. **Volunteer burnout** - Automate what's ethical
4. **Sustainability** - Community funding models

### Success Metrics
- Request fulfillment rate
- Geographic distribution equity
- User privacy incidents: 0
- Community trust scores
- Response time to needs

## Crisis Response Adaptations

During emergencies (fires, heat dome, etc.):
- Streamlined request process
- Increased anonymity options
- Rapid resource mobilization
- Temporary trust relaxation
- Post-crisis security review

---

*This example shows how movement project patterns adapt to the specific needs and values of mutual aid work, prioritizing community autonomy and privacy protection.*