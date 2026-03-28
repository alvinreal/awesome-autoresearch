# Research Loop Rules

## Purpose

Periodically discover new autoresearch-related projects worth adding and open issues suggesting them.

## Frequency

Run once per week. Do not run if you already opened a research issue in the last 7 days (check `agent:suggested` label).

## Sources to Check

1. **GitHub search** — `karpathy autoresearch fork`, `autoresearch loop`, `keep-or-revert` in repo descriptions/READMEs
2. **GitHub network** — forks of `karpathy/autoresearch` sorted by recently updated
3. **Papers with Code / arXiv** — new papers citing autoresearch or describing autonomous improvement loops
4. **Twitter/X** — search `autoresearch karpathy`, `autoresearch loop` for recent demos
5. **Hacker News** — search for autoresearch mentions in Show HN or recent posts

## Qualification Criteria

A project qualifies if:
- Clear autoresearch connection (lineage, citation, or same loop pattern)
- Real functional repo (not a stub)
- Not already in the list (search README before suggesting)
- Fits an existing section

## How to Suggest

Open a GitHub issue with:
- **Title:** `[Research] Add: <owner/repo>`
- **Body:**
  - Repo URL
  - One-sentence description
  - Autoresearch connection (explicit — what makes this autoresearch-lineage?)
  - Suggested section
  - Source where you found it

Apply label `agent:suggested`.

## Limits

- At most **3 research issues per cycle**
- Check existing `agent:suggested` issues to avoid duplicates

## Edge Cases

- **Very new fork (<1 week):** Still suggest if clearly autoresearch-derived
- **Writeup/blog post (no repo):** Suggest for Notable Use Cases section if it documents a real autoresearch-style run
- **Paper with open implementation:** Suggest if the paper explicitly relates to the autoresearch loop pattern
