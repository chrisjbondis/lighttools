# Interior/Spec Fundamentals Content Plan

**Date:** 2026-08-05
**Status:** ✅ READY FOR BUILD
**Feeds into:** `ADSENSE-CONTENT-HANDOFF.md`

---

## For Claude Code — start here

Build order — **4 articles** (Article D was scoped and then dropped, see its section below for why — don't build it):

1. **Article A** — Choosing the Right LED: CCT, CRI & Beam Angle Explained — ready. Includes a significant physiology/circadian section (melanopsin, ipRGCs, 1800K advanced callout, glare/flicker sensitivity) — this is the article's real differentiator, don't compress it down to a basic spec glossary.
2. **Article B** — Dimming Compatibility & Why LEDs Fail Early — ready, no blockers.
3. **Article C** — Cove & Under-Cabinet Lighting Done Right — ready. Features a real Solstice product (P24x9-REC-2000 mounting profile, linked) and Solstice's own CRI 95 strip range by name — treat both as genuine, accurate product mentions, not placeholder copy.
4. **Article E** — How to Read a Photometric Datasheet / IES File (Without Being a Lighting Designer) — ready, no blockers.

Each article should follow the site's existing template (TOC, callouts, comparison tables, "18-year industry professional" voice, per `ADSENSE-CONTENT-HANDOFF.md`) and slot into the Guides hub under the categories already defined in `guides-hub-content-plan.md`. Preview each before deploy per the standard handback process. "**[NEEDS CHRIS]**" markers throughout this doc are non-blocking open items (real job examples, specific product/brand confirmations) — build around them, don't wait on them.

---

## Grouping rationale

The original candidate list had 11 separate interior topics (CCT, CRI, beam angles, downlight spacing, dimming compatibility, cove lighting, under-cabinet lighting, why LEDs fail early, IES basics, emergency lighting, AS/NZS 1680). Rather than 11 thin articles, grouped into what became 4 build-ready ones (a 5th, emergency lighting + AS/NZS 1680, was scoped then dropped — see Article D below) — deeper, more useful pieces instead of a pile of near-duplicate "what is X" pages.

---

## Article A — Choosing the Right LED: CCT, CRI & Beam Angle Explained

**Angle:** These three numbers are on every spec sheet and every box, and most buyers either ignore them or get them backwards. This is the "how to actually read a spec sheet" article — practical, room-by-room, not a physics lecture.

**Structure:**

1. **CCT (colour temperature) — what the Kelvin number actually means**
   - 2700–3000K: warm, relaxed — living rooms, bedrooms; keeping bedrooms at 2700K or below supports the evening wind-down rather than fighting it
   - 3000–4000K: neutral — kitchens, bathrooms; clean and functional without reading as clinical
   - 3500–5000K+: cool/daylight — task-heavy areas, garages, offices
   - Important callout: CCT is not brightness — that's lumens, a completely separate number people conflate
   - **Chris's actual defaults:** living rooms/bedrooms — 3000K as the default, with the odd accent or uplight in 2700K for warmth where it suits. Kitchens/bathrooms — 3000K generally, but sometimes 4000K specifically for a mirror/makeup light, to give a decent colour balance against natural exterior light exposure at that spot. Task-heavy areas (garage, office) — mostly 4000K, though 3000K still gets used depending on the job.
2. **CRI — when it's worth paying for and when it isn't**
   - Scale to 100 (perfect, matches natural daylight); under 80 reads as poor, 90+ is the "great" tier
   - Where it matters: kitchens (food colour), bathrooms (skin tone at the mirror), wardrobes/dressing areas (matching clothes), retail/display, anywhere colour accuracy affects a decision
   - Where it doesn't matter much: garages, general circulation, storage — 80 CRI is fine, no need to pay the premium
   - **Chris's practical rule:** in a residential setting, sticks to CRI 90 as the minimum across the board — the reasoning being that incandescent (what people are used to and comparing everything against, even subconsciously) was effectively CRI 100. Strong, quotable framing for the article: CRI 90+ isn't a premium upsell, it's the baseline needed to not read as a downgrade from what people already know.
3. **Beam angle — the number that determines whether a downlight actually does its job**
   - Spot (~10–20°): accent/feature lighting, highlighting art or a single object
   - Narrow flood (~24–35°): kitchen benchtops, task areas needing concentrated light on a surface
   - Flood (~36–45°): general room downlighting, the most common residential choice
   - Wide flood (~46°+): large open areas, ambient fill
   - The mistake that gets made constantly: using a flood/wide-flood downlight over a kitchen island or benchtop and wondering why the task area still feels dim — beam angle chosen for the room type, not the actual task at that point
   - **Chris's actual defaults:** island bench/benchtop — 36–60°, but the bigger lever than the angle number itself is a highly recessed source for low glare (i.e., a well-recessed 60° fitting can outperform a poorly-recessed narrower one — worth making this the article's actual point rather than just publishing a beam-angle-by-room table). General living areas — 60°. Feature wall/accent — around 60° as well.
   - **[NEEDS CHRIS]** — still open: real "wrong beam angle" jobs fixed — Chris flagged "plenty, let's come back to that." Now has a strong home in section 5 below (see note there) rather than sitting as a standalone anecdote.
