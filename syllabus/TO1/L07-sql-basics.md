# L07: SQL Basics (EO6)
**Objectives:** Core SELECT/WHERE/JOIN; simple schema design.

## Resources
- SQLBolt lessons 1–6: https://sqlbolt.com/lesson/select_queries_introduction
- SQLZoo SELECT basics: https://sqlzoo.net/wiki/SQL_Tutorial
- Guided practice: freeCodeCamp SQL course: https://www.freecodecamp.org/learn/relational-database/

## Tasks
- Run SQLBolt lessons and solve exercises.
- Write 5 custom queries on a sample DB: filter, join two tables, COUNT with GROUP BY.
- Design a 3-table schema (users, posts, comments) with primary keys and foreign keys.

## Example to Analyze
```sql
SELECT u.name, COUNT(p.id) AS posts
FROM users u
LEFT JOIN posts p ON p.user_id = u.id
GROUP BY u.name
ORDER BY posts DESC;
```
Explain what rows it returns and why LEFT JOIN matters.

## Knowledge Check
- Difference between INNER JOIN and LEFT JOIN?
- What does GROUP BY do?
- Why add an index on a foreign key?

## Exit Criteria
- Queries run correctly on practice DB.
- Schema diagram (even text) that shows PK/FK relationships.
