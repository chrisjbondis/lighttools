# Guides Hub — Site Structure Plan

**Date:** 2026-08-05
**Status:** ✅ READY FOR BUILD
**Feeds into:** `ADSENSE-CONTENT-HANDOFF.md`

---

## For Claude Code — start here

Build order:

1. Create `/guides.html` — hub page listing all 9 existing guides, grouped into the 4 categories below, using the existing `.tool-card` grid styling from `index.html` for visual consistency (don't invent new card styling).
2. Add **"Guides"** to the main nav on every page, positioned after Fitting Selector / Sparky Selector, before About — see nav order below.
3. Add a small "Related Guides" block (2–3 links, not a wall of links) to each calculator page per the cross-linking table below.
4. Add `/guides.html` to the sitemap (standard step, already covered by the pre-deploy checklist).

Category structure and nav label are **confirmed by Chris — build as specified below, no further sign-off needed on those two points.**

---

## Why this matters now

Checked the live site structure: 9 guide/article pages already exist (3 original + the 6 just built from the exterior batch), and **none of them are linked from the main nav**. Right now they're only reachable by direct URL or search. That's a real problem beyond just navigation — for AdSense specifically, a pile of unlinked orphan pages reads worse than a smaller number of well-organised, clearly-linked ones. A Guides hub fixes both the UX gap and strengthens the "genuine, organised content" signal.

---

## Proposal

**1. New page: `/guides.html`** — a hub listing every article, using the same card-grid pattern already used for the calculators on the homepage (`.tool-card` styling) for visual consistency, so it doesn't look bolted on.

**2. Add "Guides" to the main nav**, positioned after the calculators/tools, before About:

```
Driver Calculator | Strip Selector | Lux Calculator | Garden Lighting | Voltage Drop | Fitting Selector | Sparky Selector | Guides | About | Disclaimer
```

**3. Category structure on the hub page** — grouping the guides so the page reads as organised rather than a flat list. Proposed categories based on what exists now plus what's planned:

| Category | Current guides | Planned (once built) |
|---|---|---|
| **Outdoor & Garden Lighting** | How Far Does Outdoor Light Travel, Why Fitting Construction Matters, In-Ground Fittings & IP68 Joins, Decorative & Accent Lighting, Fittings That Live in Water | Sensors/timers, Solar realistic expectations, Wildlife-friendly lighting, Seasonal/festive safety |
| **LED Strip & Driver Basics** | How to Install LED Strip Lighting, How to Choose an LED Strip Driver | Dimming Compatibility & Why LEDs Fail Early, Cove & Under-Cabinet Lighting |
| **Lighting Fundamentals** | What is Lux? | Choosing the Right LED (CCT/CRI/Beam Angle), How to Read a Photometric Datasheet/IES File |
| **Compliance & Standards** | RCD & Outdoor Lighting in Australia | Emergency Lighting & AS/NZS 1680 |

**Confirmed by Chris** — categories and nav label approved as drafted. RCD article stays primary-categorised under Compliance & Standards (it's cross-linked from the Outdoor category's related-guides context anyway via the calculator pages).

**4. Contextual cross-linking from calculator/tool pages** — this is the "relevant on other pages" part. Each calculator should surface a small "Related Guides" block (2–3 links, not a wall of links) pointing at genuinely relevant articles:

| Page | Related guides to surface |
|---|---|
| `garden-lighting-calculator.html` | How Far Does Outdoor Light Travel, Decorative & Accent Lighting, Fittings That Live in Water |
| `lux-calculator.html` | What is Lux?, (future) Choosing the Right LED |
| `led-strip-driver-calculator.html` | How to Choose an LED Strip Driver, (future) Dimming Compatibility |
| `led-strip-light-selector.html` | How to Install LED Strip Lighting |
| `fitting-selector.html` | Why Fitting Construction Matters, In-Ground Fittings & IP68 Joins, Fittings That Live in Water |
| `voltage-drop-calculator.html` | (future) Cove & Under-Cabinet Lighting once built |

This also quietly helps the calculators themselves — right now they're pure tools with minimal surrounding text; a related-guides block gives Google (and users) more context without padding the tool page itself with filler copy.

**5. Sitemap** — `/guides.html` needs adding once built; standard step already covered by the pre-deploy checklist.

---

## Status

All open items resolved 2026-08-05:
- ✅ Category structure and names — approved as drafted
- ✅ Nav label — "Guides", confirmed
- ✅ Timing — build now against the 9 existing guides; new cards get added incrementally as future articles (interior batch, exterior backlog) ship — each addition is a small follow-up job, not a re-scope

No open items remaining. Straightforward build — reuse existing card component styling from `index.html`, no new technical dependencies (no geocoding, no data source concerns like the Fitting Selector had).
