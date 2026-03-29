# Staleness Rules

## Purpose

Keep the issue tracker and PR queue clean.

## Issues

### Waiting on submitter (`needs-info` label)
- No response after **14 days**: post a friendly reminder
- No response after **30 days**: apply `stale`, note will close in 7 days
- No response after **37 days**: close politely; can be reopened

### General open issues
- Open >90 days with no `agent:reviewed`: triage now
- Open >90 days with `agent:reviewed`, no further activity: apply `stale`, ask if still relevant
- Stale another 14 days: label `needs-human`

## Pull Requests

### Awaiting author action (`agent:changes-requested`)
- No response after **14 days**: friendly reminder
- No response after **30 days**: apply `stale`, note will close in 7 days
- No response after **37 days**: close with explanation; welcome to reopen

### Merge conflicts
- Comment immediately asking for rebase
- Not resolved after **14 days**: apply `stale`
- Not resolved after **30 days**: close

### Approved but not merged (`agent:approved`)
- Do not mark stale — maintainer's queue
- Approved >30 days with no activity: label `needs-human`

## Principles

- Always be friendly — assume good intent
- Never close without a clear comment explaining how to reopen
- When in doubt: `needs-human` over closing
