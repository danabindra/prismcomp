
# [BUG] Session timeout not redirecting to login

## Bug Report
**Reported By:** CRM #4521 (customer: County of Sisson )  
**Reported Date:** 2026-01-18  
**Environment:** Production  
**Severity:** P1-high (blocking user workflows)

## Description
Users report that after session timeout (30 min inactivity), the application 
shows a blank white screen instead of redirecting to the login page. Requires 
manual browser refresh to recover.

## Steps to Reproduce
1. Log in to application
2. Leave browser idle for 30+ minutes
3. Attempt any action (click button, navigate)
4. **Expected:** Redirect to login with "Session expired" message
5. **Actual:** Blank white screen, console shows 401 errors

## Environment Details
- Browser: Chrome 120, Firefox 121, Edge 120 (all affected)
- OS: Windows 11, macOS Sonoma
- Application Version: v2.3.1

## Logs/Screenshots
