# L09: Integration Mini-Project (EO1–EO7)
**Objectives:** Tie together shell/Git, Python, HTTP, SQL, and basic security notes.

## Project
- Build a Python script that calls a public HTTP API (e.g., Pokémon API), stores selected fields in SQLite, logs actions, and pushes to GitHub.

## Tasks
- HTTP: fetch data with `requests`; handle HTTP errors. (Requests docs: https://requests.readthedocs.io/en/latest/user/quickstart/)
- Data: parse JSON, insert into SQLite with parameterized queries.
- Logging: print timestamps to stdout; optionally to a file.
- Git: commit code and README; push to GitHub.
- Security: avoid hardcoded secrets; validate user inputs (if any); minimal logging (no sensitive data).

## Example Code to Analyze
```python
import requests, sqlite3
conn = sqlite3.connect("data.db")
cur = conn.cursor()
cur.execute("CREATE TABLE IF NOT EXISTS pokemon (id INTEGER, name TEXT)")

resp = requests.get("https://pokeapi.co/api/v2/pokemon/1")
resp.raise_for_status()
data = resp.json()
cur.execute("INSERT INTO pokemon VALUES (?, ?)", (data["id"], data["name"]))
conn.commit()
```
Discuss error handling, parameterized SQL, and logging additions.

## Knowledge Check
- How do you handle a non-200 response?
- How do you prevent SQL injection here?
- What should NOT be committed to Git?

## Exit Criteria
- Repo includes code + README with run steps and sample output.
- Script runs end-to-end and populates SQLite.
- README lists 3 security considerations you accounted for.
