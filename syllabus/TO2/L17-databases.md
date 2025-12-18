# L17: Databases (EO6)
**Objectives:** ACID, normalization, indexing; queries with joins/aggregates.

## Resources
- “Use the Index, Luke” (intro): https://use-the-index-luke.com/
- Normal forms quick summary (1NF–3NF): https://www.guru99.com/database-normalization.html
- Video: Normalization explained (Traversy Media, ~12m): https://www.youtube.com/watch?v=UrYLYV7WSHM

## Tasks
- Design schema for a small app (e.g., tasks, users, tags).
- Write queries: multi-table JOINs, aggregates (COUNT, AVG), GROUP BY with HAVING.
- Add an index on a frequently filtered column; explain expected benefit.

## Example to Analyze
```sql
BEGIN;
UPDATE accounts SET balance = balance - 100 WHERE id = 1;
UPDATE accounts SET balance = balance + 100 WHERE id = 2;
COMMIT;
```
Why do we wrap this in a transaction?

## Knowledge Check
- What does each ACID letter mean?
- When do you denormalize?
- Why can indexes speed reads but hurt writes?

## Exit Criteria
- Schema diagram (text or image) showing PK/FK.
- 5 working queries with joins/aggregates.
- Short note on where an index helps in your schema.
