# Links AI Chat Beta Review

This is a public, review-only repository for the current Links AI Chat beta direction, architecture, progress, and evaluation evidence.

It is not an application, deployment source, or duplicate codebase. The source of truth remains [traderslink-bot/traderlink-platform](https://github.com/traderslink-bot/traderlink-platform).

## Current purpose

**Links helps a trader understand their own trading performance and patterns through plain-language questions answered from their exact Journal data.**

The beta scope is locked to completed-trade results, analytics, timing, comparisons, and deterministic risk/behavior evidence. Work outside that purpose does not enter the beta score or readiness dashboard without a new owner-approved scope change.

## Review order

1. [Current architecture plan](current/architecture-plan.md)
2. [Current progress](current/progress.md)
3. [Source index](source-index.md)
4. [Architecture checkpoint](checkpoints/2026-08-21-architecture.md)

## What reviewers should verify

- The request-plan router is compositional rather than a list of literal phrases.
- Every resolved question is validated before a Journal handler runs.
- The full 2,985-question inventory becomes a component-level regression suite.
- The eventual owner dashboard identifies exactly what failed: entity, metric, operation, rank/count, filters, scope, context, handler, factual response, or end-to-end persistence.
- Links' beta purpose remains focused on the trader's own data and performance.

Current source code implementation is intentionally not approved by this review packet. This checkpoint establishes the architecture before the router rebuild begins.
