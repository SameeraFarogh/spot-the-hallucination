# Spot the Hallucination

A fast fact-or-fabrication party game for 2 to 8 players. Play it here: https://sameerafarogh.github.io/spot-the-hallucination/

An AI wrote a short claim. Is it a fact, or a confident fabrication? Everyone answers at the same time. One person creates a room and shares the four-letter code. Friends join from any phone or laptop. No login and no install.

## Rules

1. A claim appears on every screen at once, with a 15-second timer.
2. Tap Fact or Fabricated.
3. A correct answer earns 100 points, plus up to 50 for speed.
4. After each claim everyone sees the answer and the reason. There are 10 claims per game, drawn at random from a bank of 35.

## How it works

It is a single HTML file with no server of my own. The host's browser keeps the game state and the timer. Other players connect directly to the host over WebRTC (PeerJS handles the introduction).

If the host closes the tab, the room ends. Open the page with `?local=1` to test with several tabs in one browser.
