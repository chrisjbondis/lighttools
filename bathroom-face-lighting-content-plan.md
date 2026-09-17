# How to Light a Face Well in a Bathroom — Content Plan

**Date:** 2026-08-05
**Status:** ✅ READY FOR BUILD
**Feeds into:** `ADSENSE-CONTENT-HANDOFF.md`

---

## For Claude Code — start here

Build order:

1. **Article** — "How to Light a Face Well in a Bathroom (Not Just the Room)" — build per the structure below. This is a differentiated, expertise-led piece (not a stock listicle) — keep the physics explanations (vertical vs horizontal illuminance, the law of reflection for the bounce technique) intact rather than simplifying them away.
2. **Diagrams** — 3 concepts prototyped and approved (narrow vs wide mirror layout, diffuse vs clear glass shadow comparison, bounce technique under a low ceiling); a working SVG prototype is saved at `bathroom-face-lighting-diagrams.svg` in the outputs folder as a visual/logic reference — treat the prototype's logic as correct, refine visual execution to match the site's existing diagram style during build. A 4th diagram (very-wide/double-vanity band) is optional, not blocking.
3. **Companion tool — Bathroom Lighting Selector (v1, guided configurator only)**: inputs are mirror width, mirror-top height, ceiling height, and whether the mirror is a projecting cabinet (yes/no + rough depth). Output is a recommended approach (flanking sconces / central-spanning fixture / bounce technique) plus a generated diagram of that specific layout. This is a rules engine + parametric diagram, same complexity class as the existing Fitting Selector — **do not build the full physics-based light simulation** (beam falloff, rendered heatmap) as part of this batch; that's explicitly parked as a separate future project.
4. Slot the finished article into the Guides hub under the appropriate category (Lighting Fundamentals, per `guides-hub-content-plan.md`'s structure) and add it to the sitemap per the standard pre-deploy checklist.

The AS/NZS 3000 bathroom zone figures in section 6 were researched properly but trade sources disagreed with each other — present them as general guidance with a "confirm with a licensed electrician" caveat, not as unqualified fact, consistent with how the RCD article handled compliance content.

---

## Why this one's good

This is a genuinely differentiated topic — most competitor content is "5 bathroom lighting ideas" listicles with stock photos. What Chris described is an actual design methodology: direct light vs reflected/bounce light, why mirror width dictates fitting count and position, why glass/diffuser material determines whether you get shadows, and what to do when ceiling height and cabinet height fight each other. That's real expertise, not decoration advice. Research confirms the underlying principle: standard downlights are engineered to project a downward cone onto horizontal work surfaces, and that geometry fundamentally fails when the "surface" being lit is a vertical one — a face looking into a mirror. Most lighting guides don't explain *why* face lighting is a different problem to room lighting; this article can.

---

## Article structure

**Working title:** How to Light a Face Well in a Bathroom (Not Just the Room)

1. **The core problem: lighting a face is a different job to lighting a room**
   - Most bathroom downlights are designed to throw light down onto horizontal surfaces (floor, benchtop) — that geometry doesn't work on a vertical target (a face at a mirror), which is why a bathroom can measure "bright enough" overall and still leave someone looking washed out or shadowed at the mirror
   - Two separate concepts worth naming explicitly: **horizontal illuminance** (general room brightness) vs **vertical illuminance** (light actually landing on the face) — a bathroom frequently has plenty of the first and not enough of the second
   - **Direct light vs reflected/bounce light** — the two tools available, and why understanding which one a given fitting is providing is the actual design skill here

2. **Mirror width determines the whole approach — three bands (confirmed with Chris)**
   - **Narrow (~1000mm or under):** two sconces, one each side, genuinely cover the full face width — the classic "flanking" approach, and it works specifically because the mirror is narrow enough that the two light paths overlap in the middle rather than leaving a dark zone
   - **Mid/wide (~1000mm–3000mm):** two edge fittings alone won't reach the centre of the face — light falls off before it crosses to the opposite side. Needs a light positioned centrally (top or side-spanning), a run of tiltable/gimballed downlights across the width, a surface-mounted fitting, or a diffused pendant positioned behind the user's eyeline
   - **Very wide / double-vanity (~3000mm+):** a single central fixture is no longer enough to span the distance either — this band needs multiple central/spanning fixtures or a continuous linear light source (echoes the cove/under-cabinet linear-lighting logic from the interior spec-fundamentals batch — same "continuous run, not a single point" principle, applied here to a double-vanity mirror)
   - **Note:** if Chris's "3000mm" steer was aimed at a different cutover than a third band above the existing wide category, flag it on review — drafted here as the natural double-vanity extension of the existing 1000mm/1500mm reference points from the original brief

3. **Why glass/diffuser material makes or breaks a side sconce**
   - A wall light either side of the mirror must be genuinely bright enough *and* use white/opal glass — a diffuse, even light-emitting surface — rather than clear glass, clear ribbed glass, or an exposed globe
   - The mechanism (confirmed by research): a diffuser with an opal/frosted surface presents one large, uniform luminous area rather than a small bright point, which is what actually eliminates shadow — a clear-glass or exposed-globe fitting is still a point source no matter how bright it is, and point sources cast hard shadows across the face (under the brow, beside the nose) exactly where you don't want them
   - This is a good "why the cheap option looks wrong" section, similar in spirit to the strip-lighting dotty/SMD-vs-COB point in the interior spec-fundamentals batch — same underlying idea (point source vs. diffuse source), different application

4. **Mirror height and ceiling height change the whole equation**
   - **High mirror top (≥2400mm):** a light mounted above needs to be genuinely bright and aimed down deliberately, or it will simply miss the face when someone leans in close (e.g. for detailed grooming) — at this height, side lighting (if the mirror is narrow enough) or a pendant/surface-mount/downlight positioned so the light source stays visible when leaning in becomes the more reliable option
   - **Low ceiling + mirrored cabinet (a very common real-world setup):** e.g. 2400mm ceiling, cabinet mirror top around 2100mm. Cabinets that project off the wall add a further complication worth its own callout — the projection depth changes the geometry again, since it changes both the mounting point available and what gets shadowed
   - **The bounce/incidence technique — explained via the physics, not a case study (Chris's steer: use physics rather than a specific job anecdote):** the law of reflection — angle of incidence equals angle of reflection, both measured from the perpendicular to the mirror surface — is the whole mechanism here, and it's worth actually explaining in the article rather than just asserting "bounce the light." A fitting mounted directly above the mirror sends light straight down at roughly 0° incidence, which reflects straight back up — it never reaches a face standing in front of the mirror at all, it just illuminates the ceiling via the mirror. Setting the fitting back and angling it toward the mirror creates a real incidence angle, so the reflected ray travels forward and down onto the face instead. This is genuinely why "positioned a little behind, angled toward the mirror" works and a straight-down fitting doesn't — the geometry, not a trick. An oyster, wide-angle downlight, or gimballed/tilted downlight are all just different ways of creating that angled source.
   - Worth pairing with a simple diagram (see below) showing the reflection geometry — an oyster/gimbal is one of the diagrams already prototyped

5. **Magnifying mirrors with integrated lighting**
   - Purpose-built for exactly the close-up task (plucking, detailed grooming) that overhead/side lighting alone often can't serve well at high mirror-top heights — worth a short, honest section: this isn't a replacement for good general mirror lighting, it's a targeted tool for a specific task

6. **Compliance callout — bathroom IP zones (AS/NZS 3000)** *(new addition — not in Chris's original brief, but directly relevant and currently uncovered by any existing article)*
   - **Researched properly per Chris's request (2026-08-05) rather than left as a first-pass figure.** Trade sources are notably inconsistent on the exact numbers — several disagree on whether Zone 0 is IP67 or IPX7, whether Zone 1 is IP44 or IPX4, and whether a bathroom has 3 zones or 4 (some sources define a further Zone 3). This inconsistency across supposedly authoritative trade sites is itself worth knowing before publishing anything as settled fact.
   - **Most consistent picture across sources:**
     - **Zone 0** — interior of the bath or shower base: only SELV (extra-low voltage, ~12V) equipment permitted, minimum **IPX7** (protected against temporary immersion)
     - **Zone 1** — directly above the bath/shower enclosure, up to ~2.25m high: minimum **IPX4** (commonly quoted in trade contexts as "IP44," which folds in a dust rating IPX4 alone doesn't specify — worth using IPX4 as the precise figure and noting IP44 as the practical equivalent tradespeople commonly reference)
     - **Zone 2** — extends ~600mm horizontally beyond Zone 1, up to ~2.25m high, plus a ~150mm radius around basins extending ~400mm above them (this is the zone mirror/vanity lighting actually sits in): minimum **IPX4**
     - Some sources also define a **Zone 3**, beyond Zone 2, with no special IP requirement — not universally referenced, so worth treating as secondary/optional detail rather than a headline figure
   - **Given the genuine inconsistency found in research, this section should be framed carefully:** present the zones and figures above as general guidance, and be explicit that exact clearances and ratings should be confirmed against the current AS/NZS 3000 edition (or with a licensed electrician) for any real installation — same cautious framing already used successfully in the exterior batch's RCD article, not a case of the article claiming false precision
   - **[NEEDS CHRIS]** — still worth a final human sanity-check against what he applies on real jobs before this goes live, given the source disagreement uncovered — but the research legwork is now done rather than resting on a single first-pass search

7. **Cross-references worth building in:**
   - CCT/CRI content from Article A (interior batch) — a mirror light is one of the clearest real-world cases where CRI genuinely matters (skin tone accuracy), and CCT choice (Chris's own 4000K-for-mirror-lights note from Article A) ties in directly
   - Dimming/flicker content from Article B — flicker sensitivity is especially noticeable at close range in a mirror
   - IP rating concepts already established in the exterior/water-contact articles — same underlying idea (rating matched to real exposure), different environment

8. **Practical takeaway box** — a simple decision flow: measure mirror width → check ceiling/mirror-top height → pick direct (flanking sconces) or bounce (oyster/gimbal) approach accordingly → confirm IP zone compliance → confirm diffuser material if using any wall-mounted fitting

---

## Diagrams

Chris flagged wanting visuals for this one — the wide-mirror-vs-narrow-mirror layouts, the bounce/incidence technique, and the diffuse-vs-clear-glass shadow comparison are all things that are much clearer shown than described. A first-pass prototype of three diagrams was drafted and shared (2026-08-05) covering: (1) narrow vs wide mirror fitting placement, (2) diffuse vs clear glass shadow comparison, (3) the bounce/incidence technique for a high mirror under a low ceiling. **Direction confirmed by Chris as good** — visual polish to happen once the article itself is actually being built, not before. Claude Code should treat the prototype logic as correct and refine the visual execution during build, rather than needing a further round of concept sign-off.

---

## Companion tool — Bathroom Lighting Selector (v1 scope, guided configurator)

**Decision (2026-08-05):** build a guided selector now, matching the Fitting Selector's complexity class — not the full physics-based simulation Chris originally floated. That's explicitly parked as a separate, later project (see below) rather than blocking this one.

**Concept:** user enters mirror width, mirror-top height, ceiling height, and whether the mirror is a projecting cabinet (yes/no + rough depth) → tool applies the rules from the article and recommends an approach (flanking sconces vs central/top light vs bounce technique via oyster/gimbal) → generates a simple diagram of the recommended layout, in the same visual style as the article's diagrams, personalised to the user's actual numbers rather than a generic illustration.

**Core logic:** essentially the decision flow already laid out in the article's practical takeaway box (section 8), turned into an interactive form — mirror width threshold → height/ceiling check → bounce-technique trigger if mirror-top is high and ceiling is low → IP zone reminder for whatever's recommended. No physics simulation, no rendering engine — a rules engine plus a parametrically-generated diagram, which is squarely in the same build complexity as the existing Fitting Selector.

**Status:** mirror-width bands now defined (three tiers, see article section 2) — tool logic can be built against these. Worth Chris double-checking the bands read correctly against his "3000mm" steer during review, but not a hard blocker.

### Parked for later — full light simulation (v2, separate project)

The "adjust every fitting and see a rendered light pattern" version Chris originally described is a genuinely different scale of build — a real physics engine (beam falloff, diffuse reflection off the mirror, a rendered illuminance heatmap), not a lookup/rules tool. Worth scoping as its own dedicated project once the guided selector is live and the article's out, rather than folding it into this batch. Flagging now so it doesn't get lost, not committing to a build approach yet.

---

## Open items for Chris

Chris signed off "good enough for now" (2026-08-05) — remaining items below are non-blocking, build around them:

- Quick read-through of the three mirror-width bands (section 2) to confirm they match his "3000mm" steer as intended
- Final sanity-check of the AS/NZS 3000 zone figures against real job experience — research is done and sources reconciled, but worth a last human check given how inconsistent the trade sources turned out to be
- Diagram set still only covers 3 of the article's concepts (narrow/wide/bounce) — worth a 4th prototype for the very-wide/double-vanity band once that section is confirmed

## Resolved (2026-08-05)

- ✅ Diagram direction — confirmed good, refine visual polish during build rather than now
- ✅ Tool scope — guided selector (v1) now, full physics simulation parked as a separate later project
- ✅ Mirror-width threshold — three-band structure defined (narrow ≤1000mm, mid/wide 1000–3000mm, very wide/double-vanity 3000mm+)
- ✅ Bounce technique — now explained via the actual physics (law of reflection) rather than needing a job anecdote
- ✅ AS/NZS 3000 bathroom zones — properly researched; figures reconciled across sources with inconsistency flagged, framed as general guidance rather than false-precision fact
