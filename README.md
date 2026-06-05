# social-media-manager

An experimental repository on [gittensor](https://github.com/gittensor). Miners compete to write my social media posts; the best one each day gets posted to my real account and earns the day's rewards.

## Goal

I want to improve my presence on X (`@kimbologics`). As a subnet owner, being known within the Bittensor ecosystem matters, and right now my presence is near zero. This repo turns that into an incentivized game: miners submit tweets, I post the best one daily.

## How it works

1. **Miners submit PRs.** Each PR is one candidate post — text, image(s), or both. No videos.
2. **One PR per miner per day.** Any additional PR from the same miner is closed. The day resets at 00:00 UTC.
3. **The agent culls to a shortlist.** Once a day an agentic maintainer reads every open PR and narrows them to the top 5 for me to review.
4. **I pick the winner.** I merge exactly one PR. That post goes live on my X account.
5. **The winner earns the day.** Because only merged PRs score, the merged author is the only miner rewarded that day.
6. **Clean slate.** All remaining open PRs are closed at end of day — no backlog. It repeats tomorrow.

## How winners are chosen

There is no scoring equation. I rank on:

- **Virality** — perceived likelihood to get impressions and engagement.
- **Authenticity** — does it sound like *me*, not generic AI filler.
- **Personal taste.**

I also weigh **track record**: if a miner's previous post performed well, that factors into the agent's shortlist and my merge decision.

## Eligibility

Rules are intentionally lax — **any PR that gets merged is rewarded.** There is no credibility gate or minimum history to participate.

## Repo structure

```
README.md
CONTRIBUTING.md
x-kimbologics/          # <platform>-<username>; scales to other accounts/platforms later
  06-05-26.md           # one merged post per day, named mm-dd-yy.md
  06-06-26.md
  ...
```

Every PR adds a single markdown file to `x-kimbologics/` named with today's date as `mm-dd-yy.md`. Since all PRs target the same dated file, only one can win the slot each day.

See [CONTRIBUTING.md](CONTRIBUTING.md) for the exact PR format and rules.
