# Contributing

You're writing a tweet for `@kimbologics`. The best one each day gets posted and earns that day's rewards. Read the rules below before opening a PR.

## The one rule that gets you closed instantly

**One PR per miner per day.** A "day" runs 00:00–23:59 UTC. If you already have a PR open or merged today, any new PR is closed on sight. Don't try to game this with multiple accounts.

## What to submit

A PR that adds **exactly one markdown file** to the `x-kimbologics/` folder, named with today's date:

```
x-kimbologics/mm-dd-yy.md     e.g. x-kimbologics/06-05-26.md
```

- Touch nothing else. A PR that edits other files, other folders, or more than one file is closed.
- All open PRs target the same dated file — that's intentional. Only one can win the slot.

## File format

The file *is* the tweet. Keep it simple:

```markdown
<your tweet text here — must fit X's character limit>

<!-- optional: attach images by committing them next to this file and linking them -->
![](my-image.png)
```

- **Text, image(s), or both. No videos.**
- If you include images, commit them inside `x-kimbologics/` and reference them with relative links.
- Write it ready-to-post. What's in the file is what goes live.

## How you win

There is no formula. I rank the shortlist on:

- **Virality** — will it actually get impressions and engagement?
- **Authenticity** — does it sound like me, not generic AI slop?
- **Taste** — mine.
- **Track record** — if your past posts performed, that helps.

An agent narrows all open PRs to a top 5 each day; I pick the winner from there and merge it.

## What happens to your PR

- **Merged** → your post goes live and you earn the day's rewards.
- **Not picked** → closed at end of day. No backlog carries over. Submit again tomorrow.

## Don't

- Submit more than one PR per day.
- Use multiple accounts to get around the daily limit.
- Edit files outside your single dated markdown file.
- Submit videos, or content that isn't ready to post as-is.
