# L06: Web and Network Primer (EO5)
**Objectives:** Understand HTTP request/response basics, status codes, DNS lookup, TCP handshake idea; use curl/httpie.

## Resources
- Watch: NetworkChuck “How the Internet Works” (~20m): https://www.youtube.com/watch?v=x3c1ih2NJEg
- Read: MDN “Overview of HTTP”: https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview
- Guided project: Use httpie tutorial quickstart: https://httpie.io/docs/cli/usage

## Tasks
- Use `http` or `curl -i` to GET a page; identify status code, headers, body.
- Use `nslookup` or `dig` on a domain; note A/AAAA record.
- Describe TCP 3-way handshake conceptually (SYN, SYN-ACK, ACK).
- Make a POST with JSON using httpie or curl.

## Example to Analyze
- Inspect an HTTP response: why are `Content-Type` and `Set-Cookie` important?

## Knowledge Check
- Difference between GET and POST?
- What does DNS solve?
- Why is TLS needed on top of TCP?

## Exit Criteria
- You can explain the flow: browser → DNS → TCP handshake → HTTP request → response.
- You can craft a GET and POST from the CLI and read status codes.
