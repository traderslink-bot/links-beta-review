# Architecture Checkpoint — 2026-08-21

## Status

Draft architecture published for owner and external review. No router rebuild, provider call, database migration, UI build, deployment, or beta capability claim belongs to this checkpoint.

## Approved direction under review

Links AI Chat's first beta purpose is helping a trader understand their own completed-trade performance and patterns from exact Journal data.

The planned engine resolves user language into a validated typed request plan before reading Journal data. It exposes component-level evaluation instead of a generic pass/fail result, and later provides an owner-visible readiness dashboard.

## Immediate next decision

Approve or revise the architecture plan before implementation begins.

## First implementation target after approval

Completed-trade performance language: P/L, gain/loss outcome, trade count, best/worst and top/bottom completed trades, and calendar date scope. The target is a validated request plan and component-level result for every case, not a collection of literal phrase checks.
