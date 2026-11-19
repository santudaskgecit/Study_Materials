# System Design: HLD, LLD and Distributed Systems

## High-level design interview framework
1. Clarify functional requirements and explicit non-goals.
2. Identify users, APIs and key user journeys.
3. Estimate scale: users, requests/second, storage, payload sizes and read/write ratio.
4. Define data model and access patterns.
5. Draw the high-level architecture and request/data flows.
6. Deep dive into bottlenecks, consistency, failure handling and security.
7. Discuss trade-offs and evolution; do not add technology without a reason.

## Core concepts
- Horizontal vs vertical scaling; stateless services and load balancing.
- API gateway, service discovery and service boundaries.
- SQL vs NoSQL, indexes, replication, partitioning and sharding.
- Cache-aside, write-through, TTL, invalidation and hot keys.
- Queues/streams, Kafka fundamentals, ordering, partitions and consumer groups.
- At-most-once, at-least-once and effectively-once processing; idempotency.
- CAP theorem, consistency models, quorum concepts and eventual consistency.
- Distributed transactions, Saga and transactional outbox.
- Timeouts, retries with exponential backoff/jitter, circuit breakers and bulkheads.
- Rate limiting, backpressure, load shedding and graceful degradation.
- Multi-region considerations, disaster recovery, RPO/RTO.
- Authentication, authorization, encryption, secrets and audit trails.
- Observability: logs, metrics, distributed tracing and SLOs.

## HLD practice designs
1. URL shortener.
2. Rate limiter.
3. Notification service.
4. Chat/messaging platform.
5. E-commerce product catalogue and search.
6. Cart, checkout and order management.
7. Payment processing and ledger.
8. Inventory/reservation service.
9. Ride booking or food delivery.
10. File upload/storage service.

For each design, prepare APIs, schema, scale assumptions, architecture, critical sequence, failure cases, consistency requirements and two alternatives with trade-offs.

## LLD principles
- SOLID, encapsulation, composition and interface-driven design.
- Separate domain logic from infrastructure and transport.
- Use patterns only when they simplify change: Strategy, Factory, Builder, Adapter, Observer, Decorator and State.
- Model state transitions explicitly; validate invariants.
- Design for testability and dependency injection.

## LLD exercises
- Parking lot, elevator, movie booking, food ordering, payment gateway, inventory management and Splitwise.
For each: clarify requirements, identify entities, define interfaces, draw relationships, implement core flows, handle concurrency and write tests.

## Project deep-dive prompts
Use your commerce integration experience to explain pricing and calculation provider boundaries, cart/checkout lifecycle, stateful vs stateless calls, API contracts, retries, fallbacks, idempotency, data mapping, observability and failure recovery. Explain decisions and trade-offs without exposing confidential code or customer details.
