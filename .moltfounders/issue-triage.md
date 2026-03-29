# Issue Triage Rules

## When to Run

On every agent loop cycle, scan all open issues.

## Skip Conditions

- Issue already has `agent:reviewed` label → skip entirely
- Issue was opened by an agent → skip
- GitHub-generated issue → skip

## Triage Steps

### 1. Classify the issue type

- **Addition request** — someone wants a new project added
- **Removal request** — entry is stale, wrong, or weak
- **Correction** — fixing description, link, or section placement
- **Question / discussion** — not a concrete change request
- **Spam / off-topic** — unrelated

### 2. Evaluate addition requests

The **primary bar** (from CONTRIBUTING.md): the project must be:
- directly inspired by `karpathy/autoresearch`, OR
- explicitly cites autoresearch as a foundation, OR
- clearly uses the same autonomous improvement loop pattern in a meaningful adjacent domain

**Secondary checks:**
- Is the repo real and accessible?
- Is it not already in the list? (Search README)
- Does it fit an existing section?
- Is it actively maintained or a useful reference?

**Not sufficient alone:**
- "It's an AI research agent" — must have autoresearch lineage
- "It does autonomous improvement" — must connect to the autoresearch loop pattern specifically
- Being adjacent is ok for the Related Resources section, but connection must be obvious

### 3. Comment with clear verdict

- What you checked
- Whether it meets the autoresearch connection bar
- If not, explain specifically what's missing
- If yes, suggest the right section and invite a PR

### 4. Apply labels

- Always apply `agent:reviewed`
- Apply `agent:commented` if you left a comment
- Apply `no-autoresearch-connection`, `duplicate`, or `needs-info` as appropriate
- Apply `needs-human` for borderline cases

## Edge Cases

- **Clearly autoresearch-derived but poorly described issue:** Ask for a PR instead of the issue
- **Borderline connection:** Label `needs-info`, ask submitter to explain the autoresearch link specifically
- **Issue >90 days, no activity:** Follow staleness rules in `staleness.md`
