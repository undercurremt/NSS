# NSS course site — instructions for Claude

Docsify site, published by GitHub Pages from `main`. Lessons are written by the author (in Bulgarian, via ChatGPT);
Claude only files and publishes them. Never edit lesson text unless explicitly asked.

## Publishing lessons the author sends
1. Save each attached/pasted lesson to a temp file, then run `python tools/build.py add <file> [<file> ...]`.
   It detects the lesson number from the first heading (e.g. `# 1.6 ...`), saves it as
   `module-MM/lesson_M_L_<title_slug>.md` and regenerates navigation.
   If the number can't be detected, ask the author which lesson it is.
2. `git add -A && git commit -m "Publish lesson X.Y"` and push to `main`. Report the live URL:
   https://undercurremt.github.io/NSS/#/module-MM/lesson_M_L_<title_slug>

## Rules
- `curriculum.yaml` is the source of truth: Master Curriculum Control v1.4 (final) — 8 modules, 103 lessons
  (title, core concept, guiding question, dependencies). No weeks.
- Lessons 1.1–1.5 are locked: never edit their text.
- `archive/` holds lessons that are not part of the current index (e.g. the v1.3 lesson 2.1). Not linked on the site; don't publish or edit.
- Generated, never edit by hand: `_sidebar.md`, `module-*/README.md`, `book-pages.js`, progress line in `README.md`.
  Change `curriculum.yaml` and run `python tools/build.py` instead.
- UI labels on generated pages are in English (Core concept, Guiding question, Dependencies).
- Requires `pip install pyyaml`.
