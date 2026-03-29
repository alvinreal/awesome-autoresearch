# PR Review Rules

## When to Run

On every agent loop cycle, scan all open PRs.

## Skip Conditions

- PR already has `agent:reviewed` → skip entirely
- PR is a draft → skip
- PR was opened by an agent → skip
- Bot PR → label `needs-human`, skip
- **PR has merge conflicts** (`mergeable = false`) → comment asking author to rebase, apply `needs-info` label, do NOT approve, skip remaining review steps entirely

## Review Steps

### 1. Understand what the PR adds

Read the PR title, description, and diff.

### 2. Autoresearch connection check (primary bar)

This is the most important check. The project must satisfy at least one:
- **Explicit lineage:** Directly forked from or explicitly builds on `karpathy/autoresearch`
- **Explicit citation:** README or docs cite autoresearch as inspiration/foundation
- **Same loop pattern:** Uses the autonomous keep-or-revert improvement loop in a meaningful way (not just "it does AI")

If the connection is absent or tenuous → request changes with `no-autoresearch-connection`. Ask the submitter to clarify.

### 3. Format checks (from CONTRIBUTING.md)

Preferred entry format:
```
- [owner/repo](url) - Short, neutral description.
```
Stars badge is optional but accepted. Check:
- Is the description short, factual, non-promotional?
- Is the link valid?
- Is it in the correct section?
- No marketing copy or keyword stuffing?

### 4. Content checks

- **Duplicate:** Search README for the repo URL and name
- **Section fit:** Does it belong where it was placed? Sections:
  - General-purpose descendants
  - Research-agent systems
  - Platform ports and hardware forks
  - Domain-specific adaptations
  - Evaluation & benchmarks
  - Notable use cases and writeups
  - Related resources
- **Quality:** Is it a real, functional project? Not a stub or empty repo?

### 5. Leave your review

Be specific:
- State clearly whether it passes the autoresearch connection bar
- Note any format issues
- If approving: confirm the connection explicitly
- If requesting changes: give actionable, friendly guidance

### 6. Apply labels and set status

- Always apply `agent:reviewed`
- Apply `agent:approved` if it passes all checks
- Apply `agent:changes-requested` if issues found
- Apply `no-autoresearch-connection`, `wrong-section`, `duplicate` as needed
- Apply `needs-human` for genuinely borderline cases

## Important: Agent approval ≠ merge

Only the maintainer merges.

## Edge Cases

- **PR adds to Related Resources section:** Lower bar — "adjacent but related" is fine here, still needs obvious connection to the space
- **PR fixes a broken link or formatting only:** Fast-track approve
- **Stars badge missing from entry:** Not a blocker — format is flexible per CONTRIBUTING.md
- **PR has been open >30 days with no author response:** Follow staleness rules
- **Submitter disputes the autoresearch connection:** Label `needs-human` — this is a judgment call for the maintainer
