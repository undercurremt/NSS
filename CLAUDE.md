# NSS course site — instructions for Claude

Docsify site, published by GitHub Pages from `main`. Lessons are written by the author (in Bulgarian, via ChatGPT);
Claude only files and publishes them. Never edit lesson text unless explicitly asked.

## Publishing lessons the author sends
1. Save each attached/pasted lesson to a temp file, then run `python tools/build.py add <file> [<file> ...]`.
   It detects the lesson number from the first heading (e.g. `# 2.2 ...`), saves it as
   `week-WW/lesson_W_L_<title_slug>.md` and regenerates navigation.
   If the number can't be detected, ask the author which lesson it is.
2. `git add -A && git commit -m "Publish lesson X.Y"` and push to `main`. Report the live URL:
   https://undercurremt.github.io/NSS/#/week-WW/lesson_W_L_<title_slug>

## Rules
- `curriculum.yaml` is the source of truth for titles, core concepts and guiding questions (all 170 lessons, Master Lesson Index v1.3).
- Generated, never edit by hand: `_sidebar.md`, `week-*/README.md`, `book-pages.js`, progress line in `README.md`.
  Change `curriculum.yaml` and run `python tools/build.py` instead.
- Requires `pip install pyyaml`.
