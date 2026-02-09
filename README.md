# DefenseSpace 🔥

AI-powered wildfire defensible space assessment tool. Homeowners walk their property, photograph each zone, and get instant AI analysis of every hazard with specific fix recommendations.

## What It Does

- **Guided walkthrough** — zone-by-zone photo capture (Zone 0: 0-5ft, Zone 1: 5-30ft, Zone 2: 30-100ft)
- **AI object detection** — identifies 30+ hazard types: wood fences, juniper bushes, trash cans, propane tanks, bark mulch, dead trees, etc.
- **Species identification** — flags high-risk plants (juniper, eucalyptus, arborvitae, Italian cypress)
- **Zone grading** — scores against CA PRC 4291 + Zone 0 or NFPA Firewise USA standards
- **Fix recommendations** — specific, actionable fixes for every detection
- **Photo overlays** — AI bounding boxes drawn on captured photos with confidence scores

## Current Status

**Phase 1** — Demo/POC with simulated AI detections (working)  
**Phase 2** — Real Claude Vision API integration (planned)

## Quick Start

```bash
# Clone
git clone https://github.com/YOUR_USERNAME/defensespace.git
cd defensespace

# Run locally
npx serve public -p 3000
# Open http://localhost:3000 on your phone (same network)

# Or just open public/index.html in a browser
```

## Deploy to Vercel

```bash
# Install Vercel CLI if needed
npm i -g vercel

# Deploy
vercel

# Or connect GitHub repo in Vercel dashboard for auto-deploy
```

## Project Structure

```
defensespace/
├── public/
│   └── index.html      # Full PWA app (single file)
├── package.json
├── vercel.json          # Vercel deployment config
└── README.md
```

## Phase 2 Roadmap

- [ ] Claude Vision API integration (real photo analysis)
- [ ] Before/after comparison slider images
- [ ] Video capture + frame extraction
- [ ] PDF report generation
- [ ] Offline support (service worker)
- [ ] Plant species ID API integration
- [ ] LiDAR distance estimation (iPhone Pro)
- [ ] ArcGIS integration for parcel data overlay

## Standards Supported

- **California PRC 4291** + AB 3074 Zone 0 (2023)
- **NFPA Firewise USA** (national)

## Hazard Database

30+ detection types across 6 categories:
- Structures (wood fence, deck, pergola, shed, siding)
- Ground Cover (bark mulch, dry grass, leaf litter)
- Vegetation (juniper, eucalyptus, arborvitae, dead trees, ivy)
- Stored Items (trash cans, propane, firewood, vehicles, furniture)
- Building Features (vents, gutters, roof, windows, eaves)
- Fuel Patterns (ladder fuel, continuous vegetation, canopy contact)

## Built By

Dragon (Jeff Franzen) — GIS Developer, American Red Cross

---

*Protecting homes. Saving lives. One assessment at a time.*
