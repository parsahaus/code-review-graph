<!-- agent-sync:begin -->

# code-review-graph

`./CLAUDE.md` is the complete and authoritative instruction file for this
project. **Read it in full before doing anything here.** Every rule in it
applies to you exactly as written, whichever agent you are.

### Non-negotiable rules for this project

Repeated here because breaking one of them cannot be undone. This list is a
floor, not a summary. It does not replace reading CLAUDE.md.

- SQL always uses parameterized queries with `?` placeholders. Never interpolate a value into the query string.
- API keys come from environment variables only, never hardcoded.

### Applies everywhere on this machine

- Never hardcode a secret, token, API key or password. Environment variables or the project's own secret store only, and never echo a credential back once you have read one.
- On this machine, never use `npx`, `cmd`, `bunx`, `pnpm dlx` or a `*.cmd` file as a hook or MCP server command. Always `node "<absolute path>"`, and every child_process spawn inside a hook passes `windowsHide: true`. The reason is that those entry points flash a console window that steals focus from fullscreen apps.
- Commit and push only when the owner asks for it. Never push to a default branch on your own initiative.

<!-- agent-sync v3 | shape=owned | claude_sha256=d80072b0aec70bb6e7b1cda4f389f598d53c8fb3aae6342fe34b06f62324087b | content_sha256=d24febf6eae3e5da4321045a1789907e0fafc0361a9e98bec2ef224957a712df | generated=2026-09-09T03:51:37Z -->
<!-- Generated. Do not edit inside the agent-sync markers; edit
     ~/.agent-sync/projects.json and re-run sync_agents.py. -->
<!-- agent-sync:end -->
