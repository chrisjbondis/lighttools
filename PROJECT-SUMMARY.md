# LightTools & VoltageDrop — Project Summary

## What This Project Is

Two free electrical/lighting calculator websites monetised via Google AdSense and Amazon Associates affiliate links.

- **lighttools.com.au** — hub site with 5 calculators
- **voltagedrop.com.au** — standalone voltage drop calculator (keyword-exact domain)

---

## Server

| Detail | Value |
|---|---|
| Provider | Oracle Cloud Infrastructure (OCI) — free tier |
| OS | Ubuntu 22.04 |
| IP | 168.138.23.164 |
| SSH user | ubuntu |
| SSH key | `OneDrive\Desktop\ssh-key-2026-04-21 (1).key` |
| Web server | Nginx |
| SSL | Let's Encrypt (Certbot) — auto-renews |

### SSH Command (PowerShell)
```powershell
ssh -i "$env:USERPROFILE\OneDrive\Desktop\ssh-key-2026-04-21 (1).key" ubuntu@168.138.23.164
```

---

## Domains

| Domain | Purpose | DNS |
|---|---|---|
| lighttools.com.au | Main hub site | A record → 168.138.23.164 |
| www.lighttools.com.au | Redirects → lighttools.com.au | A record → 168.138.23.164 |
| voltagedrop.com.au | Standalone voltage drop calculator | A record → 168.138.23.164 |
| www.voltagedrop.com.au | Redirects → voltagedrop.com.au | A record → 168.138.23.164 |
| voltagedrophelp.com | Redirects → voltagedrop.com.au | A record → 168.138.23.164 |
| lighttools.tools | Redirects → lighttools.com.au | A record → 168.138.23.164 |
| lighttools.co.in | Redirects → lighttools.com.au | A record → 168.138.23.164 |
| lighttools.africa | Redirects → lighttools.com.au | A record → 168.138.23.164 |

DNS registrar: **Ventra IP**

---

## File Structure

### On the server
```
/var/www/lighttools/        ← lighttools.com.au web root
/var/www/voltagedrop/       ← voltagedrop.com.au web root
/etc/nginx/sites-available/lighttools   ← Nginx config (all sites)
```

### On your computer (C:\Users\user\Documents\Claude\Projects\)
```
lighttools/
  index.html                  ← Homepage + hub
  disclaimer.html
  sitemap.xml
  voltage-drop-calculator.html
  led-strip-driver-calculator.html
  led-strip-light-selector.html
  lux-calculator.html
  garden-lighting-calculator.html

voltagedrop/
  index.html                  ← Full 5-mode voltage drop calculator
  disclaimer.html
  sitemap.xml

lighttools-nginx.conf         ← Nginx config backup
```

---

## How to Upload Files to the Server

### Upload lighttools files (PowerShell)
```powershell
scp -i "$env:USERPROFILE\OneDrive\Desktop\ssh-key-2026-04-21 (1).key" "C:\Users\user\Documents\Claude\Projects\lighttools\*" ubuntu@168.138.23.164:/var/www/lighttools/
```

### Upload voltagedrop files (PowerShell)
```powershell
scp -i "$env:USERPROFILE\OneDrive\Desktop\ssh-key-2026-04-21 (1).key" "C:\Users\user\Documents\Claude\Projects\voltagedrop\*" ubuntu@168.138.23.164:/var/www/voltagedrop/
```

### Upload Nginx config (PowerShell)
```powershell
scp -i "$env:USERPROFILE\OneDrive\Desktop\ssh-key-2026-04-21 (1).key" "C:\Users\user\Documents\Claude\Projects\lighttools-nginx.conf" ubuntu@168.138.23.164:/home/ubuntu/lighttools-nginx.conf
```
Then on the server:
```bash
sudo cp /home/ubuntu/lighttools-nginx.conf /etc/nginx/sites-available/lighttools && sudo nginx -t && sudo systemctl reload nginx
```

---

## Monetisation

### Google AdSense
- Publisher ID: **ca-pub-1409689781104144**
- Status: Applied — "Low value content" flag (content additions uploaded, awaiting re-review)
- ads.txt live on both sites

### Amazon Associates
| Program | Tag | Used on |
|---|---|---|
| Amazon AU | lighttools-22 | All AU calculator pages |
| Amazon US | lighttools22-20 | US region calculator pages |
| Takealot (ZA) | (no tag) | ZA region — no affiliate yet |
| Amazon India | (not yet applied) | Apply when AU traffic grows |

---

## Analytics & Search Console

### Google Analytics 4
- Account: LightTools (under chris@solsticelighting.com.au)
- lighttools.com.au stream: **G-82HX4HNTVF**
- voltagedrop.com.au stream: **G-315J8CF00W**

### Google Search Console
- lighttools.com.au — verified, sitemap submitted
- voltagedrop.com.au — verified, sitemap submitted
- Both sites submitted for indexing

---

## lighttools.com.au — Calculator Pages

| Page | File | Theme colour |
|---|---|---|
| Homepage | index.html | Blue |
| Voltage Drop | voltage-drop-calculator.html | Blue |
| LED Strip Driver | led-strip-driver-calculator.html | Gold |
| LED Strip Selector | led-strip-light-selector.html | Purple |
| Lux Calculator | lux-calculator.html | Amber |
| Garden Lighting | garden-lighting-calculator.html | Green |

Each page has: calculator + article content + FAQ accordion + FAQ JSON-LD schema

---

## voltagedrop.com.au — Calculator Modes

1. Single Phase AC
2. Three Phase AC
3. DC
4. Series Runs
5. Motor Starting

Region toggles: AU / US / IN / ZA (adjusts standards, cable sizes, voltage drop limits)

---

## Pending / To Do

- [ ] Wait for AdSense re-review (low value content flag)
- [ ] Wait for Google indexing (1–4 weeks for new domains)
- [ ] Click "Validate Fix" in Search Console for both sites (www redirect canonical issue now fixed)
- [ ] Delete accidentally created empty Analytics property G-NQNQ83PG3F
- [ ] Apply for Amazon India Associates when AU traffic grows
- [ ] Consider Commission Factory (AU) for Bunnings/RS Components links
- [ ] Consider building more standalone tool sites (cable sizing, lux, etc.)

---

## SSL Certificates (Let's Encrypt)

| Cert | Covers | Expires |
|---|---|---|
| lighttools.com.au | lighttools.com.au + www + .tools + .co.in + .africa variants | 2026-07-28 |
| voltagedrop.com.au | voltagedrop.com.au + www + voltagedrophelp.com + www | 2026-07-29 |
| optimisedeats.com | optimisedeats.com + www | 2026-08-02 |

Certbot auto-renews — no action needed unless it fails.
