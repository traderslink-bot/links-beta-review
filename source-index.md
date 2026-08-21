# Source Index

## Reachable implementation checkpoint

- Source repository: [traderslink-bot/traderlink-platform](https://github.com/traderslink-bot/traderlink-platform)
- Source branch: `codex/traderlink-platform-replacement`
- Exact source commit: [`a5ca6b66b656c091e787ab7cbb50faf45867f2d4`](https://github.com/traderslink-bot/traderlink-platform/commit/a5ca6b66b656c091e787ab7cbb50faf45867f2d4)
- Commit: `feat(coach): add typed Links trade performance routing`

This replaces the earlier local-only draft reference. The commit above is now
reachable and is the first implementation checkpoint for external source review.

## Exact changed paths

- `docs/migration/links-beta-performance-language-engine-plan.md`
- `docs/migration/links-beta-performance-language-engine-progress.md`
- `docs/migration/ai-chat-plan.md`
- `docs/migration/ai-chat-progress.md`
- `src/modules/coach/server/coach-ai-chat-question-time-scope.ts`
- `src/modules/coach/server/coach-ai-chat-completed-trade-performance-language.ts`
- `src/modules/coach/server/coach-ai-chat-completed-trade-performance-language-fixtures.ts`
- `src/modules/coach/server/coach-ai-chat-completed-trade-performance-evaluator.ts`
- `src/modules/coach/server/coach-ai-chat-deterministic-fast-path.ts`
- `src/modules/coach/server/coach-ai-chat-generation-service.ts`
- `src/modules/coach/server/coach-ai-chat-generation-runtime.ts`

## What this checkpoint implements

- Typed deterministic plans for selected-account completed-trade P/L, trade
  count, win/loss count, best/worst trade, top/bottom trades, outcome filters,
  and calendar scopes.
- A plan context that records selected account scope, reporting currency,
  selected-account timezone, and one fixed request reference time.
- Deterministic execution through existing `summarize_closed_trades` and
  `query_trade_explorer` Journal handlers, with code-rendered factual answers
  and evidence references.
- Static independent evaluation fixtures: 30 resolved plans and five boundary
  cases. Evaluation reports plan components rather than only pass/fail.
- Explicit collision protection: trading-day and ticker questions are not
  misrouted as all-trade P/L; deferred metrics and invalid rank counts remain
  component failures.

## Deliberately not in this checkpoint

No ticker/day/session aggregate implementation, comparison, behavior/rule
analysis, Luna fallback, readiness UI, migration, new data source, UI change,
provider call, live chat run, or server process.

Focused ESLint, TypeScript, and whitespace checks passed for the changed source.
