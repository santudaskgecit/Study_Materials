# Core Java and Spring Backend Checklist

## Core Java
- OOP: encapsulation, abstraction, inheritance, polymorphism; composition over inheritance.
- SOLID principles and practical examples.
- Interfaces vs abstract classes; records, enums and sealed classes at a high level.
- Collections: List, Set, Map, Queue, Deque; complexity and implementation trade-offs.
- equals/hashCode, immutability, defensive copies and object contracts.
- Generics, wildcards, bounded types and type erasure.
- Exceptions: checked/unchecked, custom exceptions and exception translation.
- Streams, lambdas, functional interfaces, Optional and method references.
- Date/time API, BigDecimal for money, serialization basics.
- Java 17/21 features relevant to your runtime; know records, switch expressions, text blocks and virtual threads conceptually and verify runtime compatibility before using them.

## JVM and performance
- Heap, stack, metaspace, object allocation and garbage collection basics.
- GC goals and trade-offs; diagnose memory leaks and high allocation.
- JIT compilation, class loading and thread dumps.
- Profiling basics: CPU, heap, allocation, latency and throughput.
- Explain how to investigate slow APIs rather than guessing.

## Concurrency
- Thread lifecycle, race conditions, visibility and atomicity.
- synchronized, volatile, locks and atomic classes.
- ExecutorService, thread pools, queue saturation and graceful shutdown.
- CompletableFuture composition and exception handling.
- ConcurrentHashMap and concurrent collections.
- Deadlock conditions and prevention.
- Thread safety, immutable objects and safe publication.
- Virtual threads: when they help, blocking-I/O considerations and limits.

## Spring and Spring Boot
- IoC/DI, bean scopes, lifecycle and configuration.
- Component scanning, auto-configuration and conditional configuration.
- AOP/proxies; self-invocation implications.
- REST controllers, DTOs, validation, exception handling and API versioning.
- Configuration profiles, externalised secrets and configuration management.
- Spring Security basics; OAuth2/JWT resource-server concepts.
- Actuator, health checks, metrics and structured logging.
- Unit/integration testing with JUnit and Mockito; Testcontainers where useful.

## Persistence and data
- SQL joins, grouping, indexes, query plans and normalization.
- Transactions, ACID, isolation levels, locking and deadlocks.
- JPA entity lifecycle, persistence context, lazy/eager loading and N+1.
- Optimistic vs pessimistic locking.
- Pagination, batch operations and connection pools.
- Redis caching: TTL, invalidation, cache stampede and consistency.
- Know when relational, document, key-value or search stores are appropriate.

## API and backend engineering
- HTTP methods/status codes, headers, idempotency and pagination.
- REST resource design, OpenAPI contracts and backward compatibility.
- Authentication vs authorization; least privilege.
- Timeouts, bounded retries with jitter, circuit breakers and bulkheads.
- Input validation, rate limiting, request correlation and auditability.
- Messaging, outbox pattern, duplicate delivery and consumer idempotency.
- Observability: logs, metrics, traces, SLOs and alert quality.

## Practical exercises
Implement a Spring Boot service with CRUD APIs, validation, PostgreSQL persistence, migrations, tests, Docker Compose, health endpoint, structured logs and OpenAPI documentation. Add caching and asynchronous messaging only after the baseline works.
