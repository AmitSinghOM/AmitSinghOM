# Amit Singh

**Senior Backend & Platform Engineer** · Pune, India
Python · AWS · Event-Driven Systems · Production Reliability · Applied AI

I build systems that stay correct under pressure. 7+ years across product safety, network
operations and financial data; currently an SDE II with Realtek Software Services delivering
multi-tenant product-safety platforms for Amazon Ring and Lab126.

## Selected work

Every number below is re-verified by running the suite before it is published.

- **[fastapi-microservices-platform](https://github.com/AmitSinghOM/fastapi-microservices-platform)** —
  Self-hosted webhook delivery on PostgreSQL alone (no Redis/Kafka): lease-fenced durable queuing,
  per-endpoint event-type subscriptions, Standard Webhooks-compliant signatures cross-verified by the
  official ecosystem library, SSRF-isolated egress and audited dead-letter replay. Evidence-gated
  releases: a reproducible 1M-delivery zero-loss run and a
  [benchmarks page](https://github.com/AmitSinghOM/fastapi-microservices-platform/blob/main/docs/benchmarks.md)
  that reports the target it missed. 187 tests.
- **[code-quality-analyzer](https://github.com/AmitSinghOM/code-quality-analyzer)** —
  Privacy-first static analysis for Python plus bounded Go, TypeScript/JavaScript, Java, Kotlin,
  C#/.NET and C/C++ pilots, on PyPI as
  [`cqa-analyzer`](https://pypi.org/project/cqa-analyzer/) via Trusted Publishing with digital
  attestations and no long-lived release credentials. One shared 56-pattern architecture catalog
  (DSA, GoF, production-systems) under a versioned scoring policy, enforced-offline execution,
  cross-file AST duplication detection, SARIF/baseline CI gates. 400 tests on a 3-OS × 4-Python matrix.
- **[cloudscale-backend](https://github.com/AmitSinghOM/cloudscale-backend)** —
  CQRS + event sourcing with a typed hexagonal core: exactly-once-effect projections via
  transactional dedupe, retry / circuit-breaker / dead-letter resilience, SQLite and PostgreSQL
  adapters behind shared ports, and an authenticated HTTP tier that sustained 1,431 rps in a
  scripted gate run. 204 tests including 9 Hypothesis property suites.
- **[agent-skills](https://github.com/AmitSinghOM/agent-skills)** —
  Three tested Agent Skills for coding agents (Claude Code, Kiro, Codex, Cursor), each backed
  by a runnable tool or a behaviour contract. `code-quality-gate` turns `cqa-analyzer` into a
  CI gate that fails only on new findings on changed lines, with a stdlib git-diff-to-manifest
  generator and config pinning so a PR cannot weaken the gate. Spec-validated against
  agentskills.io; 30 tests; CI on Python 3.10–3.13 plus a live analyzer smoke job.

## How I work

- Make trust boundaries explicit, failures observable, and behaviour difficult to bypass.
- Report the target that was missed rather than hide it; record rejected designs, not just chosen ones.
- Trace problems to the correct ownership layer and carry the fix through rollout and support.

## Elsewhere

[Portfolio](https://amitsinghom.github.io/) · [Résumé](https://amitsinghom.github.io/resume.html) ·
[LinkedIn](https://linkedin.com/in/amit-singh-491100192) · amitdsingh710@gmail.com
