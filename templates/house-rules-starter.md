# House rules (starter)

Put this in `~/.claude/CLAUDE.md` to begin. Later, move it into a plugin and leave a pointer. Replace every `<…>`.

## Who I am
<Role, e.g. film/TV composer>. Work splits into <creative/business> and <tools/tech>.

## Machine
- Host: `<name>` · user: `<user>` · <OS>
- Documents/media root: `<cloud folder path>`
- Code root: `~/dev/`

## Operating principles
1. **Route me to the right surface.** Chat = decide, design, research, drafts. Cowork = hand-off multi-step work.
   Claude Code = anything touching files, repos or automation. If I started in the wrong one, say so first.
2. **Front-load, then run.** Ask every question you need at the start, in one batch. Then finish without
   check-ins, except before anything destructive or irreversible.
3. **Automate me out of the loop.** Prefer unattended, idempotent, self-healing solutions. Flag any step I repeat.

## Working rules
- Handoffs: when another surface fits better, say so and give a ready-to-paste blurb that says where to start reading.
- Recurring procedure → suggest making it a skill.
- Keep docs current; reference them instead of re-deriving; flag stale ones.
- Never delete: move to `_to_delete/` with the date and reason. Back up before overwriting (`.bak-YYYYMMDD`).
- One owner per fact: no file restates what another owns.
- Papercuts: one dated line in `~/dev/_vault/Papercuts.md` whenever something costs an extra step.

## Which file to believe
| When these disagree | Believe |
|---|---|
| Any doc vs the files / build / command output | the files, build, output |
| STATE.md vs LOG.md | STATE for now, LOG for history |
| Claude's memory vs project files | project files |

## Two roots
- `<cloud folder>`: documents, media, deliverables (`_INBOX/`, `Workspace/`, `Delivered/`, `Studio/`, `Admin/`, `_ARCHIVE/`).
- `~/dev/`: code, git, private GitHub repos. Never a repo inside the cloud folder.
- Deliverables go to `_INBOX/` or the named project folder, never Desktop or Downloads.

## Naming
Filename carries what the folder doesn't. `_INBOX`: project first. Project folder: document first. Piles: date first.
Lowercase; hyphens inside tokens, underscores between. Never `: / < > | ? *`.

## Project files
Every repo: CLAUDE.md, STATE.md, LOG.md, ERRORS_AND_LESSONS.md, SECURITY.md. "Start here" reads them in order;
"checkpoint this project" updates them, tests, commits and pushes, then bumps the hub row.

## How I work
- Be direct; skip preamble. Push back when I'm wrong. Show tradeoffs for anything with real cost.
- Least effort for me: do it yourself → suggest the missing connector or app → give me one Terminal command.
- When a tool is broken or disconnected, give me the fix before working around it.
- Browser and computer use stay in the background; ask before bringing a window forward.

## Security
- Follow `<your security playbook>`. Secrets only in `<password manager / keychain>`.
- Agents: allow-listed tools, sandboxed, human approval for send/spend/delete/config, caps, logged tool calls.
- Every repo has SECURITY.md; run the review before release. A qualified human reviews code before anything is sold.

## Session discipline
On start: "start here". On end: "checkpoint this project", then bump the hub row.
