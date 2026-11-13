# The Nervous System, One Concept at a Time

> **38 weeks · 190 lessons · 8 parts**  
> A reveal.js slide site generated from the Master Curriculum v1.2.

Live URL (once deployed): `https://YOUR_USERNAME.github.io/nervous-system-series/`

---

## Project Structure

```
nervous-system-series/
├── index.html                          ← Main entry point (all weeks wired here)
├── 00-introduction/
│   └── index.md                        ← Course overview slides
├── part-01-neurobio-foundations/
│   └── index.md                        ← Part I title + week list
├── week-01/
│   └── index.md                        ← 5 vertical lesson slides
├── week-02/
│   └── index.md
│   ...
└── week-38/
    └── index.md
```

**47 markdown files total** (1 intro + 8 part intros + 38 weeks).  
Each week file has **6 vertical slides**: a week header + 5 lesson slides.

---

## Navigation

| Key | Action |
|-----|--------|
| `→` | Next week / part |
| `↓` | Next lesson within the week |
| `Space` | Forward through everything |
| `Esc` | Overview map of all slides |
| `F` | Full screen |

URL format: `#/week-01`, `#/week-01/index`, `#/part-02`

---

## Setup — Local Preview

You need a **local HTTP server** (the Markdown plugin cannot load `.md` files directly from `file://`).

**Option A — Python (no install needed):**
```bash
cd nervous-system-series
python -m http.server 8000
# Open http://localhost:8000
```

**Option B — Node.js live-server:**
```bash
npm install -g live-server
live-server nervous-system-series
```

---

## Deploy to GitHub Pages

```bash
# 1. Initialise git
cd nervous-system-series
git init
git add .
git commit -m "Initial commit — full 38-week curriculum scaffold"

# 2. Push to GitHub
git remote add origin https://github.com/YOUR_USERNAME/nervous-system-series.git
git push -u origin main

# 3. Enable GitHub Pages
# → GitHub repo → Settings → Pages → Source: main branch, root folder → Save
```

Your site will be live at `https://YOUR_USERNAME.github.io/nervous-system-series/` within ~60 seconds.

---

## Editing a Lesson

Each lesson slide in `week-XX/index.md` follows this pattern:

```markdown
--

<div class="week-badge">Week X · Lesson X.Y</div>
<div class="lesson-code">X.Y — English Title</div>

## Short Concept Label

<div class="concept-label">Core Concept</div>
<div class="concept-text">Bulgarian concept text here.</div>

<div class="question-label">Guiding Question</div>
<div class="question-text">English or Bulgarian guiding question?</div>
```

- `---` separates **horizontal** slides (used between the week header and lesson block)
- `--` separates **vertical** slides (used between each lesson)

---

## Extending a Lesson

When you develop a full lesson (Blueprint v2.0), you can expand any `--` slide block with additional vertical slides:

```markdown
--

## Механистична карта / Mechanism Map

(diagrams, key terms, evidence labels)

--

## Practice / Демонстрация

(type, manipulation, mechanism, safety)

--

## Проверка на разбирането

(a single mechanism or prediction question)
```

---

## Tech Stack

| Component | Details |
|-----------|---------|
| Framework | [reveal.js 5.x](https://revealjs.com) via CDN |
| Content | External Markdown files per week |
| Hosting  | GitHub Pages (free static hosting) |
| Theme    | `night` + custom NS colour palette |

No build step, no `npm install`, no local dependencies required.

---

*Master Curriculum — Permanent Control Document · v1.2*
