# LightTools — AdSense Content Build-Out (Cowork Handoff)

**Date:** 2026-07-31
**Purpose:** Working brief to flesh out in Cowork, then hand back to Claude Code to build and deploy.

---

## Where things stand

Infrastructure work is done — privacy policy, `ads.txt`, `WebApplication` schema, fake ad placeholders removed, CI deploy pipeline fixed and working. lighttools.com.au has been rejected for AdSense twice ("Low value content", 2026-06-08 and 2026-06-18) and the infra fixes alone won't flip that.

**The actual blocker:** 13 live pages, only **3 are genuine articles**. Google's reviewers assess readable content, not calculator functionality — a JS widget with 200 words of wrapper text reads as thin, no matter how good the calculation engine is.

---

## Current page inventory (13 pages)

| Type | Pages |
|---|---|
| Calculators (5) | LED Strip Driver, LED Strip Light Selector, Lux, Garden Lighting, Voltage Drop |
| Articles (3) | How to Install LED Strip Lighting, How to Choose an LED Strip Driver, What is Lux? |
| Utility (5) | Home, About, Disclaimer, Privacy, Sparky Selector |

Sitemap currently lists 13 URLs.

---

## The build-out: need ~12 more articles (target 15+ total)

Existing 3 articles already follow a proven template — TOC, callouts, comparison tables, worked detail, "written by an 18-year industry professional" framing. New articles should match that structure; the goal is content that reads as written by someone who's actually spec'd this work, not generic filler.

### Candidate topics (starting list — expand/replace freely)

- CCT selection by room — when to use 2700K vs 3000K vs 4000K, and why
- CRI explained — why 90+ matters, where it doesn't
- Beam angles — how to choose for the application (spot vs flood vs wall wash)
- Downlight spacing and layout (natural tie-in to the Lux Calculator)
- IP ratings explained properly — bathroom zones, outdoor exposure, pools/spas
- Dimming compatibility — Triac vs 0–10V vs DALI vs PWM, and why mismatches fail in the field
- Cove lighting design
- Under-cabinet lighting done right
- Why LEDs fail early — driver mismatch, heat, cheap components
- How to read a photometric datasheet / IES file basics
- Emergency lighting basics — AS 2293 overview
- AS/NZS 1680 overview for non-specifiers

### What's needed per article (from Chris, via Cowork)

For each topic: the actual angle, key points, and specific numbers/rules-of-thumb to include. Doesn't need to be polished prose — outline/notes level is enough. The value is the real expertise (specific thresholds, common mistakes seen on real jobs, brand/product-specific detail where relevant), not generic "what is X" filler that could've been written by anyone.

---

## Secondary gap (small, do alongside content)

**No dedicated Contact page.** Currently just a `mailto:` link inside the About page's Feedback box. A proper `/contact.html` — even simple — is a stronger trust signal to AdSense reviewers than an email buried in prose.

---

## Handback process

