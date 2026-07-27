# Argenis Vargas — Principal Engineer | Integration & Distributed Systems Architect

Backend Engineer and Systems Architect with 9+ years of experience specializing in high-throughput distributed systems, event-driven architectures, GraphQL federation, and cloud integrations (GCP & AWS).

Formerly Principal Software Engineer & Tech Architecture, designing and scaling multi-tenant B2B systems for 20,000+ users.

---

## What I actually do

- Design **event-driven pipelines** using GCP Pub/Sub and AWS SNS→SQS fan-out patterns for async batch execution.
- Build and unify domain APIs with **Strawberry + Apollo Federation**, resolving N+1 bottlenecks and decoupling core systems.
- Optimize **PostgreSQL & Django ORM at scale** — refactoring bulk transactional workflows (e.g., from 120K individual queries down to 8 bulk operations).
- Design **resilient async pipelines** that cut processing times from **3.6 hours to 26 minutes** with strict idempotency guarantees.
- Build **streaming Excel and CSV exports** for datasets of 80K+ rows without OOM — using server-side cursors, sequential memory phases, and explicit release.
- Implement **resiliency patterns** (Circuit Breaker, Exponential Backoff, Connection Pooling) for cross-system fault tolerance.
- Drive **observability and monitoring** across distributed interfaces using Prometheus, structured logging, and distributed tracing.

---

## Engineering principles I live by

1. **A loop with DB queries is an incident in waiting.**
   If there is a `for` loop issuing queries inside, it’s a scale bottleneck ready to explode. Refactor to bulk set operations early.

2. **Think in sets, not in items.**
   The difference between $O(N)$ and $O(1)$ usually lies in reformulating the problem statement, not micro-optimizing the loop body.

3. **Logic bugs are far more dangerous than performance bugs.**
   A slow query annoys users; a process that silently corrupts transactional data destroys business trust.

4. **The event loop does not forgive synchronous ORM blocking.**
   Proper async boundary management (`sync_to_async`) isn't an afterthought when mixing Django with async processing — it's core architecture.

5. **Explicit memory management in long-running pods isn't micro-optimization.**
   When operating near RAM thresholds in containerized environments, relying solely on garbage collection lead to unpredictable OOM crashes.

---

## Core Stack & Tooling

```python
languages   = ["Python 3.12", "Go (Exploring)"]
frameworks  = ["Django", "FastAPI", "Strawberry GraphQL"]
databases   = ["PostgreSQL", "Redis"]
cloud_infra = ["GCP (Pub/Sub, Cloud Run, GKE)", "AWS (S3, SQS, SNS)", "Terraform", "Kubernetes"]
patterns    = ["Distributed Systems", "Event-Driven Architecture", "GraphQL Federation",
               "Domain-Driven Design (DDD)", "Idempotency & Resiliency", "Bulk Operations"]
observability = ["Prometheus", "Distributed Tracing", "Structured Logging"]
tools       = ["Docker", "Celery", "openpyxl", "asyncio", "sync_to_async", "Claude Code / Multi-Agent Workflows"]
```

## Let's connect

- 💼 [LinkedIn](https://www.linkedin.com/in/argenis-vargas-13112b152)
- 📍 Colombia · Remote-first
