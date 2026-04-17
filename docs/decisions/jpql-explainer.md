# JPQL (Jakarta Persistence Query Language) — Quick Explainer

This short note explains what JPQL is, how it differs from raw SQL, and why we used it in the `UserAccountJpaAdapter` implementation.

## What is JPQL?

- JPQL (Jakarta / JPA Query Language) is the object-oriented query language used by JPA providers (e.g., Hibernate).
- JPQL queries operate on entity types and their properties (e.g., `UserAccountEntity.loginIdentifier`), not directly on database tables and columns.
- A JPQL query is translated by the JPA provider into vendor SQL at runtime.

## Key differences vs. raw SQL

- Targets: JPQL targets entity classes and fields; SQL targets tables and columns.
- Portability: JPQL is portable across JPA providers and databases; raw SQL may require vendor-specific adjustments.
- Safety: JPQL keeps data-model concerns at the ORM boundary, reducing direct use of SQL strings in business code.

## Example used in the codebase

The `UserAccountJpaAdapter` uses a JPQL query to look up an account by login identifier:

```java
TypedQuery<UserAccountEntity> q = em.createQuery(
    "SELECT u FROM UserAccountEntity u WHERE u.loginIdentifier = :login",
    UserAccountEntity.class);
q.setParameter("login", loginIdentifier);
```

This is JPQL — note the use of the entity name `UserAccountEntity` and its field `loginIdentifier` rather than a table name or column.

## Alternatives (when you want fewer JPQL strings)

- NamedQuery: declare `@NamedQuery` on the entity and call it by name from the adapter. Keeps the query declaration next to the entity class.

- Criteria API: build queries programmatically with `CriteriaBuilder` for type-safety and no literal strings.

- Native SQL: `createNativeQuery(...)` if you need a specific DB feature or custom SQL — lose portability and should be used sparingly.

## Recommendation for RIAP

- JPQL is idiomatic for JPA/Hibernate and appropriate for the repository-level queries in `p00005`.
- If you prefer to avoid in-code JPQL strings, prefer `@NamedQuery` on entities or use the Criteria API for type-safety.

## Traceability

- This decision is implementation-level and is documented in `docs/decisions/dbms-persistence-approach.md`.
- The `UserAccountJpaAdapter` demonstrates a concise JPQL usage and can be refactored to `@NamedQuery` or Criteria API on request.
