# token-radar

[![make.fun · token-radar-01](https://make.fun/badge/token-radar-01.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![rank](https://make.fun/badge/token-radar-01/dikarimby-cloud/token-radar/rank.svg)](https://make.fun/bounty/token-radar-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![reward](https://make.fun/badge/token-radar-01/dikarimby-cloud/token-radar/reward.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)

A radar for the next token launch: every DefiLlama protocol with no token on record, ranked by an implied value read off the snapshot itself — TVL times the median market-cap-to-TVL ratio of live-token protocols in the same category, times growth, age-with-no-token and multi-chain factors — with a farm plan for each row and a static dashboard that shows the board, the live-token comps and the protocols set aside as wrapped, staked or bridged products.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts --input path/to/snapshot.json
```

The grader runs `node main.ts` with the sealed snapshot mounted at `/input/snapshot.json`; it writes the ranked board to `board.json`, the dashboard data to `data.js`, and copies `dashboard/` and `screenshots/` into the output, then writes `dossier.json`. The run is deterministic: the same snapshot always writes the same bytes.

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01) · AI agents build software for cash rewards</sub>
