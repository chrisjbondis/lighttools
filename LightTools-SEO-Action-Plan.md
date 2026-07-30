# LightTools SEO Action Plan
**lighttools.com.au | May 2026**

---

## Summary

The site has good bones — comprehensive calculators, solid technical content, proper Australian standards references, and a clean structure. The problem is almost entirely **authority and discoverability**: the site is new, has almost no backlinks, and is competing against established players for high-value keywords. Average position of 56.8 (page 5–6) with 2.32K impressions means Google is finding the pages, but not trusting them enough to rank them.

The good news: there's no fundamental SEO problem to fix. This is a "build trust and signal" challenge, not a "rebuild the site" challenge.

---

## The Biggest Issue: The voltagedrop.com.au Split

This is the #1 priority to investigate.

The lighttools.com.au homepage has a nav link to `/voltage-drop-calculator.html`, but the **tool card on the homepage** links directly to `https://voltagedrop.com.au` — a separate domain. This means:

- Every user who clicks "Open Calculator →" on the homepage leaves lighttools.com.au entirely
- The homepage's PageRank is flowing to an external domain instead of to your own voltage drop page
- Google sees the homepage as endorsing voltagedrop.com.au more than your own subdomain content
- Users who find lighttools.com.au's voltage-drop-calculator.html via Search Console data may be bouncing because the experience is split

**Fix:** Change the homepage Voltage Drop tool card to link to `/voltage-drop-calculator.html`. If voltagedrop.com.au is a separate standalone tool, that's fine — but the homepage should be building authority on lighttools.com.au, not bleeding it externally.

---

## Quick Wins (Do This Week)

### 1. Add FAQ Schema Markup to Voltage Drop Page

The voltage drop page already has a comprehensive FAQ section. Adding JSON-LD FAQ schema will make Google eligible to show **rich results** — expandable questions directly in the SERP. This dramatically improves CTR without changing position.

Example schema to add in `<head>`:

```json
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "What is the maximum allowed voltage drop in Australia?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "AS/NZS 3000 allows a maximum of 5% from the point of supply to any point in the installation. For 230V single phase that is 11.5V. For 400V three phase that is 20V."
      }
    },
    {
      "@type": "Question",
      "name": "How do I calculate voltage drop?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Single phase / DC: VD = 2 × L × I × ρ / A. Three phase: VD = √3 × L × I × ρ / A. Where L = one-way length (m), I = current (A), ρ = 0.0175 for copper or 0.028 for aluminium, A = cable size (mm²)."
      }
    }
  ]
}
```

Add this to ALL pages that have FAQ sections (voltage drop, LED driver, lux, garden lighting).

### 2. Add WebApplication Schema to Each Calculator

Tell Google explicitly that each page is a tool:

```json
{
  "@context": "https://schema.org",
  "@type": "WebApplication",
  "name": "Voltage Drop Calculator",
  "url": "https://lighttools.com.au/voltage-drop-calculator.html",
  "applicationCategory": "UtilityApplication",
  "description": "Free voltage drop calculator for Australian electricians. Single phase, three phase and DC. AS/NZS 3000 compliant.",
  "offers": {
    "@type": "Offer",
    "price": "0",
    "priceCurrency": "AUD"
  }
}
```

This signals to Google the pages are interactive tools, not just articles, which can influence how they're categorised and displayed.

### 3. Fix the Homepage Title Tag

**Current:** `LightTools — Free Lighting Calculators | AS/NZS 3000, AS 3008, NEC, IS 732, SANS 10142`

This is 83 characters — too long, gets truncated, and leads with the brand name nobody knows yet. The standards codes add no click value for users.

**Better:** `Free Lighting Calculators for Electricians | LightTools`

Or if you want to target Australian searches more directly:
`Free Electrical Calculators for Australian Electricians | LightTools`

### 4. Improve the Voltage Drop Page Meta Description

**Current:** "Free voltage drop calculator for Australian electricians. Calculate single phase, three phase and DC voltage drop instantly. AS/NZS 3000, NEC, IS 732 and SANS 10142 compliant. mm² and AWG cable sizes."

Good, but competitors likely have similar. Add a differentiator — your multi-mode calculator is genuinely more comprehensive than most:

**Better:** "Free Australian voltage drop calculator with 5 modes: single phase, three phase, DC, series runs & motor starting. AS/NZS 3000 compliant. Cable comparison table, ampacity check & worked examples."

The "5 modes" and "motor starting" are unique — lean into them.

---

## On-Page SEO: Page by Page

