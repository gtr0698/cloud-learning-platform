# ADR-0001

## Title

Adopt a Modular Monolith Architecture

---

## Status

Accepted

---

## Context

The Cloud Learning Platform is expected to evolve into a large-scale cloud-native system.

At the beginning of the project, the business domain is still evolving and bounded contexts are being refined.

Starting directly with microservices would introduce unnecessary operational complexity and slow down development.

---

## Decision

The application will initially be implemented as a Modular Monolith.

Business capabilities will be isolated into independent modules based on the identified bounded contexts.

Communication between modules will occur through well-defined interfaces.

Future extraction into microservices should require minimal business changes.

---

## Consequences

### Positive

- Simpler development workflow.
- Easier debugging.
- Faster local development.
- Lower infrastructure cost.
- Easier refactoring while the domain evolves.
- Clear migration path toward microservices.

### Negative

- Requires architectural discipline.
- Module boundaries must be respected.
- Future extraction still requires engineering effort.

---

## Alternatives Considered

### Microservices from Day One

Rejected because the domain is still evolving and operational complexity would outweigh the benefits.

---

## References

- Product Vision
- Domain Model
- Bounded Contexts
