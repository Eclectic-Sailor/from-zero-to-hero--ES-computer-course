# L08: Security Intro (EO7)
**Objectives:** Security mindset, XSS/SQLi demos and mitigations, authN vs authZ.

## Resources
- Read: OWASP Top 10 (overview): https://owasp.org/Top10/
- Labs: PortSwigger Web Security Academy
  - SQLi UNION basic: https://portswigger.net/web-security/sql-injection/union-attacks/lab-determine-number-of-columns
  - Reflected XSS basic: https://portswigger.net/web-security/cross-site-scripting/reflected/lab-html-context-nothing-encoded
- Watch: NetworkChuck SQLi demo (~15m): https://www.youtube.com/watch?v=pWqL-9q1v7g

## Tasks
- Complete the two PortSwigger labs above.
- Write a one-paragraph summary of CIA triad; distinguish authN vs authZ with examples.
- Show a parameterized query in Python (e.g., sqlite3 with `?` placeholders).

## Example to Analyze
```python
cur.execute("SELECT * FROM users WHERE name = ?", (name_input,))
```
Why is this safer than string concatenation?

## Knowledge Check
- What’s the difference between reflected and stored XSS?
- How do parameterized queries stop SQLi?
- What headers/cookie flags help protect sessions?

## Exit Criteria
- Labs completed (screenshot/notes).
- You can explain one mitigation for XSS and one for SQLi.
- You can state the difference between authentication and authorization.
