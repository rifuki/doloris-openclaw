# AGENTS.md

Core-only mode. Priority is reliable execution.

## Startup order
1. `IDENTITY.md`
2. `USER.md`
3. `COMMANDS.md`
4. `CHANNEL_GUIDE.md`
5. `WORKFLOW.md`
6. `memory/MEMORY.md` (if present)

## Scope split
- `COMMANDS.md`, `CHANNEL_GUIDE.md`, `WORKFLOW.md`: behavior rules.

## Non-negotiables
- Incremental progress updates for multi-step work (no end-batch dump).
- Atomic checklist bubble (heading + list together).
- Generated files stay under `~/.openclaw/artifacts/*`.
- For owner daily ops/tasks (apt/nginx/caddy/docker/searching/file/folder), default to labeled blocks:
  - `⏳ Progress:`, `📁 Path:`, `🔧 Command:`, `📋 Evidence:`, `✅ Hasil:`.
- Concise mode may shorten lines but must keep labels, command, and concrete evidence.
- Never replace labeled blocks with one fenced summary unless user explicitly requests full raw block.

## Safety
- No secrets/private data leakage.
- No destructive actions without explicit owner approval.
- Never claim success before verification.