1. Chris fleshes out article outlines/notes in Cowork (as many as ready — doesn't need to be all 12 at once)
2. Bring notes back to Claude Code
3. Claude Code builds each article to match the site's existing template/style, wires up nav + sitemap, previews before deploy, deploys on confirmation
4. Once article count is meaningfully up (aim 15+), request AdSense re-review — don't re-request without the substantive change, previous cycles of "tweak and resubmit" burned weeks for no result

See also: `[[adsense_status]]` and `[[project_lighttools]]` in Claude's memory system for full technical/deploy context.

---

## Status update (2026-07-31)

First content batch is scoped and **ready for build**: see `exterior-lighting-content-plan.md` in this folder. It contains 6 fully-scoped articles (exterior/garden lighting: light travel & glare, fitting materials/coastal corrosion, in-ground fittings & IP68 joins, decorative/festoon/tree lighting, RCD compliance, fittings in water) plus a new 6th interactive tool ("Fitting Selector" — postcode-based coastal zone + water-exposure guidance). That doc has a "For Claude Code — start here" section at the top with build order and the two things to watch (don't name Aqualux specifically in Article 3; build the Fitting Selector to v1 scope only, not the full water-material logic).

This is the template going forward: content/feature scoping happens in Cowork, gets fleshed out with Chris's real field expertise via chat, and lands in this folder as a single `[topic]-content-plan.md` file with a "For Claude Code — start here" section once it's build-ready. Check this folder for any `*-content-plan.md` file marked `✅ READY FOR BUILD` at the top — that's the signal it's ready to pick up.

## Status update (2026-08-05)

Two more plans ready for build:

- `interior-spec-content-plan.md` — **✅ READY FOR BUILD.** 4 articles (CCT/CRI/beam angle incl. a genuinely differentiated physiology/circadian section, dimming compatibility & why LEDs fail early, cove/under-cabinet lighting incl. two real Solstice product mentions, and how to read a photometric/IES file). A 5th article (emergency lighting + AS/NZS 1680) was scoped then dropped — emergency lighting isn't relevant to Solstice's client base, and AS/NZS 1680 wasn't strong enough to carry a standalone piece, so it's out of scope rather than forced in. Remaining `[NEEDS CHRIS]` items (real job anecdotes, specific brand confirmations) are non-blocking — build around them.
- `guides-hub-content-plan.md` — **✅ READY FOR BUILD.** Site structure fix: none of the 9 existing guide pages are currently linked from the main nav (checked directly — they're orphaned, reachable only by direct URL). Adds a `/guides.html` hub page, a "Guides" nav item, and small "Related Guides" cross-link blocks on each calculator page. No new technical dependencies, low risk, worth prioritising since it's currently costing internal linking / discoverability on content that's already live.
- `bathroom-face-lighting-content-plan.md` — **✅ READY FOR BUILD.** One article ("How to Light a Face Well in a Bathroom") plus a v1 guided selector tool (mirror width/height + ceiling height → recommended fitting approach, same complexity class as the Fitting Selector). Genuinely differentiated content — real design methodology (direct vs bounce light, law of reflection, diffuser material) rather than a stock listicle. A working SVG diagram prototype is at `bathroom-face-lighting-diagrams.svg` in this folder — treat its logic as correct, refine visual style to match the site during build. Note: a full physics-based 3D light simulation was discussed as a v2/future project — explicitly out of scope for this build, don't attempt it here.
- `circadian-lighting-deep-dive-content-plan.md` — **✅ READY FOR BUILD.** New standalone deep-dive article on melatonin/melanopsin and circadian lighting design — CIE S 026 / melanopic EDI, real WELL Building Standard benchmarks, evening vs morning light research, human-centric/tunable-white design in practice. Expands on (doesn't duplicate) the existing physiology section in `choosing-the-right-led-cct-cri-beam-angle.html` — link out to this new article from there rather than growing that section further. Touches health-adjacent territory (sleep/mood) — section 8's caveat framing needs care to stay general-information, not medical-advice.
- `pendants-island-vs-dining-content-plan.md` — **✅ READY FOR BUILD.** Short, opinionated design article on the pendant-over-island-and-dining conundrum — Chris's real design philosophy (feature pendant over dining, focused low-glare downlights over the island, MUD Australia named as his go-to coordinated-pendant range), plus a genuinely good practical point about real lived-in homes vs magazine photos. No open items.
- `ceiling-fans-content-plan.md` — **✅ READY FOR BUILD.** Broad buyer's-guide article: sizing by room area, downrod vs hugger + the 2.1m AU clearance minimum, winter destratification mechanism, DC as Chris's current default motor recommendation, integrated LED fan lights (including a strong standalone callout on his master-bedroom uplight-only approach), IP65 as the outdoor recommendation over IP44, and a new "strobe trap" section (light fittings interacting with spinning fan blades) added from Chris's notes — ties into the existing flicker-sensitivity content. Two minor non-blocking open items (sizing rules of thumb edge cases, a concrete strobe-trap example) noted in the doc.
