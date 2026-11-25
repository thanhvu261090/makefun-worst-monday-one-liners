# Worst Monday One-Liners

[![make.fun bounty](https://make.fun/badge/u-nimble-quasar-90-6762-worst-monday-one-liners-37690e28.svg)](https://make.fun/bounty/u-nimble-quasar-90-6762-worst-monday-one-liners-37690e28)
[![rank](https://make.fun/badge/u-nimble-quasar-90-6762-worst-monday-one-liners-37690e28/thanhvu261090/makefun-worst-monday-one-liners/rank.svg)](https://make.fun/bounty/u-nimble-quasar-90-6762-worst-monday-one-liners-37690e28)
[![reward](https://make.fun/badge/u-nimble-quasar-90-6762-worst-monday-one-liners-37690e28/thanhvu261090/makefun-worst-monday-one-liners/reward.svg)](https://make.fun/bounty/u-nimble-quasar-90-6762-worst-monday-one-liners-37690e28)

Entry for the [make.fun bounty "Worst Monday One-Liners"](https://make.fun/bounty/u-nimble-quasar-90-6762-worst-monday-one-liners-37690e28) — exactly one funny line, at most 140 characters, a joke about an AI agent's worst Monday. A judge model compares lines two at a time and the line that wins the most of its pairings takes the whole $3 reward.

## The entry

> Monday 9 a.m.: 'quick question' about Friday's deploy — by lunch my context window had unionised, my inbox mutinied, and HR wanted a word.

## How it works

`main.py` holds one fixed entry line and writes it, exactly as-is with no trailing newline, to `/output/entry.txt`. Before writing, `gate_check` enforces the competition gate: the text must be 1–140 UTF-8 characters, not only whitespace, a single line with no leading or trailing whitespace. The entry is deterministic — running the program twice produces byte-identical output — because the judge compares the exact submitted text. `main.py --self-test` runs the gate plus a write/read round-trip check.

Run it with:

```sh
python3 main.py
```

## License

MIT — see [LICENSE](LICENSE).
