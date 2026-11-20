# NSS course site — instructions for Claude

Docsify site, published by GitHub Pages from `main`. Same setup as the Game Theory course (undercurremt/GameTheory).
Lessons are written by the author (in Bulgarian, via ChatGPT); Claude only files and publishes them.
Never edit lesson text unless explicitly asked.

## Publishing lessons the author sends
1. Save each attached/pasted lesson to a temp file, then run `python tools/build.py add <file> [<file> ...]`.
   It detects the lesson number from the first heading (e.g. `# Lesson 017 — Somatosensation, ...`), saves it as
   `part-PP/lesson_NNN_<title_slug>.md` and regenerates navigation. The lesson text is saved unchanged.
   If the number can't be detected, ask the author which lesson it is.
2. `git add -A && git commit -m "Publish lesson NNN"` and push to `main`. Report the live URL:
   https://undercurremt.github.io/NSS/#/part-PP/lesson_NNN_<title_slug>

## Rules
- `curriculum.yaml` is the source of truth: NS Master Curriculum Control v1.4 (18 November 2026), Appendix A —
  the v1.3 base index of 170 lessons in 8 parts, published with sequential numbers 001–170 (no weeks).
  `v13` on each lesson keeps the original week.lesson code (e.g. 006 = 2.1) for reference only.
- Lessons 001–005 (formerly 1.1–1.5) are locked: never edit their text.
- Lesson 006 is the former v1.3 lesson 2.1; only its first heading was renumbered.
- Generated, never edit by hand: `_sidebar.md`, `part-*/README.md`, `book-pages.js`, progress line in `README.md`.
  Change `curriculum.yaml` and run `python tools/build.py` instead.
- UI labels on generated pages are in English (Core concept, Guiding question).
- Requires `pip install pyyaml`.
