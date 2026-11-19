# AI Engineering Roadmap for Backend Engineers

## Positioning
The target is an AI-enabled backend engineer who can integrate LLM capabilities into reliable products. Do not divert the entire preparation plan into model training or advanced mathematics. Strong Java, DSA, backend and system design remain the foundation.

## Concepts to understand
- LLM basics: tokens, context windows, sampling, latency, model limitations and hallucinations.
- Prompt design, system/developer/user instructions and structured outputs.
- Tool/function calling: schemas, validation, authorization and error handling.
- Streaming responses and asynchronous execution.
- Embeddings, vector similarity, chunking and retrieval.
- RAG: ingestion, chunking, embeddings, vector store, metadata filters, retrieval, reranking, context assembly and citations.
- RAG vs fine-tuning: when to choose each; freshness, cost and data ownership.
- Agents vs deterministic workflows; state, tools, memory, planning and human approval.
- MCP: host, client, server, tools, resources and prompts; authentication and permission boundaries.
- Evaluation: golden datasets, retrieval quality, answer relevance, groundedness and regression tests.
- Production concerns: prompt injection, data leakage, PII, tool abuse, rate limits, cost, latency, observability and fallback.

## Suggested technology path
- Keep Java as the primary interview and backend language.
- Learn Spring AI for Java-native model integration, structured output, tools and RAG.
- Learn Python basics sufficient to build small LangGraph workflows and experiments.
- Use PostgreSQL plus pgvector for a practical starter vector store.
- Explore MCP by building a small server exposing a few safe, read-only tools.
- Use a model provider or local model; keep provider-specific code behind an abstraction.

## 12-week AI sequence
- Week 1: LLM concepts, tokens, context, prompts; call a model from a small Java app.
- Week 2: structured output and tool calling; validate all model-provided arguments.
- Week 3: embeddings, cosine similarity and vector search; store metadata.
- Week 4: RAG prototype with chunking, retrieval and citations.
- Week 5: Spring AI model client, advisors, prompt templates and output mapping.
- Week 6: RAG in Spring AI; add metadata filtering and retrieval evaluation.
- Week 7: tool calling and deterministic workflow orchestration.
- Week 8: MCP architecture; implement a minimal server and client interaction.
- Week 9: LangGraph state, nodes, edges, persistence and conditional routing.
- Week 10: multi-step agent workflow with explicit limits and human approval.
- Week 11: security, prompt injection, access control, evaluation and cost controls.
- Week 12: deploy/demo, add metrics/traces, test failure cases and document trade-offs.

## AI interview questions
- What is RAG and why use it instead of fine-tuning?
- How do embeddings and vector similarity work?
- How do you reduce hallucinations and provide grounded answers?
- How do you secure tools an LLM can invoke?
- What is MCP and how is it different from a direct function call?
- When is an agent unnecessary and a deterministic workflow better?
- How do you evaluate RAG quality?
- How do you control latency, token usage and cost?
- How do you protect tenant data and prevent prompt injection?

## Safe engineering rules
Treat retrieved documents and model output as untrusted input. Enforce authorization in backend tools, not in prompts. Use allow-listed tools, schema validation, timeouts, bounded retries, audit logs and human approval for consequential actions. Never let an LLM bypass existing business authorization.
