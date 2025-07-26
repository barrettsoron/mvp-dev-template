# Domain Adaptation Reference

This guide shows how to adapt the movement project template to different organizing domains. Rather than separate examples, this consolidated reference shows key adaptation patterns for four common domains.

## Setup Process

1. **Copy this template** to your project directory
2. **Copy `/templates/CLAUDE.md`** → `/CLAUDE.md` and customize
3. **Copy task templates** from `/templates/tasks/` → `/tasks/`
4. **Adapt patterns below** to your specific domain and context

## Domain Adaptations

### Campaign CRM / Electoral Tools

**Context**: Political campaign management systems tied to election cycles

**Key Adaptations**:
- **Temporal Documentation**: Pre-campaign setup, active campaign, post-campaign archival
- **Compliance Focus**: Electoral finance laws, privacy legislation (PIPEDA/CASL), contribution limits
- **Security Priorities**: Opposition research protection, donor/volunteer list security, disinformation defense

**Task Structure**:
```
tasks/
├── compliance/
│   ├── elections-canada.md      # Federal requirements
│   └── privacy-compliance.md    # CASL/PIPEDA checklist
├── phases/
│   ├── pre-campaign.md         # Setup phase
│   ├── campaign-period.md      # Active campaign
│   └── post-campaign.md        # Wrap-up and archival
```

**Decision Log Focus**: Technology choices must consider rapid deployment, volunteer training ease, post-campaign data handling

### Mutual Aid Platform

**Context**: Community resource distribution and mutual support systems

**Key Adaptations**:
- **Privacy-First Design**: Anonymous request systems, minimal data collection, community verification
- **Distributed Governance**: Consensus decision-making, community ownership, resource equity tracking
- **Safety Emphasis**: Community protection, anti-surveillance, vulnerable population consideration

**Task Structure**:
```
tasks/
├── privacy/
│   ├── anonymization.md        # Data anonymization strategies
│   └── data-minimization.md    # Minimal collection policies
├── community-safety.md         # Protection protocols
└── resource-protocols.md       # Distribution guidelines
```

**Decision Log Focus**: Every technical choice evaluated for community autonomy, surveillance resistance, equity impact

### Union / Labor Organizing Tools

**Context**: Worker organizing infrastructure and member democracy platforms

**Key Adaptations**:
- **Security Hardening**: Employer surveillance countermeasures, secure communications, member protection
- **Democratic Processes**: Member voting systems, transparent governance, participatory decision-making
- **Legal Compliance**: Labor law requirements, member privacy rights, strike preparation protocols

**Task Structure**:
```
tasks/
├── security/
│   ├── employer-surveillance.md # Threat assessment
│   └── secure-communications.md # Protected channels
├── democracy/
│   ├── voting-systems.md        # Member democracy
│   └── transparency.md          # Governance accountability
└── legal-compliance.md          # Labor law requirements
```

**Decision Log Focus**: Technology choices must support worker power, resist employer interference, enable democratic participation

### Coalition / Multi-Group Platform

**Context**: Shared infrastructure serving multiple organizations

**Key Adaptations**:
- **Multi-Tenant Governance**: Organizational boundaries, shared decision-making, resource allocation
- **Data Sovereignty**: Each organization owns their data, export rights guaranteed, clear permissions
- **Scalable Security**: Organization-level threat models, graduated access controls, audit trails

**Task Structure**:
```
tasks/
├── governance/
│   ├── coalition-agreement.md   # Multi-org coordination
│   └── decision-processes.md    # Consensus mechanisms
├── data-sovereignty/
│   ├── org-boundaries.md        # Data isolation
│   └── export-rights.md         # Guaranteed portability
└── multi-tenant-security.md     # Organization-level controls
```

**Decision Log Focus**: Technology architecture must serve coalition needs without privileging any single organization

## Common Adaptation Patterns

### Documentation Customization

**CLAUDE.md Context**:
```markdown
## Project Overview
**Type**: [Campaign tool / Mutual aid platform / Union organizing / Coalition platform]
**Primary Users**: [Staff / Volunteers / Members / Organizations]
**Security Context**: [High-risk / Medium-risk / Low-risk]

## Domain-Specific Values
- [Adapted core values for your domain]
- [Specific to your organizing context]

## Key Constraints
- [Legal/compliance requirements]
- [Timeline pressures]
- [Resource limitations]
```

### Task Management Adaptations

**Campaign Tools** → Sprint-based during active periods, compliance checklists, rapid iteration

**Mutual Aid** → Consensus-driven planning, community safety reviews, resource equity tracking

**Union Tools** → Member democracy integration, security-first development, legal compliance tracking

**Coalition Work** → Multi-org coordination, shared resource planning, distributed decision-making

### Security Model Adaptations

**Campaign Tools**:
- Primary Threats: Opposition research, voter suppression, disinformation
- Key Protections: Donor privacy, volunteer safety, electoral integrity

**Mutual Aid**:
- Primary Threats: State surveillance, community infiltration, vulnerable population exposure
- Key Protections: Request anonymity, distribution security, community autonomy

**Union Tools**:
- Primary Threats: Employer surveillance, union-busting, member intimidation
- Key Protections: Communication security, member privacy, organizing information

**Coalition Work**:
- Primary Threats: Inter-org conflicts, external surveillance, resource disputes
- Key Protections: Data sovereignty, decision transparency, equitable access

## Quick Start Checklist

### For Any Domain
- [ ] Copy and customize CLAUDE.md with your domain context
- [ ] Set up tasks/ directory with core templates
- [ ] Document your specific threat model in tasks/security.md
- [ ] Create initial decisions.md entry explaining domain adaptation choices
- [ ] Set up weekly/monthly review cycles appropriate to your timeline

### Domain-Specific Setup
- [ ] **Campaign**: Add compliance/ and phases/ subdirectories
- [ ] **Mutual Aid**: Add privacy/ subdirectory and community safety protocols
- [ ] **Union**: Add security/ and democracy/ subdirectories
- [ ] **Coalition**: Add governance/ and data-sovereignty/ subdirectories

### First Sprint Tasks
- [ ] Define user stories for your specific community
- [ ] Set up development environment with security baselines
- [ ] Document key stakeholders and decision-making processes
- [ ] Establish regular review cycles (daily/weekly/monthly)

---

*Adapt these patterns to your specific context while maintaining their democratic and organizing-centered spirit.*