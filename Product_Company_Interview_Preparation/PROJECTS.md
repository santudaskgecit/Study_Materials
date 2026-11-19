# Portfolio Projects

Build two finished, explainable projects rather than several unfinished demos.

## Project 1: Order Management Backend
**Goal:** demonstrate strong backend engineering independent of a specific commerce vendor.

Suggested stack: Java 17/21, Spring Boot, PostgreSQL, Redis (optional), Kafka (optional), Docker, JUnit/Mockito and OpenAPI.

Features:
- Product, inventory, cart, order and order-status APIs.
- Checkout validates stock and creates an order.
- Idempotency key prevents duplicate order creation.
- Explicit order state machine and validation of legal transitions.
- Transaction boundaries and optimistic locking for inventory.
- Outbox/event publishing for reliable asynchronous updates.
- Retry, timeout and error handling for external payment simulation.
- Tests for concurrency, duplicate requests and failure scenarios.
- Docker Compose, migrations, health checks and concise architecture documentation.

Deliverables: README, architecture diagram, API examples, schema, tests, local run instructions and design trade-offs.

## Project 2: AI Commerce Support Agent
**Goal:** demonstrate practical LLM/RAG/tool integration while reusing commerce-domain knowledge.

Suggested architecture:
- Java Spring Boot backend owns authentication, business rules and tools.
- Product and policy documents are ingested, chunked and embedded.
- PostgreSQL/pgvector stores vectors and metadata.
- RAG answers product/policy questions with source references.
- Read-only tools retrieve order status and product details from mock APIs.
- MCP exposes selected tools through a controlled interface.
- Optional Python/LangGraph service orchestrates a multi-step workflow.
- Human approval is required before any consequential action; initial demo should remain read-only.

Required safeguards:
- Authenticate user and enforce ownership/tenant scope in each tool.
- Validate tool arguments and restrict tool allow-list.
- Treat retrieved content as untrusted; defend against prompt injection.
- Add timeouts, rate limits, token/cost limits and audit logs.
- Evaluate with a small golden question set and record retrieval/answer quality.

## How to present projects
For each project, explain the problem, requirements, architecture, data model, API contract, alternatives, failure modes, security, tests, metrics and what you would improve at larger scale. Be transparent that these are personal learning projects.
