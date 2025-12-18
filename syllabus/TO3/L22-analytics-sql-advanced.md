# L22: Analytics and SQL Advanced (EO2)
**Objectives:** Window functions, CTEs, data cleaning, basic visualization/storytelling.

## Resources
- DuckDB (in-Python) quickstart: https://duckdb.org/docs/api/python/overview.html
- SQLite quickstart: https://www.sqlite.org/cli.html
- SQL window functions guide: https://mode.com/sql-tutorial/sql-window-functions/
- Matplotlib getting started: https://matplotlib.org/stable/users/getting_started/
- Seaborn tutorial: https://seaborn.pydata.org/tutorial.html

## Tasks
- Run queries with window functions (top-N per group, rolling average).
- Use a public dataset (CSV) and run CTE + window queries (DuckDB in Python is easy).
- Clean data: handle missing values, type conversions.
- Visualize 2 key insights with plots; write a short narrative.

## Example Query to Analyze
```sql
WITH ranked AS (
  SELECT user_id, score,
         ROW_NUMBER() OVER (PARTITION BY user_id ORDER BY score DESC) AS rn
  FROM scores
)
SELECT * FROM ranked WHERE rn = 1;
```
What does this return and why?

## Knowledge Check
- Difference between GROUP BY and window functions.
- When to use CTEs vs subqueries.
- Why document data cleaning steps?

## Exit Criteria
- Two working window queries + plots with brief written insights.
- You can explain the output of a ROW_NUMBER/LAG query.
