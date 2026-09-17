# Exterior/Garden Lighting Content Plan

**Date:** 2026-07-31
**Status:** ✅ READY FOR BUILD
**Feeds into:** `ADSENSE-CONTENT-HANDOFF.md`

---

## For Claude Code — start here

This doc is ready to build against. Build order and scope:

1. **Article 1** — How Far Does Outdoor Light Really Travel? (lumens/lux/glare) — ready, no blockers
2. **Article 2** — Why Fitting Construction Matters (materials/coatings/IP) — ready, no blockers
3. **Article 3** — In-Ground Fittings: Water Ingress & IP68 Joins — ready. **One constraint: do not name "Aqualux" or make specific product claims about an anti-siphon connector** — describe the connector category generically only (see the article's structure section for the exact approved wording). Chris will supply the confirmed product detail later for an update.
4. **Article 4** — Decorative & Accent Lighting (festoon/fairy/RGBW/tree lighting) — ready, no blockers
5. **Article 5** — Do You Need an RCD for Outdoor Lighting in Australia? — ready. Built from research, not yet spot-checked by Chris; flag as "please confirm framing reads right" in the build preview rather than treating as final.
6. **Article 6** — Fittings That Live in Water — ready, no blockers
7. **Fitting Selector tool** — build to **v1 scope only** (see tool section below): postcode-based coastal-zone lookup with the material table as given, plus a yes/no "is this going in water?" toggle that returns a guidance message + Solstice contact CTA + Aqualux/Hunza brand mention (not a full material recommendation). The full water-type material logic table is an explicit v2, out of scope for this build.

Each article should follow the site's existing template (TOC, callouts, comparison tables, "18-year industry professional" voice, per `ADSENSE-CONTENT-HANDOFF.md`). Preview each before deploy per the standard handback process. "**[NEEDS CHRIS]**" markers throughout this doc are non-blocking open items — build around them, don't wait on them.

---

## Article 1 — How Far Does Outdoor Light Really Travel? (Lumens, Lux, Glare & Light Trespass)

**Angle:** Most people size outdoor lighting the same way they'd size a room — wrong. Outdoor light behaves completely differently: it falls off fast (inverse square law), needs far fewer lumens than people assume, and the real failure mode isn't "too dim," it's glare and light spilling where it shouldn't.

**Structure (matches existing article template — TOC, callouts, tables, worked examples):**

1. **Why outdoor ≠ indoor lighting** — the core misconception people bring from indoor lighting shopping
2. **The inverse square law in plain terms** — light intensity drops with the square of distance; double the distance, quarter the light. Worked example with a real fitting (e.g., a common 12V garden spike light).
3. **How little light you actually need outdoors** — table comparing AS/NZS 1158.3.1 pathway categories:
   - PP1: 10 lux, PP2: 7 lux, PP3: 3 lux, PP4: 1.5 lux, PP5: 0.85 lux
   - Contrast against indoor: living areas 100–300 lux, task/reading 300–500+ lux
   - The "why" — eyes dark-adapt outdoors; over-lighting kills that adaptation and creates hot spots/shadows that feel *less* safe, not more
4. **Glare — the real enemy** — unshielded fittings, low mounting height, direct line of sight to the LED chip. Glare vs illuminance: a path can be technically "compliant" and still be unusable if the fitting isn't shielded properly
5. **Light trespass and obtrusive lighting** — AS/NZS 4282:2023 governs spill onto neighbouring properties, sky glow, and glare as assessed at property boundaries/building façades; increasingly used by councils in planning approvals. Practical takeaway: aim/shield fittings, don't just add more of them
6. **Real numbers/rules of thumb (Chris's actual specs)** — typical lumen output by fixture type:
   - Path lights: 3W
   - Step lights: 1–2W
   - Tree uplights: 3–6W
   - Façade wash: 6W
   - Driveways: 6W
   - **[NEEDS CHRIS]** — still open: common mistakes/real jobs where over-lighting caused problems (glare complaints, blown-out driveways, etc.)
7. **Practical takeaway box** — how to actually plan an outdoor lighting layout without guessing

**Natural internal links:** Garden Lighting Calculator, Lux Calculator, new Fitting Selector (below)

---

## Article 2 — Why Fitting Construction Matters for Exterior Lighting (Materials, Coatings, IP Ratings)

**Angle:** Two fittings can look identical and carry the same IP rating on the box, yet one lasts 15 years outdoors and the other corrodes and fails in 18 months. IP rating alone doesn't tell you if a fitting will survive where it's actually installed — construction and material grade do.

**Structure:**

1. **IP ratings explain water/dust ingress, not corrosion resistance** — common misconception; a fitting can be IP65 and still corrode fast in a coastal environment because IP has nothing to do with material chemistry
2. **What actually determines fitting lifespan outdoors:**
   - Base material — die-cast aluminium (most common, quality varies hugely) vs marine-grade stainless steel (316) vs standard 304 stainless vs polymer/composite housings vs solid brass/bronze/copper (traditional marine/architectural choice — doesn't corrode structurally, develops a protective patina instead; used a lot in high-end coastal and landscape fittings)
   - Coating/finish — powder coat quality and pre-treatment (chromate conversion, e-coat priming before powder coat), anodising for aluminium, and why cheap powder coat over untreated die-cast fails first at the fixing points and cut edges
   - Seals and gaskets — UV-stable silicone vs cheap rubber that perishes and cracks in a couple of Australian summers
   - Stainless fixings/screws — a fitting can have a good body and still fail early because the screws are mild steel and rust, staining and weakening the fixing
3. **Atmospheric corrosivity zones (AS/NZS 2312 / AS 4312)** — table:
   - CX (Extreme): within ~200 m of surf beaches/rough seas
   - C4/C5 (High/Very High): sheltered bays, up to ~50 m inland, and coastal strip generally
   - C3 (Medium): roughly 100 m to a few km inland
   - C2 (Low): can extend to ~1 km from sheltered water
   - C1 (Very Low): most of Australia, 50 km+ from the sea
   - Practical translation: what grade of fitting to specify for each zone
4. **Real field examples (Chris's experience)** — die-cast aluminium fittings are the recurring failure: rusty, pitted, and cheap powder coat fading fast in coastal exposure. What he specifies instead now: low-maintenance materials — copper, brass, bronze, anodised finishes, and proper coastal-rated powder coat systems.
   - **[NEEDS CHRIS]** — still open: which specific ranges are genuinely marine-rated vs just marketed as "coastal" without the material to back it up (a good "buyer beware" section if he's got examples)
5. **Practical takeaway box** — a simple decision path: know your distance from the coast → know your minimum material/coating spec → check IP rating for the specific application (in-ground vs wall-mounted vs submerged)

**Natural internal link:** New Fitting Selector tool (below) — this article is the "why," the tool is the "what do I actually need"

---

## Article 3 — In-Ground Fittings: Water Ingress, Cable Entry & How to Do a Proper IP68 Join

**Angle:** An in-ground fitting's IP68 rating describes the sealed housing tested in a lab — it says nothing about the join where the cable leaves the fitting or the connections buried further down the run. Most real-world in-ground failures aren't the fitting body letting go; they're water travelling in along/inside the cable jacket and finding the join. This is the detail that separates a fitting that lasts 15 years buried in a lawn from one that fails in 18 months.

**Structure:**

1. **Two routes water takes into an in-ground fitting** — worth stating explicitly since most buyers only think about the first:
   - Route A: through the housing seal/lens gasket (what the IP68 lab test actually measures)
   - Route B: down/along the cable — water runs down the cable jacket to the entry point, or wicks along the stranded conductor itself via capillary action between strands, bypassing a perfectly good housing seal entirely
2. **Why Route B is the one that actually kills fittings in the field** — a fitting can be IP68 out of the box and still fail within a season if the cable entry isn't managed properly, because the failure path never goes through the tested seal at all
3. **How manufacturers try to solve this** —
   - Gel-filled or resin-potted cable entries that fully encapsulate the conductor at the entry point, stopping capillary wicking
   - Double-sealed cable glands with a compression seal on the jacket
   - Pre-terminated quick-connect systems designed so the field join happens in a purpose-built connector rather than a raw twist-and-tape or wire-nut joint
   - **Anti-siphon connector systems (kept generic — do not name Aqualux):** worth a line noting that some manufacturers now build anti-siphon connectors specifically designed to stop water travelling up the cable into the fitting, rather than relying on the housing seal alone. Chris has one specific product in mind but hasn't had the exact mechanism confirmed by the supplier yet, so the article should describe the category/concept rather than name or claim specifics about any one product until that's verified. Can be named and detailed in a later update once confirmed.
4. **How a contractor should actually do an IP68 join in the field** — the practical section, worth building out as a numbered how-to box:
   - Strip cable cleanly — no nicked strands (a nicked strand is a wicking path)
   - Use a genuinely gel-filled or resin-filled IP68 connector rated for direct burial — not a housing that's IP68 dry but relies on grease that can be displaced
   - Where possible, terminate in an accessible valve box rather than a bare direct-buried joint — makes future fault-finding possible without digging up the lawn
   - Form a drip loop in the cable before it enters the fitting/gland, so water runs off the low point instead of straight into the entry
   - Don't mix dissimilar metals at the join (galvanic corrosion between conductor, lug and terminal accelerates failure, especially relevant in the coastal zones covered in Article 2)
   - Correct crimp/torque on the connection — a loose crimp leaves a gap for water to wick into before it ever reaches the "sealed" part of the connector
   - Insulation-resistance test the circuit before backfilling — cheap to check now, expensive to dig up later
   - **Real examples (Chris's experience):** this is a very common failure — he's seen "tons" of fittings with water having travelled up the cable and into the housing, confirming Route B is a routine, not rare, field problem. Good real-world framing for the article's opening — this isn't a theoretical edge case, it's one of the most common in-ground lighting failures he sees.
5. **External resource** — link to a genuine, verified how-to video on making a proper IP68 direct-bury join. **[NEEDS CHRIS]** — none yet; still open, still don't want to fabricate a link
6. **Practical takeaway box** — tie back to Article 2's material/coating guidance: right material + right coating means nothing if the cable join fails first

**Natural internal links:** Article 2 (fitting construction), Fitting Selector tool

---

## Article 4 — Decorative & Accent Lighting: Festoon, Fairy Lights, Tree Lighting & Colour-Changing Systems

**Angle:** This is the "make it beautiful" article, sitting alongside the more technical pieces — covers the decorative side people actually search for (festoon for entertaining areas, fairy lights, uplighting a feature tree) without dropping the same standard of real detail (spacing numbers, mounting method, what actually looks cheap vs premium).

**Structure:**

1. **Festoon lighting**
   - Bulb/globe spacing: ~30–50 cm is the common warm, even-glow spacing; wider spacing (~60 cm+) gives a more minimal look but needs careful run planning to avoid dark patches
   - Catenary/tension wire: for spans over ~8 m, or any exposed/windy site, run a galvanised steel support wire rather than relying on the festoon cable itself to carry the load — this is a common corner cut that ages badly
   - Leave sag — roughly a 1:50 sag-to-span ratio — to absorb thermal expansion and wind movement; pulling it drum-tight looks neat on install day and fails at the fixings within a season
   - Mounting height: minimum ~2.1–2.4 m clearance over anywhere people walk
   - IP rating: IP44 minimum for covered/sheltered outdoor areas in Australia, IP65 preferred for anything fully exposed to rain — and the connection points/joiners are the weak link, not the cable run, so they need the same or better rating
   - **Real spacing (Chris's practice):** normally 50 cm–100 cm depending on space size and mounting height — wider range than the generic guide figure above, worth using his real number as the primary guidance rather than the generic one
   - **[NEEDS CHRIS]** — still open: any festoon jobs that failed early (usually at the joiners or fixings) worth using as a cautionary example
2. **Fairy lights**
   - Same IP-rating logic as festoon — IP44 minimum, IP65 near pools/spas or fully exposed
   - Low-voltage systems are the standard/required approach near pools, spas and other wet areas
   - Connection points are the most vulnerable part — same lesson as Article 3's in-ground cable-join content, worth cross-linking rather than repeating
3. **Colour-changing / tunable systems — RGB vs RGBW vs RGBCCT**
   - RGB: 3-channel (red/green/blue), cheapest, but "white" is a mix of the three colours and reads slightly blue/muddy rather than a clean white
   - RGBW: 4-channel — adds a dedicated white diode alongside RGB, giving a genuinely clean white in addition to colour — better choice if the fitting needs to do both "everyday warm white" and "party mode colour" well
   - RGBCCT: 5-channel — adds tunable white (warm-to-cool) on top of RGB, the most flexible and usually the most expensive
   - Control protocols in plain terms: DMX for large-scale, precisely synced commercial/architectural jobs; Zigbee/Wi-Fi/Bluetooth mesh for residential smart control via an app — worth a line of caution about proprietary apps/ecosystem lock-in when specifying a smart system for a client
   - **Chris's honest take:** genuinely subjective, and the real risk is overdoing it — RGBW/RGBCCT needs to be classy, not overdone, especially in a residential setting. This is a strong, quotable framing for the article: colour-changing done well is restrained, not a light show.
4. **Tree lighting — uplighting vs moonlighting**
   - Uplighting: ground-mounted fixtures roughly 1–6 ft (0.3–1.8 m) from the trunk depending on tree size, aimed upward at 30–45° into the canopy — dramatic, good for feature/specimen trees
   - Moonlighting: fixtures mounted high in the canopy aimed downward, mimicking moonlight through branches — soft, dappled shadow on the ground below, especially effective over patios, seating areas and paths; less "look at this tree," more ambient mood
   - Tree health/mounting note (a genuinely differentiating professional detail): use non-invasive strap-mount brackets rather than screwing or nailing into the trunk/branches — drilling or nailing creates entry points for disease and pests that damage the tree over the long term. Worth flagging plainly since a lot of DIY guides skip it entirely
   - **Fixture wattage/beam angle (Chris's practice):** genuinely depends on the job — no fixed formula, it's assessed per tree based on canopy size, height, and desired effect. Worth stating that directly in the article rather than forcing a false-precision table — it's itself a useful professional insight (contrast against generic guides that quote fixed numbers regardless of the actual tree)

**Natural internal links:** Garden Lighting Calculator, Article 1 (lumens/glare — ties directly into "how bright should the uplight be"), Article 3 (cable joins — for the festoon/fairy connection-point content)

---

## Article 5 — Do You Need an RCD for Outdoor Lighting in Australia? (Short, high-intent compliance piece)

**Angle:** A short, direct-answer article targeting a specific compliance question people actually search. Cheap to produce relative to the others, strengthens the site's trust/compliance signal, and is genuinely useful rather than filler.

**Key facts to build it around:**
- AS/NZS 3000:2018 Amendment 2 closed a prior gap — all outdoor lighting circuits now require 30 mA RCD protection (previously some permanently wired outdoor lighting was exempt)
- RCD protection can be delivered via an RCD-protected circuit breaker at the switchboard or RCD-protected outlets at the point of use
- Type AC RCDs are no longer permitted for new or altered installations in Australia (since May 2023) — needs to be Type A minimum
- **[NEEDS CHRIS]** — practical framing: what this actually means for a homeowner getting garden lighting installed (i.e., "ask your electrician to confirm the circuit is RCD-protected to current standard," not a DIY checklist) — keep this one tightly scoped and accurate since it's compliance-adjacent; flag clearly that it's general information, not electrical advice, and a licensed electrician should confirm compliance for the specific installation

**Natural internal links:** Article 3 (in-ground cable joins), Article 4 (festoon/fairy near pools)

---

## Article 6 — Fittings That Live in Water: Materials, Water Chemistry & Why Connections Should Never Be Submerged

**Angle:** "Submersible" and "rated for wet locations" get used almost interchangeably by buyers, but a fitting sitting in a garden bed getting rained on and a fitting permanently sitting in chlorinated pool water are facing completely different chemical environments. IP68 tells you the housing keeps water out under a lab test — it says nothing about what the water itself will do to the fitting's materials over years of contact. This article does for submerged/water-contact fittings what Article 2 did for coastal atmospheric exposure.

**Structure:**

1. **"Submersible" ≠ one spec** — IP68 (continuous immersion) is a starting point, not the whole answer; AS/NZS 60598.2.18 is the actual Australian/NZ standard governing luminaires for pools, fountains, and garden pools specifically, requiring SELV (separated extra-low voltage), IPX8/IP68 watertightness, and Class III insulation. A fitting genuinely built to this standard is a different proposition to a generic "IP68 garden light" pressed into pool service.
2. **Why the water type matters as much as the IP rating** — the same IP68 fitting will age completely differently depending on what it's sitting in:
   - **Freshwater ponds/water features** — the mildest environment of the three; main long-term risks are UV exposure (if not fully submerged/shaded) and biofilm/algae buildup rather than aggressive corrosion
   - **Chlorinated pools** — chlorine isn't itself a strong oxidiser of metal, but at pool concentrations it attacks the passive chromium-oxide layer that protects stainless steel, particularly at welds, crevices and fixing points — this is why "stainless" pool fittings still pit and fail over time if the grade or fabrication quality is wrong
   - **Salt-chlorinated pools** — a common misconception is that salt pools are "gentler" than chlorine pools; they still generate chlorine (via the salt cell) and the added conductivity of the salt water actually accelerates galvanic corrosion between dissimilar metals, even though pool salt levels (~3,000–3,500 ppm) are nowhere near seawater (~35,000 ppm)
   - **Practical translation:** water type should drive material selection as deliberately as the coastal-zone table in Article 2 drives it for atmospheric exposure
3. **Materials that actually hold up in water contact:**
   - 316 stainless — still the benchmark, but grade and weld/fabrication quality matter more here than in atmospheric exposure, since crevice corrosion at a poor weld is exactly where chlorine attack starts
   - Marine bronze/brass — same patina-not-corrode logic as Article 2, genuinely well suited to water contact and long used in pool/fountain fittings
   - Anodised aluminium, resin-encapsulated, and engineered polymer housings — a strong option specifically because there's no base metal for the water chemistry to attack at all; often the more reliable long-term choice for pool-adjacent fittings than a poor-quality "stainless" one
   - Sacrificial (zinc) anodes — standard practice on pool equipment generally to protect more valuable metal components by corroding preferentially; worth a mention even where it's not built into the light fitting itself, since it affects the fitting's environment
4. **Neon flex / LED strip jacket material — this is where a lot of pool/water-feature jobs actually go wrong:**
   - **Silicone** — the correct choice for anything in sustained contact with pool/spa water: strong resistance to chlorine, salt, UV, and mild acids/alkalis, without the jacket breaking down and letting water reach the LEDs and copper strip beneath
   - **Polyurethane (PU)** — tougher mechanically and more abrasion-resistant, a reasonable choice for general exterior runs that get rained on, but breaks down faster under sustained chemical/chlorine exposure — fine for splash-zone or non-immersed exterior use, the wrong call for anything actually living in pool water
   - **PVC** — cheapest and least chemically resistant of the three; the one to avoid for any wet or chemically active application, pool or otherwise
   - **[NEEDS CHRIS]** — real examples of neon flex/strip failing in a pool or spa environment because the wrong jacket material was used (or specified by someone who didn't know the difference) — this is a strong "expertise" data point for the article
5. **Connections must be out of the water — no exceptions:**
   - Never splice or join cable underwater, regardless of the connector's own IP rating — this is standard trade practice, not a Solstice-specific opinion, and worth stating plainly
   - Route the cable so it rises out of the water to a connection point above the highest possible water level, in a covered/weatherproof junction box — not the fitting sitting low with a join buried below it
   - This is the same principle as Article 3's in-ground cable-join content taken further: get it wrong in soil and a fitting fails in a season or two; get it wrong permanently submerged and the timeline can be weeks
6. **Compliance callout** — ties to Article 5: pool circuits specifically are a heavily scrutinised area of AS/NZS 3000/60598.2.18 compliance; this is a "confirm with a licensed electrician" area, not a DIY one, and the article should say so plainly rather than reading as installation instructions
7. **Practical takeaway box** — decision path: identify the water type → select base material accordingly → if using strip/neon product, confirm silicone jacket for anything submerged → route and terminate all connections above the waterline → confirm compliance with AS/NZS 60598.2.18 for anything actually going into a pool

**Natural internal links:** Article 2 (materials/coatings — same logic, different chemistry), Article 3 (cable joins — same "keep it out of the water" principle escalated), Article 5 (RCD/compliance), Fitting Selector tool (worth considering whether the tool should also ask "is this fitting going in water?" as a second input alongside coastal proximity — flagging as a scope question for the tool build)

---

## Other topics worth considering (not yet scoped — flagging for the backlog)

Came up during research as genuinely useful, differentiated topics but not built out yet — worth a quick yes/no from Chris on which to add to the ~12-article target:

- **Sensors, timers and photocells** — dusk-to-dawn photocells vs astronomical timers vs motion sensors, and where each actually makes sense (ties into the RCD/compliance article and the smart-control section of Article 4)
- **Solar garden lighting — realistic expectations** — where solar genuinely works (path markers, low-demand accent) vs where it disappoints (anything needing consistent brightness or all-night operation, southern Australian winter daylight hours), a good "manage expectations before you buy" piece
- **Wildlife/ecology-friendly outdoor lighting** — reducing blue-rich light near bushland/waterways to limit impact on nocturnal wildlife (relevant to Australian conditions — flying-foxes, turtles, insects); this is a genuinely under-covered, non-generic angle few competitor sites take, worth considering as a differentiator
- **Seasonal/festive lighting safety** — Christmas light circuit loading, extension lead safety, what changes (and what doesn't) versus permanent festoon/fairy installs

---

## New Interactive Tool — Fitting Selector

**Concept:** User enters an address or suburb/postcode → tool estimates distance from coast and corrosivity zone per AS/NZS 2312/4312 → returns a plain-English minimum spec: material grade, coating/finish, fixing hardware, and IP rating guidance by application (path light, wall light, in-ground, near pool/spa).

**Confirmed with Chris:**
- The tool should also ask a second, independent question — **"is this fitting going in water?"** — alongside coastal proximity.
- **Scope for v1 (simplified, unblocks build now):** rather than a full combined water-type × coastal-zone recommendation table, a "yes" answer to the water question should return a guidance message rather than a specific material spec:
  - Explain that water type matters a lot (freshwater vs chlorinated pool vs salt-chlorinated pool all behave differently — see Article 6) and the right fitting depends on knowing which one applies
  - Recommend the user get in touch with Solstice directly to select the right fitting for their specific situation — a soft lead-gen CTA, not a DIY spec output
  - Name **Aqualux** and **Hunza** as the premier, fully maintainable fitting brands in the Australian market worth looking at for water-contact applications
  - The full water-type × material logic table (from Article 6) can be built out as a v2 enhancement once there's time to properly map it — not a blocker for v1
- Postcode-based lookup (not live geocoding) is fine for now.
- No corrections to the material/coating table below — Chris confirmed it's accurate as drafted.

### How it should work

**Input:** Address, or fallback to suburb/postcode (simpler, no geocoding API dependency, matches privacy-friendly approach of the other calculators) — **plus** a yes/no "will this fitting be in water?" toggle

**Core logic:**
1. Geocode/lookup approximate coordinates for the postcode/suburb
2. Calculate straight-line distance to nearest coastline (need a coastline dataset — this is the main technical dependency, worth scoping with Claude Code on data source/API before committing to the address-lookup approach)
3. Map distance → corrosivity category using AS/NZS 2312/4312 bands above (with the caveat that these bands assume typical conditions — wind, topography, and vegetation shift the real-world zone, and the tool should say so rather than present a false-precision result)
4. Return recommendation:

| Zone | Distance guide | Minimum material | Coating/finish | Fixings |
|---|---|---|---|---|
| CX | ~0–200 m, surf beach | Marine-grade 316 stainless, solid brass/bronze/copper, or marine-rated UV-stable polymer/composite | Marine powder coat system w/ full pre-treatment, or none needed (raw 316, or brass/bronze/copper left to patina) | 316 stainless only |
| C4/C5 | ~0–50 m sheltered coast, general coastal strip | 316 stainless, brass/bronze/copper, or high-quality marine-rated polymer preferred; high-spec coated aluminium as fallback | Full pre-treat + powder coat (if aluminium), inspect/maintain regularly | 316 stainless |
| C3 | ~100 m–few km inland | Coated aluminium (good quality die-cast), 304 stainless, or good-quality UV-stable polymer/composite | Standard powder coat with pre-treatment | Stainless or coated |
| C2 | Up to ~1 km from sheltered water | Standard coated aluminium or polymer/composite | Standard powder coat | Standard coated/stainless |
| C1 | 50 km+ inland | Standard aluminium/polymer fittings | Standard finish, no special coastal spec needed | Standard |

**On the material options:**
- **Brass/bronze/copper** — don't corrode structurally in salt air the way steel or poor-grade aluminium do; they oxidise/patina on the surface, which is largely cosmetic and often intentional (verdigris look in landscape fittings). A legitimate premium choice for CX/C4/C5, not just a stainless/aluminium binary. Worth noting in the article that patina finish is a design choice some clients love and others hate — set expectations.
- **Good-quality plastics/composites** — UV-stabilised polymers (not generic ABS) can outperform poor-quality aluminium in coastal zones since there's no metal to corrode at all; the main failure mode is UV degradation/embrittlement over time rather than salt attack. Worth distinguishing from cheap fittings that just happen to be plastic — quality of the polymer and UV stabiliser package matters as much as base material choice does for metal fittings.

**Confirmed:** table checked and approved by Chris — no corrections needed. **[NEEDS CHRIS]** — still open: IP rating guidance per application type (this table only covers material/corrosion, not ingress protection, and the two shouldn't be conflated in the output), and the water-contact branch of the logic (materials from Article 6, e.g. pool chlorine/salt vs freshwater) still needs mapping into the same table structure

**Framing for the disclaimer:** This should read as a planning/specification starting point, not a certification — recommend the user confirm with a qualified supplier/installer for the specific job, especially at zone boundaries.

**Build note for Claude Code:** the coastline-distance calculation is the one piece with real technical uncertainty (data source, accuracy, whether it needs a paid geocoding API or can use a free/open coastline dataset). Worth a short technical scoping pass before committing to the address-input UX — a postcode-to-zone lookup table (precomputed for Australian postcodes) might be simpler and more reliable than live geocoding + distance calc.

---

## Summary of what this adds to the build-out

- 6 new articles (of the ~12 targeted in the AdSense handoff) — technical (1–3), decorative/compliance (4–5), and water-contact materials (6), a good spread for AdSense's "genuine, varied content" bar
- 1 new interactive tool (6th calculator) — also a strong AdSense signal since it's genuine original functionality, not just content
- All six articles link to the new tool and to existing Garden Lighting/Lux calculators — improves internal linking, which also helps the "thin content" concern
- 4 further candidate topics identified and parked in the backlog above, pending Chris's steer on priority

## Open items for Chris

**Resolved (2026-07-31):**
- ~~Real numbers/rules of thumb for Article 1~~ — done: path 3W, step 1–2W, tree uplight 3–6W, façade wash 6W, driveway 6W
- ~~Field examples and product-specific detail for Article 2~~ — done: die-cast aluminium is the recurring coastal failure (rust/pitting/fading powder coat); Chris now specs copper, brass, bronze, anodised, coastal-rated powder coat
- ~~Sanity-check the Fitting Selector material/coating table~~ — done, confirmed accurate as drafted
- ~~Confirm postcode-lookup vs live geocoding~~ — done, postcode lookup confirmed for now
- ~~Real field examples of cable-route ingress failures for Article 3~~ — done: very common failure, "tons" of fittings seen with water travelled up the cable
- ~~Festoon spacing~~ — done: 50–100 cm depending on space/height
- ~~RGBW/RGBCCT honest take~~ — done: subjective, must stay classy/restrained, especially residential
- ~~Tree fixture wattage/beam angle~~ — done: no fixed formula, assessed per job — using that framing directly in the article
- ~~Should Fitting Selector ask about water exposure~~ — done: yes, confirmed as a second input alongside coastal proximity

**Still open:**
- Article 1: real jobs where over-lighting caused problems (glare complaints, blown-out driveways)
- Article 2: which specific ranges are genuinely marine-rated vs marketed as "coastal" without the material to back it up
- Article 3: keeping the anti-siphon connector mention generic for now (no product name) until Chris confirms the mechanism with the supplier — can be updated with specifics later
- Article 3: a genuine, trusted video URL for the IP68 join how-to (won't fabricate one)
- Article 4: any festoon jobs that failed early at joiners/fixings
- Article 5: sanity-check the homeowner-facing RCD framing
- Article 6: real examples of neon flex/strip failing in a pool/spa from wrong jacket material
- Fitting Selector: IP rating guidance per application; the full water-contact material logic table (v2 enhancement) — v1 just needs a guidance message + Solstice CTA + Aqualux/Hunza mention for the "in water" branch, which is now scoped and unblocked
