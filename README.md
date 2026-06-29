# 🚀 Aerospace Accident Investigation Registry

A free, self-contained **study & reference** web app on landmark **aerospace** accident investigations — aircraft, spacecraft, rockets, and hypersonic/supersonic vehicles — built for **students** and **investigators**.

🔴 **Live site:** https://shoiabgoku.github.io/aircraft-Investigation-reports/

It catalogues **86 documented occurrences (1954–2025)** — fatal *and* survivable — across every domain, manufacturer/agency, region and cause family, each structured the way an official report is: following **ICAO Annex 13** for aircraft, and the equivalent **Mishap Investigation Board / review-commission** logic for spaceflight (NASA, ESA, Roscosmos, ISRO, Rogers, CAIB…).

## What's inside

- **🗂️ Case Registry** — searchable, filterable cards. Search by name, vehicle, registration, location, cause or year. Filter by **domain** (Aircraft / Spacecraft & rockets / Hypersonic / Supersonic), **manufacturer or agency, region, occurrence category, investigating body, phase, report status, or decade**. Sort by recency, fatalities or operator. A live stat readout and decade chart update as you filter.
- **Case file (per occurrence)** — vehicle & mission identity, route/objective, human toll, phase, occurrence category, investigating body and status, **probable cause**, **contributing factors** split into *human / technical / organisational / environmental*, **safety recommendations & further actions**, a *student takeaway*, *why it matters*, the **official report / authority link**, and domain-aware **YouTube documentary + analysis links**.
- **🔬 How It's Investigated** — the 8-stage Annex 13 lifecycle (and its spaceflight equivalent), the four-factor model, James Reason's *Swiss-cheese* model, and the occurrence-category legend.
- **📖 Glossary** — 44 plain-language terms (CVR, FDR, CFIT, LOC-I, MCAS, RESA, hypoxia, COPV, RCC, scramjet, inlet unstart, inertia coupling, RUD, Max-Q, normalization of deviance…), filterable.
- **📺 Watch & Learn** — reputable aviation and spaceflight channels and series for further study.

## Coverage (86 cases)

**✈️ Aircraft (53)** — fatal landmarks (Comet, Tenerife, JAL 123, Pan Am 103, TWA 800, Concorde, AF447, MH370, MH17, the 737 MAX accidents, Air India 171…) and famous survivable saves (Gimli Glider, BA 9 volcanic ash, Aloha 243, BA 5390, US Airways 1549, Qantas 32, Air Transat 236, JAL 516 Haneda…).

**🚀 Spacecraft & rockets (25)** — Apollo 1 · Soyuz 1 · Soyuz 11 · Challenger · Columbia · Apollo 13 · Soyuz MS-10 abort · Nedelin catastrophe · N1 · Vanguard TV-3 · Ariane 5 Flight 501 · SpaceX CRS-7 · SpaceX AMOS-6 · Antares Orb-3 · Proton-M (2013) · Long March 3B (Intelsat 708) · Starship IFT-1 · ISRO SLV-3 · ISRO PSLV-D1 · Chandrayaan-2 (Vikram) · Mars Climate Orbiter · Mars Polar Lander · Genesis · Beresheet · Schiaparelli.

**⚡ Hypersonic / experimental (4)** — X-15 Flight 3-65 (Michael Adams) · NASA X-43A (Hyper-X) · Boeing X-51A Waverider · DARPA HTV-2.

**💨 Supersonic / experimental (4)** — SpaceShipTwo VSS Enterprise · XB-70 Valkyrie mid-air · SR-71 Mach-3 breakup (Bill Weaver) · Bell X-2 (Mel Apt).

## How to extend it

All data lives in the `DATA` array near the top of the `<script>` in [`index.html`](index.html). Add an object and the filters, stats and decade chart populate automatically. Set `domain` to one of *Aircraft* (default if omitted), *Spacecraft & rockets*, *Hypersonic / experimental*, or *Supersonic / experimental*. A new occurrence category just needs a colour in the `ACCENT` map and a one-line `CAT_DESC`. YouTube links are generated from the name (search links, so they don't go stale) and are domain-aware. The glossary, process steps and channels are simple arrays right below `DATA`.

## Tech

A single `index.html` — vanilla HTML/CSS/JS, **no build step, no dependencies, no tracking**. Works offline by opening the file directly. Deployed via GitHub Pages (Settings → Pages → *Deploy from a branch* → `main` / root).

## Disclaimer

This is an **educational, non-commercial reference**. Figures are drawn from official accident and mishap reports; for any operational, legal or research use, always consult the primary final report. Cases marked *Ongoing / Preliminary* have no final probable cause yet — findings shown are provisional. These are real tragedies; the registry exists to help understand and prevent the next one.
