# Enduro HTML5

A single-file, dependency-free HTML5 Canvas recreation of **Enduro** — the 1983
endurance-racing classic. Pass the daily car quota before the clock runs out,
and survive a rolling cycle of day, dusk, night, fog, snow, and ice.

## Play

Open `index.html` in any modern browser. No build step, no server needed.

Or serve it locally:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## How to play

- Pass **200** cars on Day 1, then **300** every day after.
- Beat the daily quota before **TIME LEFT** hits zero, or it's game over.
- Crashing into a rival drops your speed and bounces you sideways.
- Drifting onto the grass slows you down — stay on the asphalt.

## Controls

| Action | Keys |
| ------ | ---- |
| Steer  | `←` `→` or `A` `D` |
| Gas    | `↑` or `W` |
| Brake  | `↓` or `S` |
| Pause  | `P` |

On touch devices, on-screen buttons appear automatically.

## Features

- Pseudo-3D projected road with curves, hills, rumble strips, and lane dashes.
- Seven-phase time-of-day / weather cycle, each with its own palette:
  morning, day, dusk, night, fog (reduced visibility), snow (falling flakes),
  and ice (slippery, sluggish steering).
- Daily quota, time bonus, score, and a persistent best score (localStorage).
- Keyboard + touch controls, responsive pixel-perfect scaling.

## Tech

Plain HTML/CSS/JavaScript rendering to a 320×240 canvas scaled up with
nearest-neighbour for a crisp retro look. Everything lives in `index.html`.
