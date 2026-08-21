# Source Index

## Source of truth

- Repository: [traderslink-bot/traderlink-platform](https://github.com/traderslink-bot/traderlink-platform)
- Source branch at review-packet creation: `codex/traderlink-platform-replacement`
- Source commit at review-packet creation: `43baf12dbd7bdf2af466e31acc98231886ea1f5e`

## Current review material

The current design is mirrored here for easy review:

- [Architecture plan](current/architecture-plan.md)
- [Progress record](current/progress.md)

The corresponding source paths are:

- `docs/migration/links-beta-performance-language-engine-plan.md`
- `docs/migration/links-beta-performance-language-engine-progress.md`
- `docs/migration/ai-chat-plan.md`
- `docs/migration/ai-chat-progress.md`

At this initial checkpoint, the new architecture documents are a local design draft pending owner review and a later narrow source commit. This review repository deliberately preserves the exact draft reviewed by the owner and external reviewers.

## Existing assets to inspect when implementation begins

- `src/modules/coach/server/coach-ai-chat-question-bank.ts`
- `src/modules/coach/server/coach-ai-chat-deterministic-fast-path.ts`
- `src/modules/coach/server/coach-ai-chat-language-inventory.generated.ts`
- `src/modules/coach/contracts/coach-ai-chat-factual-tool-contracts.ts`
- `src/modules/coach/server/coach-ai-chat-factual-tool-registry.ts`

The review repository will link each later implementation checkpoint to its exact source commit and changed paths.
