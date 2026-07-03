# klara & hazel

A 10,000 × 10,000 word search. Two words are hidden in it — `KLARA` and `HAZEL`. Pan and zoom to find them.

**Live: https://hazelandklara.com**

## Stats

- **100,000,000 letters** (10,000 × 10,000 grid)
- **10** of them are deliberately placed — one `KLARA`, one `HAZEL` (0.00001% of the grid)
- The other **99,999,990** are generated deterministically from a constant seed, so the puzzle is identical on every load and every device
- Printed at standard word-search density (~5 mm per letter), the puzzle would be a square roughly **50 meters on a side**
- In 100 million random letters, any given 5-letter word is statistically expected to appear by chance a few dozen extra times — so there are almost certainly accidental `KLARA`s and `HAZEL`s out there too, but only one official placement of each

## How it works

Nothing is stored: each letter is computed on demand from a hash of its grid coordinates mixed with the seed, and only the cells currently visible are drawn to a canvas. Drag to pan; pinch, Ctrl/Cmd-scroll, or double-click to zoom.

The whole site is a single dependency-free `index.html`. (The exact word placements are in a clearly marked spoiler comment near the top of the file.)
