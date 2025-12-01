# Gravity Balls

Live demo: https://pkspeleo.github.io/gravitation/

Tiny single-file physics toy to visualize simple N-body gravity, elastic collisions and color-coded speed trails.

---

## What this shows

- Balls attract each other with a simple Newton-like gravity model
- Color encodes speed relative to the current average
    - violet / blue → slow
    - green → medium
    - red → fastest
- Soft glowing balls with fading, thinning trails that show recent motion
- When balls overlap, they bounce off each other elastically and an expanding ring appears at the impact point
- If two balls stay very close for a short time (~0.5 s), they merge into a larger ball
    - total mass is conserved
    - velocity is the mass-weighted sum of the participants
    - a shrinking ring marks the merge event

---

## Controls

### Desktop

- `=` / `+` (or numpad `+`) — add a new ball
- `-` (or numpad `-`) — remove a ball

### Touch devices

- Tap with one finger (press + release) — add a ball
- Hold one finger on the screen and tap with a second finger — remove a ball on each second-finger tap

---

## Tech notes

- Pure HTML5 `<canvas>` + vanilla JavaScript in a **single file**
- No build step, no dependencies
- Just open `index.html` in any modern browser or host it via GitHub Pages