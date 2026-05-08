# Oracle Logs

Daily I Ching oracle draws from [oracle.truesight.me](https://oracle.truesight.me).

Each draw is persisted as a Markdown file in `draws/YYYY-MM-DD.md` with:
- Hexagram details (primary, related, changing lines)
- AI-generated advisory (issues surfaced, suggested work, risks)
- Structured sections parseable by LLMs for automated triage

## Usage by AI agents
- `autopilot`: use `read_oracle_logs` tool to fetch the latest draw
- `opencode`: point at `draws/` for context on pipeline health

## Draw format
```markdown
# Oracle Draw — YYYY-MM-DD
## Hexagram
- Primary: #N Name
- Related: #N Name
- Changing lines: N

## Advisory
(AI-generated text)

## Issues surfaced
- [pipeline] ...
- [ledger] ...

## Suggested actions
- [auto] ...
- [review] ...
- [online] ...
```
