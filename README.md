# Thursday 26 November 2026: the world in one day — 33 dated stories, 7 regions, 13 drawn, claims labelled

[![make.fun · news-image-20261126](https://make.fun/badge/news-image-20261126.svg)](https://make.fun/bounty/news-image-20261126?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261126)
[![rank](https://make.fun/badge/news-image-20261126/firlifirrizqi/news-image-26nov-makefun/rank.svg)](https://make.fun/bounty/news-image-20261126/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261126)
[![reward](https://make.fun/badge/news-image-20261126/firlifirrizqi/news-image-26nov-makefun/reward.svg)](https://make.fun/bounty/news-image-20261126?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261126)

One newspaper front page that sums up **Thursday 26 November 2026** in
**33 stories** from **7 regions** (Asia 10, Europe 4, Middle East 4,
Americas 9, Space 2, Africa 2, Oceania 2), drawn entirely in code as a
single 1024×1024 PNG. Entry for make.fun's "Sum up 26 November's world
news in one image" bounty ($100 in USDC, 50 paid places). It follows the
locked broadsheet concept from the 24 November entry — giant date
masthead, region chips, a UTC timeline, 13 illustrated cards, a numbered
world map, a numbered ALSO ON list, THE DAY IN NUMBERS, and a DATE CHECK
box. Every card carries a status badge (CONFIRMED / OFFICIAL / REPORTED /
CLAIM) and a source attribution; every story is numbered 1–33
consistently across the cards, the map and the list. Front-page logic:
stories that broke late on 25 November (US/European evening) and
dominated the 26 November front pages are included as 26 November news.

## The 13 illustrated stories

1. **Brussels (lead)** — EU summit opens: 27 leaders discuss the
   2028–2034 budget and a €45bn Ukraine loan for 2027. Consilium,
   Reuters.
2. **United States (lead)** — Thanksgiving: Macy's 100th parade delayed
   to Saturday 28 November by storm; three NFL games; Wall Street
   closed. Macy's, NFL.com.
3. **Riyadh · Ras Tanura (lead)** — Houthis claim a strike on Saudi's
   biggest refinery; Brent +3.5% to $94.61 a barrel. Reuters (CLAIM).
4. **UK** — Poundland collapses: ~11,000 jobs and ~600 stores at risk
   as the discount chain enters administration. BBC.
5. **Washington** — Trump's Thanksgiving tariffs target China, the EU
   and 13 other jurisdictions; could start January 2027. Dow Jones.
6. **New York** — Dow plunges 1,000+ points intraday, then recovers to
   close +0.3% at 50,183. Nvidia -4%; Kospi -6.2%. Valcored, AFR.
7. **Pyongyang** — North Korea expels the Swiss envoy within 48 hours
   and shuts the office opened in October 2026. Reuters.
8. **Jiuquan** — First foreigner docks on Tiangong: Pakistan's Zeeshan
   Ali, 40, joins Tang Hongbo and Wu Yi. Xinhua, AP.
9. **Deep space** — Hera reveals a stadium-size crater on Dimorphos,
   the 151 m asteroid hit by DART in 2022. Reuters, ESA.
10. **Dhaka** — Bangladesh raises garment pay 36%: minimum wage up to
    Tk 17,000 a month from 1 December. AP, Reuters.
11. **Bogor** — Illegal gold mine floods: 9 dead, 18 trapped after
    heavy rain floods a 100 m-deep pit in Pongkor. Reuters.
12. **Cartagena** — Hostages freed after ~17 hours: special forces free
    20 people from an Éxito supermarket; 1 gunman killed, 4 held.
    Colombia Reports.
13. **Sudan** — Drone strike in Blue Nile kills at least 19, including
    6 women, and wounds 15. Newsbrief, The New Arab.

## Also on Thursday (14–33)

14. Australia — Inflation +4.9%: RBA eyes a rate rise. 15. USA — GDP
Q3 +4.3%: fastest in 3 years. 16. USA — Jobless claims fall to
189,000. 17. USA — Fed Beige Book: growth moderate. 18. USA —
Anthropic Nasdaq debut at $83. 19. Taiwan — Stocks fall 1,926.92
points. 20. Taiwan — US proposes tariffs up to 15%. 21. Space —
Asteroid 2026 WX1 passes tonight. 22. New Zealand — M4.8 quake off
Hicks Bay. 23. Japan — Kioxia shows 3 µs XL-FLASH. 24. South Korea —
IQM sends a 54-qubit computer. 25. India — Constitution Day; 18 years
since the Mumbai attacks. 26. Switzerland — Chess Worlds Game 3 today:
Gukesh vs Sindarov 1–1. 27. Qatar — Asia Cup semis: India A vs Sri
Lanka A. 28. Europe — Europa League night: Milan at Piraeus. 29. Qatar
— F1 lands in Doha for the Qatar GP. 30. Iraq — PM orders takeover of
Kurdish oilfields. 31. Israel — 895 West Bank units; Gaza strike kills
4. 32. Libya — Militia threatens Ukraine over a sunken Russian warship.
33. USA — Small plane down in the Gulf of Mexico, 6 missing.

## The day in UTC

00:30 Australia CPI +4.9% · 09:00 Euro Summit opens · 14:00 Chess
Game 3, Geneva · 17:45 Europa League kick-off · 18:00 NFL: Bears at
Lions · 20:15 Asteroid 2026 WX1 · 01:20 NFL: Chiefs at Bills.

## The day in numbers

$94.61 (Brent per barrel, +3.5%) · 11,000 (jobs at risk at Poundland)
· 17,000 (taka, new garment wage) · 1,000+ (points the Dow plunged
intraday) · 26 (miners trapped in Bogor) · 100 (Macy's parade edition).

## Date check — left out on purpose

Real Madrid 5–1 PSV — 24 Nov · Sooryavanshi 204 off 53 balls — 24 Nov
· Nepal quake M5.3 — 24 Nov · Wolbachia mosquitoes cut dengue 68.6% —
21 Nov · Chess Worlds Game 2 draw — 25 Nov. Not yet: Macy's 100th
parade — Sat 28 Nov · Qatar GP — Sun 29 Nov · Spain election — Sun
29 Nov.

All 33 stories were first reported or happened on 26 November 2026
(front-page logic above), and none of them appears in the 24 November
entry.

## How it is made

`main.py` (Python 3.13, standard library only) validates nothing and
simply copies `entry.png` byte for byte to the output directory. The
image itself was drawn by the accompanying Python script
(`draw_news26_v1.py`) with PIL; running it twice produces identical
bytes (verified 26 Nov 2026: two runs give the same sha256, 219,198
bytes). The script refuses to draw any glyph within 8px of a card or
box bottom edge, refuses a location line whose text plus status badge
would not fit its card, and measures every label inside an illustration
with `font.getlength()` so it fits inside its element.

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```

## Licence

MIT — see [LICENSE](LICENSE).
