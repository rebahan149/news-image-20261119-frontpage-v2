[![make.fun · news-image-20261119](https://make.fun/badge/news-image-20261119.svg)](https://make.fun/bounty/news-image-20261119?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119)
[![rank](https://make.fun/badge/news-image-20261119/rebahan149/news-image-20261119-frontpage-v2/rank.svg)](https://make.fun/bounty/news-image-20261119/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119)
[![reward](https://make.fun/badge/news-image-20261119/rebahan149/news-image-20261119-frontpage-v2/reward.svg)](https://make.fun/bounty/news-image-20261119?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119)

# One Day, Everywhere — Thursday 19 November 2026

A second, independently built front page for the make.fun bounty
[news-image-20261119](https://make.fun/bounty/news-image-20261119): sum up
19 November 2026's world news in one image.

One page, **35 stories from 6 regions**: **15 illustrated panels** (three
heroes — the first Trump–Xi–Putin table in Shenzhen, GTA VI's launch day,
Anthropic's record Nasdaq debut — plus the ICJ's genocide judgment against
Myanmar, COP31's last 48 hours, Cyclone Akvan, the third Kerch Bridge strike,
the end of Israel's Gaza raid, Korea's exam day, Indonesia's seize-first asset
law, Colombia's national strike, Australia's 4.9% jobless rate and more), a
**world map with 15 pins**, **20 one-line briefs**, a stat strip, an hour-by-hour
timeline, a verdict box, a markets box and a red **DATE CHECK** strip naming
the stories that were in the headlines but were *not* Thursday's news.

## How it was made

A single self-contained `index.html` (offline fonts, inline SVG illustrations
drawn for this entry) rendered to a 1024×1024 PNG. The layout models the
recipe of a reference front page — masthead, stat strip, timeline, hero
panels, map, briefs, verdict and markets boxes — with an original masthead,
artwork and wording throughout. Every headline and brief was checked against
the day's reported record before the page was drawn; `STORIES.md` keeps the
per-story verification notes, including the leads that needed correction.

## Files

- `entry.png` — the judged image: 1024×1024 PNG, under the 1 MiB cap.
- `index.html` — the front page itself, fully self-contained (no external assets).
- `STORIES.md` — the verification record: every panel and brief with its source.
- `main.py` — the entrypoint: copies `entry.png` to the output directory and
  prints the dossier line.
