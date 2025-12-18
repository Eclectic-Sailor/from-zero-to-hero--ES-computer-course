# L18: Secure Web Coding (EO7)
**Objectives:** Input validation, safe database access, session/cookie hygiene, CSRF/XSS mitigations, TLS basics.

## Resources
- OWASP Cheat Sheets: Input Validation and SQL Injection Prevention: https://cheatsheetseries.owasp.org/
- Labs: PortSwigger
  - CSRF no defenses: https://portswigger.net/web-security/csrf/lab-no-defenses
  - Stored XSS basic: https://portswigger.net/web-security/cross-site-scripting/stored/lab-html-context-nothing-encoded
- Cookie flags summary: https://owasp.org/www-community/controls/SecureCookieAttribute
- TLS basics: https://en.wikipedia.org/wiki/Transport_Layer_Security

## Tasks
- Complete the two PortSwigger labs.
- Build/modify a small Flask/FastAPI route to use parameterized SQL; add input validation (type/length).
- If using forms, add a CSRF token (e.g., simple hidden token check).
- Configure cookies with HttpOnly and Secure flags (where applicable).

## Example Code to Analyze
```python
response.set_cookie("session", token, httponly=True, secure=True, samesite="Lax")
```
What does each flag do?

## Knowledge Check
- Difference between reflected and stored XSS?
- What breaks CSRF?
- Why is TLS certificate validation important?

## Exit Criteria
- Labs completed.
- Route uses parameterized queries and input validation.
- You can explain cookie flags and one TLS takeaway (cert chain).