4. **Downlight spacing and layout** — natural tie-in to the Lux Calculator; spacing relative to beam angle and ceiling height, avoiding both dark patches and the "runway" over-downlit look
5. **Why this actually matters: light, physiology and how we function (significant expansion — Chris's steer)** — this is the section that lifts the article from "spec sheet glossary" to something genuinely differentiated. Chris's framing: the "wrong spec" jobs worth discussing aren't really about a fitting looking wrong — they're about specs that fight how the body actually responds to light. Structure:
   - **The eye does two jobs, not one:** rods and cones handle vision; a separate set of cells in the retina — intrinsically photosensitive retinal ganglion cells (ipRGCs), containing the photopigment **melanopsin** — don't contribute to what you consciously see at all. They feed directly into the suprachiasmatic nucleus, the brain's master clock, and drive non-image-forming responses: melatonin suppression, alertness, pupil response, circadian entrainment. Light isn't just something you see by — it's a direct physiological input, whether you're aware of it or not.
   - **Melanopsin's peak sensitivity is ~480nm — blue-cyan light.** This is why cooler, blue-rich CCT during the day supports alertness (mimicking daylight, which is genuinely rich in that wavelength), and why the same blue-rich content in the evening actively fights the body's wind-down by suppressing melatonin when it should be rising. This reframes the "warm at night, cool in the day" advice most people have heard as a rule of thumb into something with a specific, explainable mechanism.
   - **The advanced angle — 1800K and "extra-warm" night lighting:** worth a dedicated callout box, flagged clearly as an advanced/optional topic for the curious reader. Circadian-conscious lighting design increasingly uses a genuinely amber ~1800–2000K tier for evening/night use specifically because it minimises melanopic (blue-weighted) content, leaving melatonin production largely undisturbed — a step beyond just "go warmer at night," since 2700K is still blue-rich enough to have some suppressive effect. This is the kind of detail that signals real expertise rather than repackaged supplier copy — most competitor content stops at "use warm white in the evening" without explaining why or how far that logic actually goes.
   - **Glare and flicker sensitivity — individual variation matters:** ties directly into Article B's driver-quality argument. Flicker below ~120Hz is linked to headaches, eye strain and fatigue in sensitive individuals, and sensitivity varies significantly between people — migraine sufferers in particular show markedly higher rates of discomfort from flicker exposure than the general population. Worth stating plainly that "I can't see it flickering" doesn't mean a fitting/driver combination is actually flicker-free for everyone in the room, which is a genuinely useful, non-obvious point for someone choosing budget vs quality drivers.
   - **[NEEDS CHRIS]** — real "wrong spec" jobs now have a natural home here: e.g., cool-white specified through a bedroom fighting sleep, glare/flicker complaints traced back to a specific driver/fitting combo — still open, "come back to that," but now with a much stronger frame to plug the anecdotes into once ready
6. **Practical takeaway box** — a simple worked example: spec'ing a kitchen (CCT + CRI + beam angle by zone — general ceiling vs island vs open shelving), plus a second, shorter takeaway specifically on the physiology section: match CCT to time-of-use, not just room type, when it genuinely matters to the client (bedrooms, home offices with early/late hours)

**Natural internal links:** Lux Calculator, Article on dimming/driver mismatch (below) — flicker sensitivity content links directly to Article B's driver-quality argument

---

## Article B — Dimming Compatibility & Why LEDs Fail Early

**Angle:** Two problems that are actually the same problem — a mismatched driver. Flickering dimmers and premature LED failure both usually trace back to the same root cause: driver and control system weren't matched properly to begin with. Combining these means the article can build one coherent argument instead of two shallow ones.

**Structure:**

1. **The four dimming protocols, in plain terms:**
   - TRIAC (phase-cut): the cheap, common residential retrofit option — works, but has known flicker issues below ~20% brightness and needs a genuinely compatible driver, not just "any dimmer"
   - 0–10V: analog low-voltage control signal, common in commercial/retrofit; better flicker performance than TRIAC with a quality driver
   - DALI: bidirectional digital protocol built specifically for lighting — individually addressable, scene control, effectively flicker-free with the right driver, the professional standard for anything beyond basic residential
   - PWM: rapid on/off switching at high frequency — the mechanism many "flicker-free" claims actually rely on when done at a high enough frequency
   - The critical compatibility trap: a DALI controller won't dim a TRIAC driver, a 0–10V driver on a TRIAC wall dimmer will flicker or fail outright — protocol mismatch is one of the most common causes of "the dimmer doesn't work properly" callbacks
   - **Chris's actual practice:** phase-cut (TRIAC) is the default for standard resi jobs. Pushes toward DALI (or switch-dim) when the fittings themselves are professional-grade and specifically require it — i.e., it's often the fixture spec driving the protocol choice, not a general preference for DALI on "nicer" jobs. Worth framing the article around that logic rather than presenting DALI as simply "the upgrade tier."
   - **Chris's real-world observation:** has seen many jobs with flickering lighting, and it consistently traces back to the combination of decent-quality fittings and genuinely compatible dimmers — get that combination right and flicker is eliminated entirely; control systems like DALI or switch-dim solve it completely, but at a real cost premium, which is exactly why phase-cut remains the default rather than DALI-everywhere. Good honest framing for the article: DALI isn't just "nicer," it's a genuine fix for a real, common problem, but the cost has to be weighed against how much it actually matters for that job. Ties directly to Article A's flicker-sensitivity content — worth cross-linking explicitly both directions.
   - **[NEEDS CHRIS]** — still open: specific dimmer-compatibility callback stories — Chris flagged "quite a few, come back to that"
2. **Why LEDs (and drivers) actually fail early:**
   - Driver/LED mismatch — constant-current vs constant-voltage confusion is a real, common wiring-stage mistake that damages both driver and LED
   - Heat — every ~10°C rise roughly halves component lifespan; poor heat dissipation in cheap fittings (and poor installation practice — e.g., enclosing a fitting that needs airflow) accelerates this dramatically
   - Cheap components — electrolytic capacitors in low-grade drivers are a common weak point, degrading faster under heat and voltage stress than the LEDs themselves
   - Reframe: "the LED died" is very often actually "the driver died," and a driver failure is usually a heat or component-quality problem, not an LED problem
   - **Chris's installation practice (heat/ventilation):** reduces the number of recessed fittings in a ceiling where possible, and where recessed fittings are needed, favours ones that are sealed and/or rated to be safely covered by insulation — a genuinely practical, non-generic detail worth foregrounding since it's the kind of thing that prevents the heat-related failure this whole article is about, rather than just describing the failure after the fact.
   - **[NEEDS CHRIS]** — still open: real premature-failure jobs diagnosed, and specific driver brands/grades trusted
3. **Practical takeaway box** — a simple diagnostic flow: dimmer flickering or LED failing early? Check protocol match first, then driver quality/heat, before assuming the LED itself is faulty

**Natural internal links:** Article A (CCT/CRI/beam angle), Article 2 from the exterior batch (fitting construction — heat/component quality is the same underlying theme)

---

## Article C — Cove & Under-Cabinet Lighting Done Right

**Angle:** Linear/strip lighting done well disappears into the architecture; done badly, it's visible hot spots, colour-shift along the run, or a strip that's died in two years because it was buried in a cabinet with no airflow. This is the "the details that separate a clean result from an amateur one" article.

**Structure:**

1. **Cove lighting** — concealment technique (recess depth vs strip position to hide the light source while getting clean, even wash), colour consistency along a run (binning/batch matching so you don't get visible tone shift across a long cove), and why continuous runs need attention to voltage drop over distance (natural tie-in to the Voltage Drop Calculator)
   - **Chris's approach:** genuinely job-by-job rather than a fixed spec — the constants are high quality and high efficacy strip, whatever the specific IP/density numbers end up being for that job. Worth framing the article around "what to prioritise" (quality, efficacy, colour consistency) rather than a single fixed spec table, since that's how it's actually approached in practice.
2. **Under-cabinet lighting** — task-focused, so CCT/CRI selection matters more here than almost anywhere else in the home (ties back to Article A); mounting position to avoid glare off benchtops; heat management in an enclosed cabinet void — a strip that runs hot in a sealed space is a slow-motion failure
   - **Chris's approach:** same quality/efficacy priority as cove, but Solstice has a specific mounting profile that almost completely conceals the light source — the **P24x9-REC-2000 slot-recess aluminium mounting profile** (21x9x2000mm): https://www.solsticelighting.com.au/shop/led-strip-mounting-profiles-6/p24x9-rec-2000-profile-slot-recess-aluminium-mounting-profile-21x9x2000mm-11 — genuinely worth featuring in the article as a real, specific example of "concealment done properly," and a natural soft product mention since it's Chris's own product, not a generic supplier plug
3. **Trusted brand for colour consistency:** Solstice's own strip range — CRI 95, described as very high quality — worth naming directly in the article as the standard Chris actually specifies, not just a generic "look for high CRI" line
4. **Chris's real-world observation — the "dotty strip" problem:** has seen plenty of channels where the strip looks visibly dotty/uneven rather than a smooth continuous line — this comes down to LED density (not enough chips per metre for the application) and, more fundamentally, SMD strip (individually spaced LED chips soldered to a PCB, which inherently produces visible dots and glare) vs **COB strip** (chip-on-board — densely packed chips that behave as one continuous, glare-free light source with no visible dots). Also flagged chip failures as very common on cheap strips, for a number of reasons — worth its own short section on why budget strip fails at the individual-chip level (poor binning, inadequate heat dissipation, weak solder/substrate quality), distinct from the driver-failure content already covered in Article B. This is a strong, concrete "why the cheap option looks bad and dies early" section that most competitor content doesn't explain properly — worth making it a headline point of the article rather than a passing mention.
   - **[NEEDS CHRIS]** — still open: specific mistakes fixed on real jobs — Chris flagged "come back to that"; also worth asking whether Solstice's own strip range (already named above for CRI/colour consistency) is COB or high-density SMD, so the article can speak to it accurately
5. **Practical takeaway box** — a short spec checklist for a clean cove/under-cabinet result

**Natural internal links:** Voltage Drop Calculator, Article A (CCT/CRI), Article B (driver/heat)

---

## Article D — DROPPED (2026-08-05)

Emergency lighting (AS 2293) confirmed not relevant to Solstice's client base. Chris opted to drop this article from the batch entirely for now rather than fold or rescope it — AS/NZS 1680 content can be revisited later as its own thing if a good angle comes up, but it's not being forced into this batch just to hit a count. Interior batch is now 4 articles (A, B, C, E).

---

## Article E — How to Read a Photometric Datasheet / IES File (Without Being a Lighting Designer)

**Angle:** A genuinely differentiated, slightly technical piece — most competitor content either skips this entirely or is written for specifiers already using AGi32. This version is for the curious buyer or small business owner who's been handed a spec sheet and wants to actually understand it.

**Structure:**

1. **What an IES file actually is** — a standardised (ANSI/IES LM-63) text file describing how a specific fixture distributes light in 3D space: intensity at various angles, total lumens, fixture dimensions
2. **What it can tell you** — luminous flux, distribution pattern (is this a tight spot or a broad wash?), and when loaded into a photometric viewer, a visual read of the beam shape
3. **What it can't tell you** — a critical, honest section: an IES file says nothing about electrical listing, surge protection, driver quality, corrosion resistance, warranty, colour consistency, or suitability for a wet/hot/dusty location. A fixture can have a beautiful IES file and still be a poor-quality product — this is the point that separates this article from generic "what is an IES file" content
4. **Practical use for a non-specifier** — free viewer tools worth knowing about, and the realistic takeaway: understanding roughly what you're looking at is useful, but a proper layout calculation is still a job for someone using the file properly against real room geometry — not a DIY replacement for that
5. **Chris's actual practice:** does sometimes use DIALux for a quote, but it's rare — worth reflecting that honestly in the article rather than overstating how central photometric layout work is to a typical resi/small-commercial job; reinforces the "understand it, but it's not a DIY replacement for the real thing" framing already planned for this section.
   - **[NEEDS CHRIS]** — still open: a real (anonymised) example worth featuring to show a DIALux/IES file "in action"

**Natural internal links:** Lux Calculator (the DIY version of what a proper photometric layout does at a much simpler level)

---

## Open items for Chris

**Resolved (2026-08-05):**
- ~~Article A: default CCT by room~~ — done
- ~~Article A: default beam angle by application~~ — done (and reframed: recess quality for glare control matters more than the angle number alone)
- ~~Article A: CRI framing~~ — done: CRI 90 minimum in resi, benchmarked against incandescent's effective CRI 100
- ~~Article B: default dimming protocol~~ — done: phase-cut default, DALI/switch-dim when the fitting itself requires it
- ~~Article B: heat/ventilation installation practice~~ — done: minimise recessed fitting count, use sealed/insulation-rated fittings
- ~~Article C: strip specs and philosophy~~ — done: job-by-job, prioritising quality/efficacy over a fixed spec
- ~~Article C: trusted product for concealment~~ — done: Solstice's own P24x9-REC-2000 mounting profile, with product link
- ~~Article C: trusted brand for colour consistency~~ — done: Solstice's own CRI 95 strip range
- ~~Article D: emergency lighting relevance~~ — done: **not relevant** — Article D dropped from the batch entirely (2026-08-05), not rescoped
- ~~Article E: does Chris use IES/photometric layouts~~ — done: occasionally DIALux, rare

**Resolved (2026-08-05, round 2):**
- ~~Article A: physiology/circadian angle~~ — done: significant new section added — melanopsin/ipRGCs, non-image-forming light response, 1800K "extra-warm" advanced callout, glare/flicker sensitivity (individual variation, migraine link)
- ~~Article B: real flicker observation~~ — done: flickering jobs consistently trace to fitting+dimmer quality/compatibility; DALI/switch-dim eliminates it but at a real cost premium
- ~~Article C: dotty strip problem~~ — done: LED density + SMD (visible dots/glare) vs COB (continuous, glare-free) explained; chip failure on cheap strips flagged as a distinct, common issue

**Still open:**
- Article A: real "wrong spec" jobs (bad CCT/beam angle) — flagged "plenty, let's come back to that"; now has a natural home in the new physiology section
- Article B: specific dimmer-compatibility callback stories — flagged "quite a few, come back to that"
- Article B: real premature-failure diagnoses, specific driver brands/grades trusted
- Article C: specific mistakes fixed on real jobs — flagged "come back to that"
- Article C: is Solstice's own strip range COB or high-density SMD (needed to speak to it accurately in the dotty-strip section)
- Article E: a real anonymised DIALux/IES example to feature

## Summary

- 4 new articles from the 11 original interior candidate topics (grouped for depth over quantity; Article D dropped — emergency lighting not relevant to Solstice's client base, AS/NZS 1680 not forced into the batch on its own)
- Combined with the exterior batch (6 articles + 1 tool), this puts the site at 3 existing + 10 new = 13 articles once built, plus the exterior backlog (4 more) and the tool — still comfortably toward the 15+ AdSense re-review target once the backlog gets picked up
