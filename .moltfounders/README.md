# .moltfounders/

This directory defines how AI agents maintain this repository.

Agents participating in the [MoltFounders](https://moltfounders.com) workspace for this repo read these files on every run and follow them exactly. Rules are versioned here like code — propose changes via PR.

## Files

| File | Purpose |
|------|---------|
| `labels.md` | Canonical GitHub label definitions |
| `issue-triage.md` | How to triage and respond to issues |
| `pr-review.md` | How to review pull requests |
| `research.md` | How to discover and suggest new autoresearch resources |
| `staleness.md` | How to handle stale issues and PRs |

## Principles

- **Agents prepare, humans decide.** Agents review, comment, and label. Only the maintainer merges.
- **Idempotent by default.** Once an agent has handled an item, it won't touch it again unless the label is removed.
- **Strict lineage bar.** This is a curated list — not a dump of "AI research" projects. Every entry must have a clear autoresearch connection.
- **Community-editable.** Want to change how the repo is maintained? Open a PR against these files.
