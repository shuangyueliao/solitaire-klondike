# Solitaire (Klondike) — Store Submission Materials

## Short description (CrazyGames / GameDistribution / itch.io)

The classic Klondike solitaire, free and full-featured. Build all four
foundations from Ace to King with Draw 1 or Draw 3 modes, unlimited undo,
smart hints and the famous winning cascade. How fast can you clear the deck?

(199 characters)

## Details

- Genre: Card / Patience / Casual
- Controls: Mouse / Touch. Drag a card (or a sequence) to its destination,
  or tap a card and then tap where it should go. Double-click / double-tap
  sends a card to its foundation. Keyboard shortcuts: U undo, H hint,
  N new game, M mute.
- Modes: Draw 1 (easy) and Draw 3 (classic). Stock recycles unlimited times.
- Rules: standard Klondike — red/black alternating descending tableau builds,
  Kings (or King-led sequences) on empty columns, Ace-first foundations.
- Scoring: Windows-standard — waste→tableau +5, to foundation +10, tableau
  flip +5, foundation→tableau −15, stock recycle −20 (floor 0), time penalty
  −2 per 10 seconds.
- Features: safe autoplay to foundations, auto-finish, unlimited undo,
  3 hints per game, no-more-moves detection, best score / fastest win /
  win count saved locally, winning card cascade.
- Tech: single-file HTML5 (~48 KB), vanilla JavaScript, Canvas 2D,
  WebAudio. Procedural graphics and sounds — no external assets, no CDN,
  no fonts, no tracking, no external links. Works offline once loaded.

## Tags

solitaire, klondike, cards, patience, classic, casual, puzzle, single-file

## CrazyGames submission checklist
- [x] Self-contained index.html (SDK loads only on crazygames domains)
- [x] gameplayStart / gameplayStop / loadingStart / loadingStop / happytime events wired
- [x] Responsive (canvas scales, landscape-first, touch friendly)
- [x] No external links inside gameplay, no analytics
- [ ] Cover: cover-16x9.png (1280×720)
- [ ] Screenshots: screenshot-raw.png (1280×800)

## GameDistribution
- Upload solitaire-klondike-gd.zip (contains index.html only).
- GD SDK auto-loads on gamedistribution / gd.games domains only.

## itch.io
- Upload solitaire-klondike-itch.zip, mark "This file is playable in browser",
  entry file: index.html, kind: html. Viewport: fullpage recommended.
- Pricing: $0 (donations optional)
