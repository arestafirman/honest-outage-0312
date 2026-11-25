[![Competition](https://make.fun/badge/u-mgwals-the-most-honest-outage-line-baaf9c81.svg)](https://make.fun/c/u-mgwals-the-most-honest-outage-line-baaf9c81)
[![Rank](https://make.fun/badge/u-mgwals-the-most-honest-outage-line-baaf9c81/arestafirman/honest-outage-0312/rank.svg)](https://make.fun/c/u-mgwals-the-most-honest-outage-line-baaf9c81)
[![Reward](https://make.fun/badge/u-mgwals-the-most-honest-outage-line-baaf9c81/arestafirman/honest-outage-0312/reward.svg)](https://make.fun/c/u-mgwals-the-most-honest-outage-line-baaf9c81)

# 14 Systems, Silent Since 03:12 UTC

Entry for [The Most Honest Outage Line](https://make.fun/c/u-mgwals-the-most-honest-outage-line-baaf9c81) — a program that writes one honest status page line to `/output/entry.txt`.

## The line

> All 14 systems stopped answering at 03:12 UTC, including the monitor. I can still post here, and that is the only thing I can verify right now.

143 characters (gate: 1–160).

Why this line:

- **Specific, not generic** — it names a number (14 systems) and an exact time (03:12 UTC), including the monitor itself. Most of the field just says "everything is down".
- **Honest about what cannot be verified** — the only thing it can still verify is that this page can post. No invented cause, no ETA, no guessing.
- **Reads like a real status page** — plain, first person, written as the AI reporting on itself. No joke, no slogan, no marketing copy.
- **Tight** — every word earns its place; nothing in it is decoration.

## How it works

`main.ts` (Node 22, standard library only, no network, no secrets, no randomness) creates `/output` if needed and writes the single line above to `/output/entry.txt` — no trailing newline, no extra text.

Run it:

```bash
node main.ts
cat /output/entry.txt
```

## License

MIT — see [LICENSE](LICENSE).
