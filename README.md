# social-media-manager

This is an experimental repository on [gittensor](https://github.com/entrius/gittensor). Miners submit PRs containing a social media post; the best one each day gets posted to my account and earns emissions.

## Goal

I want to improve my presence on X (`@kimbologics`). As a subnet owner, being known within the Bittensor ecosystem is important, and right now my presence is virtually zero. With that in mind, this repo's premise is simple: miners submit tweets, I post the best one daily. In theory, consistency along with occasionally banger tweets should bring more impressions overall.

## How it works

1. **Miners submit PRs.** Each PR is one candidate post — text, image(s), or both. No videos. Follow the PR template.
2. **One PR per miner per day.** Any additional PR from the same miner is closed. The day resets at midnight US Central Time (`America/Chicago`).
3. **The agent culls to a shortlist.** Once a day (around 4:30pm Central) an agentic maintainer reads every open PR and narrows them to the top 5 for me to review.
4. **I pick the winner.** I merge exactly one PR. That post goes live on my X account.
5. **The winner earns the day.** I adjusted the repositories hyperparameters such that only the latest person with a `crown` labeled merged PR earns rewards.
6. **Clean slate.** All remaining open PRs are closed at end of day — no backlog. It repeats tomorrow.

## How winners are chosen

I rank the day's finalists on virality, fit, and personal taste, and weigh each miner's track record (if any). See [CONTRIBUTING.md](CONTRIBUTING.md#how-your-pr-gets-merged).

## Eligibility

This repository has its hyperparameters configured such that only PRs with the `crown` label get rewarded. My maintainer agent will always set the winning PR with that label and remove all other PRs with `crown` label. Which causes this repo to be 'winner take all' until I run the agentic pipeline again.

## Repo structure

```
README.md
CONTRIBUTING.md
x-kimbologics/                   # <platform>-<username>; scales to other accounts/platforms later
  06-09-26-oktofeesh1.md         # merged post, named mm-dd-yy-<github-username>.md
  06-10-26-pixelbob.md
  ...
```

Every PR adds one markdown file to `x-kimbologics/` named with today's date and the author's GitHub username — `mm-dd-yy-<username>.md`. Each miner gets their own file, so submissions never collide and the winner is chosen on merit, not a filename race.

See [CONTRIBUTING.md](CONTRIBUTING.md) for the exact PR format and rules.
