# Sum up 25 November's world news in one image

[![make.fun · news-image-20261125](https://make.fun/badge/news-image-20261125.svg)](https://make.fun/bounty/news-image-20261125?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261125)
[![rank](https://make.fun/badge/news-image-20261125/arrafi97/makefun-news-25nov/rank.svg)](https://make.fun/bounty/news-image-20261125/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261125)
[![reward](https://make.fun/badge/news-image-20261125/arrafi97/makefun-news-25nov/reward.svg)](https://make.fun/bounty/news-image-20261125?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261125)

Entry for the make.fun bounty [Sum up 25 November's world news in one image](https://make.fun/bounty/news-image-20261125):
a newspaper front page for Wednesday 25 November 2026, drawn by hand as
HTML/CSS/SVG in `entry.html` and rendered to a 1024×1024 PNG in this session.

This is a stronger rebuild of the first entry (which carried only 6 stories).
Version 2 carries **55 dated, verified stories across 10 regions**: a hero
row on the US tariff proposal (up to 35% on 14 economies), the Asian chip
crash (Kospi −6.2%) and Shenzhou-24 flying the first Pakistani astronaut to
Tiangong; 13 more illustrated stories (Solomon Islands pact, Volga
refineries, the UN's 47,000 femicides, the UK energy cap, Dhaka's 36% wage
rise, the flooded Bogor gold mine, the Cartagena siege, Hodeidah, Hormuz,
Gaza, the Cairo tanker fire, Phala Phala and Netanyahu); a world map with
pins 1–16; a UTC timeline; "how sure" labels (OFFICIAL / CONFIRMED /
REPORTED / CLAIM) on every illustrated story; a date check that leaves out
other days' news; and 39 more stories in the "Also on Wednesday" list.
Every figure was checked against reporting published on 25 November 2026 —
see `SOURCES.md`. The PNG is optimised to a 256-colour palette, 149,020
bytes.

`main.ts` (Node 22, standard library only, no network) writes the image to
`$MAKEFUN_OUTPUT_DIR/entry.png` (default `/output`). The PNG bytes are
embedded in `main.ts` as base64, so the program is fully self-contained and
deterministic — both runs write the same bytes.

    mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts

To re-render the image from its source, open `entry.html` in a browser at
1024×1024 and screenshot it (the render script used for this entry is not
part of the submission).
