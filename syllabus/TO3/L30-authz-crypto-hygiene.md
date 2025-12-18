# L30: Auth/Z and Crypto Hygiene (EO7)
**Objectives:** Understand JWT/OAuth2/OIDC flows, session vs token trade-offs, TLS/mTLS basics, key management dos/don’ts.

## Resources
- OAuth 2.0/OIDC primer (Auth0): https://auth0.com/docs/get-started/identity-fundamentals/oauth-2-0-and-openid-connect
- JWT best practices (Auth0 docs): https://auth0.com/docs/secure/tokens/json-web-tokens/json-web-token-best-practices
- TLS overview (Wikipedia): https://en.wikipedia.org/wiki/Transport_Layer_Security
- mTLS overview (mutual auth): https://en.wikipedia.org/wiki/Mutual_authentication

## Tasks
- Implement JWT-based auth on your API: login issues token with exp; protected route requires valid token.
- Discuss refresh strategy and token invalidation.
- Diagram implicit vs auth code + PKCE (brief).

## Example to Analyze
```python
token = jwt.encode({"sub": user_id, "exp": ...}, SECRET, algorithm="HS256")
```
What must you validate on incoming tokens?

## Knowledge Check
- When prefer sessions over JWT?
- Why set short expiry and rotate keys?
- High-level difference between TLS and mTLS.

## Exit Criteria
- Protected endpoint using JWT verification.
- Short write-up comparing session vs JWT and noting one mTLS use case.
