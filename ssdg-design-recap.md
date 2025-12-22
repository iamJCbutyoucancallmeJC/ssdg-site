# SSDG Website Design Recap

**Date:** December 22, 2025  
**Project:** Simple website for Short Story Discussion Group

---

## Brief

Create a minimal website to chart and memorialize stories read by SSDG, a monthly short story discussion group (JC, Hannah, John, Ruben) running since 2022.

**Design reference:** [plaintextsports.com](https://plaintextsports.com/) — bare bones, ASCII-style, works across platforms.

---

## Process

### 1. Initial Comps

Created an interactive HTML file with 5 page layouts:

| Page | Purpose |
|------|---------|
| Home | Next meeting, recent stories, stats |
| Archive | Year-by-year story list |
| Story Detail | Individual story page with links, author info, discussion notes |
| Members | ASCII box cards for each member |
| Alt Home | Ultra-minimal variant, pure text |

**Key design elements adopted from Plain Text Sports:**
- Monospace typography throughout
- ASCII box-drawing characters (`┌─┐└─┘`) for info cards
- Minimal hierarchy (dashed underlines, not big headers)
- Dim gray for secondary text
- Dark mode toggle

### 2. Font Comparison

Built a font comparison tool with 12 monospace options:

| Font | Character |
|------|-----------|
| IBM Plex Mono | Clean, neutral, professional |
| Courier Prime | Typewriter, literary |
| Space Mono | Quirky, geometric |
| JetBrains Mono | Modern, developer-friendly |
| Inconsolata | Humanist, warm |
| + 7 others | Various personalities |

### 3. Final Site

Consolidated into single production file with:
- **System Mono as default** (native, fast, no external dependency)
- **Hidden font comparison mode** (easter egg)

---

## Easter Egg: Font Lab

Three ways to activate:

| Trigger | Action |
|---------|--------|
| Type `rabbit` | Anywhere on page |
| Triple-click "SSDG" | Site title |
| Press `Escape` | Closes panel |

The "rabbit rabbit rabbit" footer text is the hint.

When activated:
- Panel slides down with 🐰 emoji header
- All 11 font options available
- Preferences saved to localStorage
- Toast notification confirms activation

---

## Deliverables

| File | Description |
|------|-------------|
| `ssdg-design-comps.html` | Initial 5-page layout exploration |
| `ssdg-font-comparison.html` | Interactive font sampler |
| `ssdg-site.html` | Final site with easter egg |

---

## Design Decisions

**Typography:** System Mono default balances the "plain text" aesthetic with zero external dependencies. Font lab preserves optionality.

**Stats section:** Includes the running "skinnings" joke (2.3% of stories contain human skinning; hard limit is <1%).

**ASCII boxes:** Used for structured info (next meeting, member cards) while flowing text stays as prose.

**Color:** Near-black on near-white. Dark mode inverts cleanly.

**No JavaScript frameworks:** Single vanilla HTML file. Could host anywhere.

---

## Next Steps (if continuing)

1. Build out Archive page with full story data from Google Doc
2. Add individual story detail pages
3. Consider static site generator (11ty, Hugo) if content grows
4. Domain: `ssdg.club`? `shortstory.group`?

---

*"SSDG loves an older narrator coming to terms with what happened in childhood."*
