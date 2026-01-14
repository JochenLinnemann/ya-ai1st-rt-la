# Architectural Decisions – Minimal Service Example

## Decision: Use a Single Service
**Status:** Accepted  
**Context:** The problem domain is small and well-defined.  
**Decision:** Implement the system as a single deployable service.  
**Consequences:**  
- Simpler deployment and debugging  
- Limited independent scaling  
**Date:** 2024-01-01

---

## Decision: Use a Relational Database
**Status:** Accepted  
**Context:** Data has clear structure and relationships.  
**Decision:** Use a relational database as the primary data store.  
**Consequences:**  
- Strong consistency guarantees  
- Schema changes require migrations  
**Date:** 2024-01-01

---

## Decision: Avoid Background Processing Initially
**Status:** Accepted  
**Context:** All operations can complete within request time limits.  
**Decision:** Handle all logic synchronously in the API.  
**Consequences:**  
- Simpler system  
- May need refactoring if workloads grow  
**Date:** 2024-01-01
