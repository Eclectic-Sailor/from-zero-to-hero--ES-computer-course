# BL4: Docker 101 + Session/Token/JWT Primer (Pre-K8s/OIDC)
**Purpose:** Ensure container fluency and modern auth concepts before advanced topics.

## Resources
- Video: NetworkChuck Docker intro: https://www.youtube.com/watch?v=eGz9DS-aIeY
- Docker docs Get Started Part 1: https://docs.docker.com/get-started/
- Sessions vs Tokens vs JWT explainer: https://auth0.com/docs/secure/tokens/json-web-tokens/json-web-token-signing-algorithms
- JWT best practices (Auth0): https://auth0.com/docs/secure/tokens/json-web-tokens/json-web-token-best-practices

## Tasks
- Write a minimal Flask/FastAPI app; create a Dockerfile; `docker build -t myapp .` and `docker run -p 8000:8000 myapp`.
- List and remove containers/images (`docker ps`, `docker images`, `docker rm`, `docker rmi`).
- Draw two auth flows: (1) server-managed session cookie; (2) JWT bearer token.
- Implement a tiny protected route using a signed JWT (hardcoded secret) to demonstrate verification.

## Knowledge Check
- When prefer sessions over JWT? (stateful vs stateless trade-offs)
- What should go into JWTs? What should not? (PII, secrets—no)
- Why set token expiry? How to invalidate/rotate?

## Exit Criteria
- You can build/run/stop Docker images locally.
- You can explain session vs token vs JWT and show a working JWT-protected endpoint locally.