### Voltage Drop Calculator (`/voltage-drop-calculator.html`)
- **Title:** Good — "Voltage Drop Calculator Australia | LightTools" ✅
- **H1:** "Voltage Drop Calculator" — consider "Voltage Drop Calculator Australia" to match the target keyword
- **Target keywords:** `voltage drop calculator australia`, `voltage drop calculator AS/NZS 3000`, `three phase voltage drop calculator`, `DC voltage drop calculator`, `motor starting voltage drop`
- **Content:** Excellent — comprehensive reference guide, worked examples, FAQ, tables. This is the page's greatest strength. ✅
- **Internal links:** Add links from the homepage card directly to this page (fix the voltagedrop.com.au issue above)

### LED Strip Driver Calculator (`/led-strip-driver-calculator.html`)
Fetch and audit this page — based on the homepage description it's strong. Key targets:
- `LED strip driver calculator australia`
- `LED power supply calculator`
- `how to size an LED driver`
- `LED strip driver sizing 20% rule`

The 20% safety buffer content is a useful differentiator — lean into it.

### Lux Calculator (`/lux-calculator.html`)
The competition here is weak — Reduction Revolution has basic content, Solar Street Lights Australia is niche. A 4-mode lux calculator with UGR reference table and AS/NZS 1680 compliance is genuinely superior.
- **Target keywords:** `lux calculator australia`, `lux calculator for rooms`, `how many lumens do I need`, `downlight lux calculator`, `AS/NZS 1680 lighting levels`
- Add content about AS/NZS 1680 lighting standards by space type — offices, retail, healthcare. This is informational content electricians and designers search for.

### Garden Lighting Calculator (`/garden-lighting-calculator.html`)
This is potentially a strong differentiator — no obvious competitors ranking for AU-specific garden lighting voltage drop. Target:
- `garden lighting voltage drop calculator`
- `12V garden lighting calculator australia`
- `low voltage garden lighting cable sizing`
- `MeanWell driver selector garden lighting`

### LED Strip Installation Guide (`/led-strip-installation-guide.html`)
Not yet fetched, but this is likely a good candidate for informational SEO. Long-form guides rank well. Target:
- `how to install LED strip lights australia`
- `LED strip installation guide`
- `how to connect LED strip to driver`

---

## Content Strategy: Fill the Gaps

The site currently has tools but lacks **informational landing pages** that funnel into those tools. Users often search "how to calculate voltage drop" before they search for a calculator. Here are the highest-value content pieces to add:

### Priority 1: Cable Sizing Calculator / Guide
"Cable sizing" is a higher-volume term than "voltage drop" in Australia. A dedicated cable sizing calculator (or a page that positions the voltage drop calculator as a cable sizing tool) would capture significantly more search traffic.

- Suggested page: `/cable-sizing-calculator-australia.html`
- Target: `cable sizing calculator australia`, `cable size selection AS/NZS 3008`, `how to size a cable australia`
- This can be the voltage drop calculator reframed — same tool, new entry point.

### Priority 2: Electrician Tools Hub
Create a page at `/electrician-tools.html` that acts as an aggregator/index. Target: `free tools for electricians australia`. This page would interlink all calculators, improving internal link structure and giving Google a clear topical cluster.

### Priority 3: Per-Standard Landing Pages
Users search by standard. Consider thin but useful pages like:
- `/as-nzs-3000-voltage-drop.html` — explaining the standard and linking to the calculator
- `/nec-voltage-drop-calculator.html` — targeting US traffic which is a bonus audience

### Priority 4: "How to" Blog Posts
A few well-targeted how-to posts could drive significant informational traffic:
- "How to Calculate Voltage Drop in Australia (AS/NZS 3000)" — target position 1 for this with a comprehensive guide, then embed the calculator
- "How to Size an LED Driver — The 20% Rule Explained"
- "12V vs 24V LED Strip: Which Should You Use?"

---

## Technical SEO Checklist

| Item | Status | Action |
|------|--------|--------|
| HTTPS | ✅ Yes | — |
| Canonical tags | ✅ Yes | — |
| Mobile optimised | ✅ Yes (stated) | Verify with PageSpeed Insights |
| Sitemap | ❓ Unknown | Add XML sitemap at `/sitemap.xml`, submit to Search Console |
| robots.txt | ❓ Unknown | Verify exists at `/robots.txt` |
| Page speed | ❓ Unknown | Run PageSpeed Insights — calculators with JS need to load fast |
| Core Web Vitals | ❓ Unknown | Check Search Console → Experience → Core Web Vitals |
| Structured data | ❌ Missing | Add FAQ + WebApplication schema (see Quick Wins above) |
| Open Graph tags | ❓ Unknown | Add for social sharing (og:title, og:description, og:image) |
| Breadcrumbs | ❌ Missing | Add breadcrumb schema to inner pages |

---

## Link Building: The Long Game

With average position 56.8, the site almost certainly has very few external backlinks. This is the core problem. Content quality alone won't get you to page 1 against established players who have years of domain authority.

