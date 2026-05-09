# Argenis Vargas — Principal Engineer

Backend engineer specializing in distributed systems, event-driven architecture and GraphQL federation. I design and build infrastructure that handles real production load — not just on paper.

Currently leading technical strategy and architecture for a high-traffic B2B platform serving organizations of 20,000+ users.

---

## What I actually do

- Design **event-driven pipelines** using GCP Pub/Sub and AWS SNS→SQS fan-out patterns
- Build **GraphQL federation** layers with Strawberry + Apollo Federation
- Optimize **Django ORM** at scale — eliminating N+1 patterns, replacing model instances with lightweight entities, using server-side cursors for high-volume queries
- Design **state machines** for distributed async processes with idempotency guarantees
- Apply **Flyweight and Copy-on-Write** patterns for multi-tenant data architecture
- Build **streaming Excel reports** for datasets of 80K+ rows without OOM — `write_only=True`, `iterator()`, sequential memory phases with explicit release
- Refactor **O(N×6) query loops** into O(1) bulk operations
- Design **composite indexes** aligned to actual query patterns
- Mentor engineers from Mid to Senior level

---

## Core stack

```python
languages  = ["Python 3.12"]
frameworks = ["Django", "FastAPI", "Strawberry GraphQL"]
databases  = ["PostgreSQL", "Redis"]
cloud      = ["AWS (S3, SQS, SNS)", "GCP (Pub/Sub, Scheduler)"]
patterns   = ["Event-driven", "Distributed systems", "GraphQL Federation",
              "SOLID", "Flyweight", "State Machine", "Bulk operations"]
testing    = ["pytest", "TDD", "Integration testing"]
tools      = ["Docker", "Celery", "openpyxl", "asyncio", "sync_to_async"]
```

---

## Engineering principles I live by

**1. El loop es una señal de alarma.**
Si hay un `for` con queries adentro, hay un problema de escala esperando para explotar.

**2. Pensar en conjuntos, no en individuos.**
La diferencia entre O(N) y O(1) casi siempre está en reformular la pregunta, no en optimizar el código.

**3. Los bugs de lógica son más peligrosos que los bugs de performance.**
Un proceso lento molesta. Un proceso que corrompe datos silenciosamente destruye confianza.

**4. El event loop no perdona el ORM síncrono.**
`sync_to_async` no es opcional cuando mezclas Django con async. Es arquitectura.

**5. Liberar memoria explícitamente en procesos de larga duración no es micro-optimización.**
En un pod con límite de RAM, el GC no es suficientemente predecible.

---

## Currently exploring

- Go — for latency-critical services
- Advanced observability — distributed tracing, structured logging at scale
- Platform engineering patterns

## Let's connect

- 💼 [LinkedIn](https://www.linkedin.com/in/argenis-vargas-13112b152)
- 📍 Colombia · Remote-first
