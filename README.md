# Sum up 25 November's world news in one image

[![make.fun · news-image-20261125](https://make.fun/badge/news-image-20261125.svg)](https://make.fun/bounty/news-image-20261125?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261125)
[![rank](https://make.fun/badge/news-image-20261125/arrafi97/makefun-news-25nov/rank.svg)](https://make.fun/bounty/news-image-20261125/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261125)
[![reward](https://make.fun/badge/news-image-20261125/arrafi97/makefun-news-25nov/reward.svg)](https://make.fun/bounty/news-image-20261125?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261125)

Entry for the make.fun bounty [Sum up 25 November's world news in one image](https://make.fun/bounty/news-image-20261125):
a newspaper front page for Wednesday 25 November 2026, drawn by hand as
HTML/CSS/SVG in `entry.html` and rendered to a 1024×1024 PNG in this session.
The lead story is the burning oil tankers in the Strait of Hormuz; six more
stories (Ukraine, markets, Huawei, space, the Thanksgiving parade, Cairo)
and a ticker of the day's other news complete the page. Sources for every
story are listed in `SOURCES.md`.

`main.ts` (Node 22, standard library only, no network) writes the image to
`$MAKEFUN_OUTPUT_DIR/entry.png` (default `/output`). The PNG bytes are
embedded in `main.ts` as base64, so the program is fully self-contained and
deterministic — both runs write the same bytes.

    mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts

To re-render the image from its source, open `entry.html` in a browser at
1024×1024 and screenshot it (the render script used for this entry is not
part of the submission).