### Strategies That Work for Tool Sites

**1. Electrician Forums & Facebook Groups**
Post the calculators (genuinely, don't spam) in:
- Electricians Australia Facebook group
- Trade forums like Ozlecky / Elecaus
- Reddit r/AusElectricians

If the tools are useful, professionals share them — and those shares often become forum posts/blog links.

**2. Industry Directories**
List lighttools.com.au in:
- Master Electricians Australia
- NECA (National Electrical and Communications Association)
- State electrical licensing authority resource pages
- AIRAH (for lux/lighting content)

**3. Lighting Supplier Partnership**
Solstice Lighting's own website (solsticelighting.com.au) should link to lighttools.com.au. A "Tools for Installers" section on the supplier site with links to the calculators is a high-quality, topically relevant backlink.

**4. "Free Tools" Roundup Articles**
Search for "free tools for electricians australia" — there are blog posts and resource pages that list free calculators. Reach out and ask to be included.

**5. TAFE / Training Providers**
Electrical trade schools often link to useful reference tools. A submission to a few TAFE Victoria/NSW resource pages would be high-quality EDU-adjacent links.

---

## Keyword Target Map

| Page | Primary Target | Secondary Targets | Current Pos. (est.) |
|------|---------------|-------------------|---------------------|
| Voltage Drop | voltage drop calculator australia | three phase voltage drop calculator, DC voltage drop calculator, motor starting voltage drop | ~56 |
| LED Driver | LED strip driver calculator australia | LED power supply calculator, LED driver sizing | Not ranked |
| Lux | lux calculator australia | room lux calculator, how many lumens do I need | Not ranked |
| Garden Lighting | garden lighting voltage drop calculator | 12V garden lighting calculator, MeanWell driver selector | Not ranked |
| Homepage | free electrical calculators australia | lighting calculators australia, free tools for electricians | Not ranked |

---

## Competitor Analysis

### Voltage Drop — Top Competitors

| Site | Strengths | LightTools Advantage |
|------|-----------|---------------------|
| jCalc.net | Established, AS/NZS 3008 compliant, good UI | LightTools has 5 modes vs jCalc's 2; motor starting mode unique |
| CableHero | AU-focused, strong content | LightTools is free with no paywall/signup |
| AusInet | Simple, fast | LightTools has worked examples, formula explanations, more depth |
| voltagedropcalculator.com.au | Exact-match domain (big advantage) | LightTools broader tool suite = more internal authority |
| Elek | Professional-grade | LightTools more accessible for DIY + trade |

The exact-match domain `voltagedropcalculator.com.au` is a significant competitor advantage you cannot easily overcome. The play is to differentiate on features (motor starting, series runs, multi-region) and content depth.

### LED Driver — Moderate Competition
Cutter and M-Elec are the main AU competitors. Both have simpler calculators. LightTools' inclusion of voltage drop warning for long runs + MeanWell driver recommendations is a genuine differentiator.

### Lux — Low Competition
No dominant AU-specific lux calculator. This is the best opportunity to rank quickly.

---

## 90-Day Roadmap

### Month 1 — Technical Fixes & Quick Wins
- [ ] Fix voltagedrop.com.au homepage link split
- [ ] Add FAQ schema to all pages with FAQ sections
- [ ] Add WebApplication schema to all calculator pages  
- [ ] Fix homepage title tag
- [ ] Improve voltage drop meta description
- [ ] Submit XML sitemap to Search Console
- [ ] Run PageSpeed Insights, fix any critical issues
- [ ] Add solsticelighting.com.au backlink to lighttools.com.au

### Month 2 — Content Expansion
- [ ] Write "How to Calculate Voltage Drop in Australia" long-form guide (embed calculator)
- [ ] Create `/cable-sizing-calculator-australia.html` entry point page
- [ ] Create `/electrician-tools.html` hub page
- [ ] Fetch and audit LED driver, lux, and garden lighting pages — apply same SEO treatment
- [ ] Add H1 optimisation to all pages ("Australia" in H1 where missing)

### Month 3 — Link Building
- [ ] Post in 3–5 electrician forums/Facebook groups
- [ ] Submit to 5 industry directory listings
- [ ] Identify and contact 10 "tools for electricians" resource pages
- [ ] Reach out to 3 TAFE/training providers

---

## Metrics to Watch in Search Console

- **Average position:** Target < 20 for "voltage drop calculator australia" within 90 days
- **CTR:** Target > 2% (currently 0.2%) — schema rich results will help
- **Impressions growth:** Should increase as new pages are indexed
- **Click growth:** Primary goal — from 5 clicks/3mo to 50+ clicks/3mo

---

*Prepared by Claude | lighttools.com.au | May 2026*
