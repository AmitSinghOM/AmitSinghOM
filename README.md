# Amit Singh

**Senior Backend & Platform Engineer** · Pune, India
Python · AWS · Event-Driven Systems · Production Reliability · Applied AI

I build systems that stay correct under pressure. 7+ years across product safety, network
operations and financial data; currently an SDE II with Amazon delivering
multi-tenant product-safety platforms for Ring and Lab126/Leo.

## Selected work

Every number below comes from a pinned public CI run or a documented benchmark of the linked
repository and is re-checked before it is published (last check: 2026-10-16).

- **[fastapi-microservices-platform](https://github.com/AmitSinghOM/fastapi-microservices-platform)** —
  Self-hosted webhook delivery on PostgreSQL alone (no Redis/Kafka): lease-fenced durable queuing,
  per-endpoint event-type subscriptions, Standard Webhooks-compliant signatures cross-verified by the
  official ecosystem library, SSRF-isolated egress and audited dead-letter replay. Evidence-gated
  releases: a reproducible 1M-delivery zero-loss run and a
  [benchmarks page](https://github.com/AmitSinghOM/fastapi-microservices-platform/blob/main/docs/benchmarks.md)
  that reports the target it missed. 220 tests (188 service, 32 Python SDK).
- **[code-quality-analyzer](https://github.com/AmitSinghOM/code-quality-analyzer)** —
  Privacy-first, offline static analysis for eight languages (Python in depth; bounded Go,
  TypeScript/JavaScript, Java, Kotlin, C#/.NET, C/C++ and Rust), on PyPI as
  [`cqa-analyzer`](https://pypi.org/project/cqa-analyzer/) via Trusted Publishing with digital
  attestations and no long-lived release credentials. 95 rules including a 27-rule CWE-anchored
  security family with SARIF security severity; one shared 62-pattern architecture catalog (DSA,
  GoF, production-systems) under a versioned scoring policy; cross-file AST duplication detection;
  changed-line CI gates with line-shift-stable baseline fingerprints; a
  [GitHub Action](https://github.com/AmitSinghOM/cqa-action) and a stdlib MCP server.
  969 tests on the deep-enabled suite; CI on Python 3.11–3.14 and on Linux, macOS and Windows.
- **[cloudscale-backend](https://github.com/AmitSinghOM/cloudscale-backend)** —
  CQRS + event-sourcing ledger with a typed hexagonal core: idempotent commands, a transactional
  outbox, double-entry transfers, holds and reverts with property-tested money conservation,
  OIDC/JWKS identity with default-deny authorization, SQLite and PostgreSQL adapters behind shared
  ports, an enforced backup/restore drill, and an authenticated HTTP tier that sustained 1,431 rps
  in a scripted gate run. 518 tests including 9 Hypothesis property suites, on Python 3.12 and 3.13.
- **[agent-skills](https://github.com/AmitSinghOM/agent-skills)** —
  Four tested Agent Skills for coding agents (Claude Code, Kiro, Codex, Cursor), each backed
  by a runnable tool or a behaviour contract. `architecture-baseline` snapshots a codebase's
  observed architecture from `cqa-analyzer`'s pattern map and fails CI when a pattern leaks
  into a layer it never lived in; `code-quality-gate` turns the same analyzer into a
  changed-line gate with config pinning so a PR cannot weaken it. Spec-validated against
  agentskills.io; 41 tests; CI on Python 3.10–3.13 plus a live analyzer smoke job.

## How I work

- Make trust boundaries explicit, failures observable, and behaviour difficult to bypass.
- Report the target that was missed rather than hide it; record rejected designs, not just chosen ones.
- Trace problems to the correct ownership layer and carry the fix through rollout and support.

## Elsewhere

[Portfolio](https://amitsinghom.github.io/) · [Résumé](https://amitsinghom.github.io/resume.html) ·
[LinkedIn](https://linkedin.com/in/amit-singh-491100192) · amitdsingh710@gmail.com
