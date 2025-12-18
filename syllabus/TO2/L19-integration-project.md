# L19: Integration Project (EO1–EO7)
**Objectives:** Build a small REST API with database, auth basics, validation, and optional containerization.

## Project
- A CRUD REST API (Flask/FastAPI) with SQL database (SQLite/Postgres), simple auth (session or token), validation, and logging. Containerize if comfortable.

## Resources
- FastAPI tutorial (guided): https://fastapi.tiangolo.com/tutorial/
- Flask quickstart: https://flask.palletsprojects.com/en/latest/quickstart/
- Dockerizing a Python app (guided): https://docs.docker.com/language/python/

## Tasks
- Endpoints: create/read/update/delete for a resource (e.g., tasks).
- DB: schema with PK/FK; parameterized SQL; migrations optional.
- Auth: simple token or session; protect mutating routes.
- Validation: type/length checks; error handling; structured responses.
- Logging: request/response status; avoid sensitive data.
- Optional: Dockerfile + docker-compose with DB.

## Example Code to Analyze
```python
@app.post("/tasks")
def create_task(task: TaskIn, user=Depends(auth_user)):
    cur.execute("INSERT INTO tasks (title, user_id) VALUES (?, ?)", (task.title, user.id))
    conn.commit()
    return {"ok": True}
```
Where would you add validation and error handling?

## Knowledge Check
- How do you protect against SQLi here?
- What HTTP status codes do you return on success/error?
- What belongs in logs vs not?

## Exit Criteria
- API runs locally with working CRUD and auth gate.
- README includes routes, setup steps, and security notes.
- Optional: Docker build succeeds if you attempted containerization.
