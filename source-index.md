# Source Index

## Source of truth

- Repository: [traderslink-bot/traderlink-platform](https://github.com/traderslink-bot/traderlink-platform)
- Source branch at review-packet creation: `codex/traderlink-platform-replacement`
- Review-source state: the Links architecture documents are a local working-tree draft under owner review. They are not yet a committed implementation checkpoint.

The earlier reference to `43baf12dbd7bdf2af466e31acc98231886ea1f5e` was a local source checkout reference and is not reachable from the public source repository. It is therefore **not** an immutable source pin for this review packet. This packet makes no false published-commit claim. Each later implementation checkpoint will instead link its exact reachable source commit and changed paths.

## Current review material

The current design is mirrored here for easy review:

- [Architecture plan](current/architecture-plan.md)
- [Progress record](current/progress.md)

The corresponding local source paths are:

- `docs/migration/links-beta-performance-language-engine-plan.md`
- `docs/migration/links-beta-performance-language-engine-progress.md`
- `docs/migration/ai-chat-plan.md`
- `docs/migration/ai-chat-progress.md`

The review copies are purpose-built review material. Their local source documents are still drafts pending owner approval and a later narrow source commit.

## Existing assets to inspect when implementation begins

- `src/modules/coach/server/coach-ai-chat-question-bank.ts`
- `src/modules/coach/server/coach-ai-chat-deterministic-fast-path.ts`
- `src/modules/coach/server/coach-ai-chat-language-inventory.generated.ts`
- `src/modules/coach/contracts/coach-ai-chat-factual-tool-contracts.ts`
- `src/modules/coach/server/coach-ai-chat-factual-tool-registry.ts`
