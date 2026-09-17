# Artificial Light, Melatonin & Melanopsin — Deep Dive Content Plan

**Date:** 2026-08-05
**Status:** ✅ READY FOR BUILD
**Feeds into:** `ADSENSE-CONTENT-HANDOFF.md`

---

## For Claude Code — start here

Build this as a new standalone article per the structure below, and add a link out to it from the existing "Why this actually matters" section in `choosing-the-right-led-cct-cri-beam-angle.html` (that section stays as-is — don't expand it further, this new article is where the depth goes). Slot into the Guides hub under Lighting Fundamentals per `guides-hub-content-plan.md`, and add to the sitemap per the standard pre-deploy checklist.

Section 8 (health-adjacent caveats) needs care in the actual writing — keep it general-information framed, not medical advice, per the plan below. No other blockers; remaining `[NEEDS CHRIS]` notes are resolved or explicitly non-blocking (see Open Items).

---

## What's already live (checked first, per your steer)

`choosing-the-right-led-cct-cri-beam-angle.html` already has a "Why this actually matters — light, physiology and how we function" section covering: the ipRGC/melanopsin mechanism, ~480nm peak sensitivity, an 1800K advanced callout, and flicker sensitivity. That section should stay as-is — it's the right length for that article. This new piece is the **proper deep dive** that section can link out to, going well beyond what's already published, with genuine additional research and design-standard detail most competitor content doesn't have.

---

## Why this is a strong pillar piece

Human-centric/circadian lighting is a live, growing area of the lighting industry right now — premium residential, aged care, and commercial fitouts are increasingly specifying for it. Most content on this topic online is either dry academic papers or vague wellness-blog hand-waving ("warm light helps you sleep!"). Almost none of it gives an actual design framework tied to real standards. This article can.

---

## Article structure

**Working title:** How Artificial Light Actually Affects You — Melatonin, Melanopsin & Designing for the Body Clock

1. **Quick recap, then go deeper (links back to Article A rather than repeating it)**
   - One paragraph recap: ipRGCs, melanopsin, the non-image-forming pathway to the suprachiasmatic nucleus (SCN) — then straight into new material

2. **The measurement gap most people don't know exists: lux isn't the whole story**
   - Standard lux measures brightness as the cone-based visual system perceives it. It says nothing about how strongly that same light stimulates the melanopsin system, because that depends on spectral content, not just apparent brightness or even CCT number
   - **CIE S 026** is the international standard (published 2018, still the reference standard) that defines how to actually measure this — introducing **melanopic EDI (melanopic Equivalent Daylight Illuminance)**, which weights light by its biological effect on the circadian system rather than just visual brightness
   - Practical translation: two fittings can read as the same CCT and lux level to a human eye and a standard lux meter, and still have meaningfully different melanopic effect depending on their actual spectral makeup — this is a genuinely non-obvious point worth making explicitly, since it means "just pick warm CCT" is a good rule of thumb but not the full picture at the professional end of this topic

3. **Real design benchmarks — WELL Building Standard**
   - WELL v2: minimum 200 equivalent melanopic lux (EML) at 75%+ of workstations, measured vertically at 1.2m, present 9am–1pm
   - WELL v6 (current): raised to 250 EML under the same measurement approach
   - Framing: most residential/small-commercial work will never need formal WELL certification, but knowing the actual professional benchmark exists — and what it targets — is useful context for positioning a genuinely well-designed lighting scheme, and for talking with commercial/aged-care clients who *do* care about this formally
   - **Resolved:** no real examples yet — keep this section as background/context only, not case-study-led

4. **What actually happens with evening light exposure — the research**
   - Cool white LED/CFL sources suppress melatonin considerably more than warm white or incandescent equivalents (already touched briefly in Article A — this section goes further)
   - A genuinely striking comparative finding worth featuring: extended evening blue-light exposure has been shown to produce meaningfully longer circadian delays than equivalent exposure to longer-wavelength (green) light — i.e., it's not just "blue light is bad," it's that blue-rich light has a disproportionately larger and longer-lasting effect on the body clock than other colours at the same brightness
   - Practical translation for evening living spaces and bedrooms: this is the mechanism behind why CCT choice for evening-use rooms is a genuine design decision, not just an aesthetic preference — ties directly to Article A's CCT defaults and the 1800K advanced note

5. **What actually happens with morning light exposure — new material, not covered elsewhere on the site**
   - Morning bright light exposure is linked to increased alertness, improved mood, healthy cortisol regulation, and better subsequent sleep quality — the same ipRGC/SCN pathway responsible for evening disruption is just as active (and useful) in the morning
   - Short-wavelength light in the ~446–477nm range is the strongest circadian synchronising signal humans respond to — meaning morning spaces (kitchens, home offices, bathrooms used at the start of the day) are a genuine design opportunity, not just evening spaces being a design risk
   - Practical translation: cooler CCT and brighter levels in morning-use spaces isn't just "task lighting," it's actively supporting the body's wake-up signal — a nice reframe of something people already do instinctively (bright kitchen lighting) with the actual mechanism behind why it feels right
   - **Brief, appropriately cautious note:** morning bright light exposure is also used clinically for certain mood-related conditions (e.g. seasonal patterns of low mood) — worth a single sentence acknowledging this exists, explicitly framed as general information rather than medical advice, with a light suggestion to speak to a health professional for anything beyond general lighting design. Keep this section tightly scoped to lighting design, not drift into health/therapy claims the site shouldn't be making.

6. **Human-centric lighting (HCL) / tunable white — how the design principle becomes an actual product**
   - Tunable white systems (adjustable CCT, typically ~2700K–6500K range) let a space follow a "dawn to dusk" curve automatically — cooler/brighter in the morning and midday, warming and dimming through the evening — rather than a single fixed CCT compromise
   - **Genuinely strong real-world example worth featuring:** a tunable lighting system installed in aged-care facility hallways has been shown to reduce resident sleep disturbances by around 50% compared to static lighting — a concrete, citable result rather than a vague wellness claim, and directly relevant if Solstice has any aged-care/healthcare-adjacent client base
   - Residential framing: premium/wellness-focused residential clients are an increasingly real market for tunable white systems — worth positioning this as an actual product conversation (tunable white downlights/drivers), not just theory
   - **Resolved — and worth writing into the article itself, not just noting here:** no specific job examples yet, but Chris is actively moving toward designing more with this in mind going forward. His honest read: the *technology* is still catching up, particularly on the control side for tunable white in a residential setting — worth including as a genuine, current-industry-state observation rather than presenting tunable white as a fully mature, plug-and-play residential option. This is a credible, non-hype-y note that fits the article's tone well: acknowledging where the industry actually is, not just where the theory says it should be.

7. **Practical design framework — the takeaway that ties it all together**
   - Not everyone needs (or can justify the cost of) a full tunable white system — the framework should scale down gracefully:
     - **Minimum viable version:** match fixed CCT to room *and* time-of-primary-use (Article A's defaults, applied with this deeper reasoning behind them)
     - **Better:** two-zone or scene-based control (a switch-dim or DALI scene for "evening mode" vs "daytime mode") in key rooms — bedrooms, living areas, home offices
     - **Full version:** genuine tunable white with an automated dawn-to-dusk curve, for clients who want to specify it properly
   - Cross-link back to Article A (CCT/CRI/beam angle) and Article B (dimming compatibility) — this section is where all three articles' content actually gets applied together

8. **Honest caveats section (important, given this touches health-adjacent territory)**
   - This is lighting design informed by circadian science, not medical advice — individual variability is real (chronotype, age, existing sleep conditions all matter), and none of this replaces a conversation with a health professional for an actual sleep or mood concern
   - The research base here is real and growing but not settled in every detail — present mechanisms and well-supported findings confidently, avoid overstating certainty on newer/single-study claims

**Natural internal links:** Article A (CCT/CRI/beam angle — the section this expands on), Article B (dimming compatibility — tunable/scene control ties in directly), any future bedroom-specific or aged-care-specific content if that becomes a topic

---

## Status

Resolved by Chris (2026-08-05):
- ✅ Section 3 (WELL benchmarks) — background/context only, no case study
- ✅ Section 6 (tunable white) — no job example yet; Chris's honest "tech/controls still maturing for resi" observation added directly into the article structure

**Still open, non-blocking:** final read-through of section 8's health-adjacent framing once drafted, to confirm tone lands as intended — not a hard blocker, just worth a look during/after build rather than before.
