# Standard project files (templates)

Copy these into a new repo's root and replace every `<…>`. A scaffold script that writes them is a good
first Claude Code project.

## CLAUDE.md
```
# <project>

## Start here (read in this order)
1. This file
2. STATE.md
3. ERRORS_AND_LESSONS.md, then the global lessons file
4. LOG.md, only as far back as the task needs

## What this is
<Two sentences: what it is, what done looks like.>

## Project rules
<Only rules specific to this project.>

## Checkpoint
- Test: `<command>` (must pass before any checkpoint commit) or `none`
- Build: `<command>` or `none`

## Write permissions
<"Whole folder writable without asking" (workshop) or "only the standard files and _OUTPUTS/" (archive).
Never delete; back up before overwriting.>
```

## STATE.md
```
---
updated: <YYYY-MM-DD>
---
# <project> — State
## Where things stand
**Next action:**
## What is open
## What must not be touched
## What has not been verified
```

## LOG.md
```
# <project> — Log
Append-only. Newest at the bottom, as `## YYYY-MM-DD — title`. Never edit an earlier entry; append a correction.
```

## ERRORS_AND_LESSONS.md
```
# <project> — Errors and lessons
One entry per incident: `## YYYY-MM-DD — title that states the lesson`, then Symptom / Cause / Fix / Rule.
```

## SECURITY.md
```
# <project> — Security
## Threat model: what it is, where it runs, data it handles, who can reach it, worst-case misuse
## Identities and secrets: identity | may do | credential + where it lives (never the value) | rotation
## Inputs and outputs: untrusted inputs and where they're validated; how model output is checked
## Dependencies: pinning; SBOM command
## AI features and agents: tool allow-list, sandbox, human-approval gates, caps, where calls are logged
## Defaults and failure modes: must fail closed
## Accepted risks: risk | why | revisit by
```
