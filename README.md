# Solitaire (Klondike)

A free single-file HTML5 Klondike solitaire — the classic patience card game.
Build the four foundations from Ace to King, one suit per pile, on a classic
green-felt table with hand-drawn canvas cards.

**Play:** https://shuangyueliao.github.io/solitaire-klondike/

## How to play

- 52 cards are dealt into 7 tableau columns (column n gets n cards, top card
  face up); the remaining 24 stay in the stock.
- Build the 4 foundations up in suit from Ace to King.
- On the tableau, stack cards in alternating colors in descending order
  (red on black, black on red). Only a King (or a sequence led by a King)
  may move to an empty column.
- Draw from the stock into the waste: **Draw 1** (easy) or **Draw 3**
  (classic) modes. When the stock runs out, the waste is recycled back
  (−20 points per recycle, Draw-1 standard scoring).
- Move a single card or any valid sequence — drag it, or tap it and then tap
  the destination. Double-tap sends a card to its foundation.
- Safe autoplay: obvious cards fly to the foundations on their own; when only
  face-up cards remain the game auto-finishes.
- **Scoring** (Windows standard): waste→tableau +5, to foundation +10,
  tableau flip +5, foundation→tableau −15, stock recycle −20, time penalty
  −2 every 10 seconds. Score never goes below 0.
- **Hint** highlights one useful move (3 per game). **Undo** is unlimited.
- Win = all 52 cards on the foundations → the classic bouncing-card cascade.
- No-more-moves detection ends the game with an option to undo or restart.
- Records saved in localStorage: best score & fastest win per mode, total wins.

## Features

- Full standard Klondike rules, verified by a 58,000-assertion rules-engine
  test suite (alternation, King-on-empty, Ace-first foundations, stock
  recycling order, scoring floors, stuck detection incl. Draw-3 triplet
  masking, 20 randomized full-game simulations).
- Procedural everything: canvas-drawn card faces (geometric suit symbols +
  corner indices), lattice card backs, green felt table — no images.
- WebAudio synthesized sounds: deal, flip, place, foundation chime, error,
  undo, win fanfare. Mute toggle (persisted).
- 3D card-flip animation, staged deal animation, flying-card moves,
  classic winning cascade with paint trails.
- Mobile touch + desktop mouse: tap-select / tap-place, drag, double-tap;
  generous drop targets; responsive landscape-first canvas.
- Single file, zero external assets, no CDN, no fonts, no tracking, no
  external links.

## Tech

- One `index.html` (~48 KB), vanilla JavaScript + Canvas 2D + WebAudio.
- Portal SDKs load only on matching domains (CrazyGames / GameDistribution
  / gd.games) with gameplayStart / gameplayStop wired; the file runs
  standalone with no SDK calls.

## Files

- `index.html` — the whole game
- `.nojekyll` — bypasses GitHub Pages Jekyll processing
- `store/` — submission materials (description, GameDistribution zip, itch.io zip)

## License

MIT
