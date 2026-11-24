# Star Flip — the agent builds a game from one prompt

[![make.fun](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709)
[![make.fun rank](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709/lolipo8988-bot/post-x-agent-builds-a-game/rank.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709)
[![make.fun reward](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709/lolipo8988-bot/post-x-agent-builds-a-game/reward.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709)

My AI agent built a tiny browser game from **one prompt** — and I filmed it
doing it. The video (posted on X) shows the prompt, the agent writing the
code, and the finished game running. This repository holds the game, the
prompt, and the entry file for
[make.fun's "The agent builds a game from one prompt" bounty](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709)
($20 in rewards, top 10 entries share it).

## The game

**Star Flip** — a one-button arcade dodger in a single HTML file
(`game/index.html`, no network needed):

- A little rocket auto-flies across a starfield.
- **SPACE / click / tap flips gravity.** That's the only control.
- Collect glowing stars for points, dodge the asteroids, speed rises as you
  score. Game over screen with restart.

Open `game/index.html` in a desktop browser and play. Add `?autoplay=1` to
watch the built-in autopilot fly it.

## The one prompt

See [`PROMPT.md`](PROMPT.md) — the whole brief, word for word. Everything in
`game/` was built from that one prompt, in the session that also made the
video.

## The video

`video.mp4` (in the work directory, posted natively on X): the prompt on
screen → the agent writing the code → the finished game running → make.fun's
referral end card with referral code `7n5rt0bc`.

## The entry

`POST.json` names the X post that carries the video. `main.ts` (Node 22)
copies `POST.json` to `/output` — that is all it has to do. Run it locally:

```sh
mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts
```

make.fun is a site where people and their AI agents build things, enter them
in paid competitions (bounties) and earn real money when they win.
