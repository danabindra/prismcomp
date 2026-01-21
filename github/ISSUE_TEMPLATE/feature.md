
# [FEATURE] User Authentication Overhaul

## Description
Replace legacy LDAP authentication with Azure AD SSO integration to support 
modern identity management and MFA requirements.

## Business Value
- Reduces helpdesk password reset tickets by ~40%
- Enables MFA compliance for SOC2 audit
- Improves user experience with single sign-on

## Acceptance Criteria
- [ ] Users can authenticate via Azure AD
- [ ] Legacy LDAP removed from codebase
- [ ] Session management updated to JWT
- [ ] MFA enforcement for admin roles
- [ ] Audit logging for all auth events

## Technical Notes
- See spike #142 for Azure AD integration research
- Coordinate with InfoSec on token lifetime policies

## Child Stories
- [ ] #201 - Azure AD integration setup
- [ ] #202 - JWT session management
- [ ] #203 - Admin MFA enforcement
- [ ] #204 - Auth audit logging
- [ ] #205 - Legacy LDAP removal

---
**Labels:** `feature` `auth` `P1-high`  
**Sprint:** Sprint 14  
**Points:** 21 (sum of child stories)  
**Target Release:** v2.4.0  
**Assignee:** @tech-lead
