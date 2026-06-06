# Contributing

You're writing a tweet for `@kimbologics`. The best one each day gets posted and earns that day's rewards. Read the rules below before opening a PR.

## Rules that get you closed instantly

**One PR per miner per day.** A "day" runs midnight to midnight **US Central Time** (`America/Chicago`). A second PR while you already have one open or merged today will be closed.

**No edits after opening.** Once your PR is open, any change — to the description _or_ the files — is liable to be closed. Get it right before you open; you don't get to revise.

## Prohibited — closed and banned

Slurs, hate speech, illegal content, doxxing, and toxic or harassing behavior are not allowed. A PR containing any of it is closed immediately and the author is **banned from the repo** — this removes you entirely.

## What to submit

A PR that adds, under `x-kimbologics/`, and **nothing else**:

- **exactly one** markdown file named with today's date — `x-kimbologics/mm-dd-yy.md` (e.g. `x-kimbologics/06-05-26.md`)
- optionally **up to 4 images** — `.png`, `.jpg`, or `.jpeg` only

No other files, folders, or edits. Any other file type, a 5th image, or touching anything else closes the PR. All open PRs target the same dated file — only one can win the slot.

## File format

The `.md` file **is** the tweet — write it exactly as it should appear on X.

- **Format your post.** Write it with the structure it should have live — line breaks, lists, emoji. You can use markdown **bold** and _italics_; those get rendered to X-styled text when posted. Write it to read exactly as you want it to appear.
- **500 character limit** on the tweet text (everything above the `===IMAGES===` line). Over the limit is closed.
- **Images** (optional): commit up to 4 `.png`/`.jpg`/`.jpeg` files in `x-kimbologics/`. To attach them, end the tweet with a line that is exactly `===IMAGES===`, then list each filename on its own line in display order:

```
Your tweet, formatted exactly as it should post.
Line breaks and emoji included. 🎉

===IMAGES===
chart.png
reaction.jpg
```

- **Text-only?** Just write the tweet — no delimiter needed. **Image-only?** Leave the text empty and start with `===IMAGES===`.
- Only the text **above** `===IMAGES===` is posted and counted toward 500. Everything below it is just the image list.

## How your PR gets merged

There is no formula. I rank the shortlist on:

- **Virality** — will it actually get impressions and engagement?
- **Fit** — right for my account and audience. It doesn't have to sound like me; informative or neutral tones are fine — just not lazy, generic filler.
- **Taste** — mine.
- **Track record** — if your past posts performed, that helps.

An agent narrows all open PRs to a top 5 each day; I pick the winner from there and merge it.

## What happens to your PR

- **Merged** → your post goes live and you earn the day's rewards.
- **Not picked** → closed at end of day. No backlog carries over. Submit again tomorrow.

## Don't

- Submit more than one PR per day.
- Edit your PR after opening it — description or files.
- Add anything beyond your dated `.md` and up to 4 images.
- Submit videos, or content that isn't ready to post as-is.

## Disclaimer

By submitting a PR you accept that I may post your work to my account and claim it as my own.
