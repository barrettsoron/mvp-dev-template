# Security Review Process

<!--
HOW TO USE:
- Copy to /tasks/security.md to initialize
- Customize threat model for your domain
- Follow review schedule consistently
See /docs/patterns.md for security-as-process pattern
-->

## Threat Model

### Primary Threats
[Specific to your domain - see /docs/reference.md for examples]
- [Threat 1]: [Description and impact]
- [Threat 2]: [Description and impact]

### Secondary Concerns
[Lower priority but still important]
- [Concern 1]: [Description]
- [Concern 2]: [Description]

### Acceptable Risks
[Documented trade-offs]
- [Risk 1]: [Why we accept this risk]

## Security Checklist

### Weekly Review (Fridays)
- [ ] Run dependency audit (`npm audit` / `pip audit` / etc.)
- [ ] Check for security alerts in dependencies
- [ ] Review recent commits for credential exposure
- [ ] Verify backup systems are functioning

### Monthly Review (First Monday)
- [ ] Review user access permissions
- [ ] Check authentication flows
- [ ] Audit data handling practices
- [ ] Review third-party service access

### Quarterly Review (Start of quarter)
- [ ] Full penetration testing (if resources allow)
- [ ] Review and update threat model
- [ ] Security training for team members
- [ ] Document security improvements made

### Per Feature Review
- [ ] Input validation implemented
- [ ] Authentication/authorization checked
- [ ] Data exposure minimized
- [ ] Error handling doesn't leak information

## Security Contacts

**Internal Security Lead**: [Name/Contact]
**External Security Support**: [Organization/Contact if available]
**Incident Response Plan**: [Location of incident response documentation]

## Recent Security Reviews

### YYYY-MM-DD: [Review Type]
**Findings**: [Summary of issues found]
**Actions Taken**: [Steps taken to address]
**Follow-up Date**: [When to review progress]

---

*Security is a process, not a destination. Regular review prevents security debt.*