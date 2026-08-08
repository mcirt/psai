Pyramid Solitaire v1.4.0

Files:
- index.html
- game.html
- solver.html

v1.4.0 highlights
- +500 completion bonus restored.
- +1260 time bonus restored on completion.
- Perfect-score target = 8260.
- Solver gives completed solutions priority over unfinished high-score partial paths.
- Full-plan search still uses a 25,000-state cap and clearly reports BEST COMPLETE vs BEST PARTIAL.
- Search summary shows best completed score, best partial score, inventory used, perfect-score candidates, and whether an 8260 route is still alive.
- Solver is seeded with the known perfect-score inventory setup family:
  * draw 8
  * draw 1, hold 31, draw 7 more
  * draw 2, hold 34, draw 6 more
  * draw 3, hold 37, draw 5 more
  * draw 4, hold 40, draw 4 more
  * draw 5, hold 43, draw 3 more
  * draw 6, hold 46, draw 2 more
  * draw 7, hold 49, draw 1 more
  * draw 8, hold 52
- Hold search can now consider Kings too when strategically useful.
- Solver Draw playback flashes the Draw button and shows a counter directly above it, including 1/1 for a single draw and 1/N, 2/N... for consecutive draws.
- Card highlights, click-to-match, drag-to-match, and Hold interactions remain enabled.
- Complementary half-color card visuals remain unchanged.

Scoring
- Scoring streak: 50, 100, 150, 200, then 250 for each later scoring action.
- Draw breaks the streak.
- Reset costs up to 50 points (score never below zero).
- Completion adds 500 points.
- Completion time bonus adds 1260 points.
- A perfect 8260 route requires 6500 gameplay points + 500 completion + 1260 time bonus and consumes all 24 inventory cards.

Important
- A 25,000-state beam search can find strong complete solutions, but BEST FOUND is not a mathematical proof of optimality unless the search explicitly reports otherwise.
