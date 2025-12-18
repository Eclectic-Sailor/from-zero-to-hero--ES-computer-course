# L28: Domain-Driven Design Basics (EO5)
**Objectives:** Identify domain model, entities, value objects, aggregates, bounded contexts; layer code accordingly.

## Resources
- Read: “Domain-Driven Design Quickly” (free PDF): https://www.infoq.com/minibooks/domain-driven-design-quickly/
- Watch: Vaughn Vernon DDD talk excerpt (~20m): https://www.youtube.com/watch?v=dnUFEg68ESM

## Tasks
- Pick a feature (e.g., tasks with due dates and tags). Identify entities, value objects, aggregates, and their invariants.
- Define boundaries/bounded contexts if multiple domains.
- Refactor a module into layers: API → application/service → domain → infrastructure.

## Example to Analyze
- Why might “Task” be an entity and “DueDate” a value object?
- What would be the aggregate root?

## Knowledge Check
- What is an aggregate and why does it matter for consistency?
- Difference between entity and value object.
- Why separate domain logic from infrastructure?

## Exit Criteria
- Short doc naming aggregates/boundaries and invariants.
- Code reflects a layered structure for at least one feature.
