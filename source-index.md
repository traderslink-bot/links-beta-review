# Source Index

## Reachable remediation checkpoint

- Source repository: [traderslink-bot/traderlink-platform](https://github.com/traderslink-bot/traderlink-platform)
- Source branch: `codex/traderlink-platform-replacement`
- Exact source commit: [`e287e5a7a281cc6bfd449faffcf6263155e02a93`](https://github.com/traderslink-bot/traderlink-platform/commit/e287e5a7a281cc6bfd449faffcf6263155e02a93)
- Commit: `fix(coach): prove completed trade language coverage`

This is the reachable remediation checkpoint requested after the initial source
foundation at `a5ca6b66`. It does not start a new capability family.

## Exact changed paths

- `docs/migration/links-beta-performance-language-engine-plan.md`
- `docs/migration/links-beta-performance-language-engine-progress.md`
- `src/modules/coach/server/coach-ai-chat-completed-trade-performance-evaluator.ts`
- `src/modules/coach/server/coach-ai-chat-completed-trade-performance-language-fixtures.ts`
- `src/modules/coach/server/coach-ai-chat-completed-trade-performance-language.ts`
- `src/modules/coach/server/coach-ai-chat-completed-trade-performance-master-evaluator.ts`
- `src/modules/coach/server/coach-ai-chat-question-bank.ts`
- `src/modules/coach/server/coach-ai-chat-question-time-scope-fixtures.ts`
- `src/modules/coach/server/coach-ai-chat-question-time-scope.ts`
- `src/scripts/evaluate-links-completed-trade-performance-master.ts`

## Executed local result

The purpose-built evaluator is source-only: it invokes no provider, Links AI
Chat, database, or factual handler.

| Measure | Result |
| --- | --- |
| Master inventory classified | 2,985 / 2,985 |
| First-slice applicable cases | 193 |
| Resolved correctly | 193 / 193 |
| Wrong-plan cases | 0 |
| Silently dropped modifiers | 0 |
| Deferred / unsupported / ambiguous | 2,792 / 0 / 0 |
| Collision and boundary suite | PASS (5 cases) |
| Date-edge suite | PASS (12 cases) |
| Component evaluator | PASS (32 resolved fixtures) |
| Provider calls | 0 |

## What the remediation proves

- Long/short is retained as a direction filter in the typed plan and canonical
  Trade Explorer request.
- Every master-bank row is explicitly classified for the current first-slice
  boundary; deferred rows are not counted as working coverage.
- Applicable plans are compared component by component, including account,
  currency, timezone, reference time, entity, metric, operation, rank, filters,
  date scope, handler, and handler request.
- Calendar month shifting handles month-end, leap-year, year-boundary, and
  account-timezone boundaries.
- Unqualified `how much did I make/lose` has an explicit net realized P/L
  meaning. Explicit gross requests remain outside this first slice.

## Deliberately not in this checkpoint

No ticker/day/session aggregate implementation, comparison, behavior/rule
analysis, Luna fallback, readiness UI, migration, new data source, UI change,
provider call, live chat run, or server process.

Focused ESLint, TypeScript, whitespace, and the complete zero-provider
evaluation passed for the changed source.
