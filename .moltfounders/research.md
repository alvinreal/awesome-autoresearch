# Research Loop Rules

## Purpose

Periodically discover new autoresearch-related projects worth adding and add them directly via a single PR.

## Frequency

Run once per week. Do not run if you already opened a research PR in the last 7 days (check open PRs with title starting with `[Research]`).

## Sources to Check

1. **GitHub search** — `karpathy autoresearch fork`, `autoresearch loop`, `keep-or-revert` in repo descriptions/READMEs
2. **GitHub network** — forks of `karpathy/autoresearch` sorted by recently updated
3. **Papers with Code / arXiv** — new papers citing autoresearch or describing autonomous improvement loops
4. **Twitter/X** — search `autoresearch karpathy`, `autoresearch loop` for recent demos
5. **Hacker News** — search for autoresearch mentions in Show HN or recent posts

## Qualification Criteria

A project qualifies if:
- Clear autoresearch connection (lineage, citation, or same keep-or-revert loop pattern)
- Real functional repo (not a stub)
- Not already in the list (search README before adding)
- Fits an existing section

## How to Add — Single PR

**Do not open issues.** Instead, open **one PR** adding all qualified entries directly to README.md:

1. Clone/pull the repo locally
2. Collect all qualifying candidates (max 5 per cycle)
3. Add each to the correct section in README.md following the existing format:
   ```
   - [owner/repo](url) ![GitHub stars](badge) - Short neutral description.
   ```
4. Open a single PR titled `[Research] Add N new entries — <date>`
5. PR body lists each addition with: name, link, autoresearch connection, suggested section

One PR per research cycle. Do not open individual issues or individual PRs per entry.

## Limits

- Max **5 entries per PR**
- If a `[Research]` PR is already open and unmerged, do not open another
- Do not add projects already in an open unmerged PR

## Edge Cases

- **Very new fork (<1 week):** Still add if clearly autoresearch-derived, note recency in PR body
- **Writeup/blog post (no repo):** Can add to Notable Use Cases section
- **No qualifying projects found:** Do nothing — do not open an empty PR
