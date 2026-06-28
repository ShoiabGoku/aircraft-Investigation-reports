# ✈️ Aircraft Accident Investigation Registry

A free, self-contained **study & reference** web app on landmark aircraft accident investigations — built for **students** and **investigators**.

🔴 **Live site:** https://shoiabgoku.github.io/aircraft-Investigation-reports/

It catalogues **53 documented occurrences (1954–2025)** — fatal *and* survivable — across every manufacturer, region and cause family, each structured the way an official report is, following the **ICAO Annex 13** framework.

## What's inside

- **🗂️ Case Registry** — searchable, filterable cards. Search by airline, aircraft type, registration, location, cause or year. Filter by **manufacturer, region, occurrence category, investigating authority, phase of flight, report status, or decade**. Sort by recency, fatalities or operator. A live stat readout and decade chart update as you filter.
- **Case file (per crash)** — flight & aircraft identity, route, human toll, phase, occurrence category, investigating authority and status, **probable cause**, **contributing factors** split into *human / technical / organisational / environmental*, **safety recommendations & further actions**, a *student takeaway*, *why it matters*, links to the **official report**, and **YouTube documentary + pilot-analysis links**.
- **🔬 How It's Investigated** — the 8-stage Annex 13 lifecycle, the four-factor model, James Reason's *Swiss-cheese* model, and the occurrence-category legend.
- **📖 Glossary** — 30 plain-language terms (CVR, FDR, CFIT, LOC-I, MCAS, RESA, hypoxia, Swiss-cheese model…), filterable.
- **📺 Watch & Learn** — reputable channels and series for further study.

## Cases covered (53)

**Fatal & landmark:** Comet 781 · Turkish 981 · Tenerife · American 191 · Mt Erebus (Air NZ 901) · Saudia 163 · KAL 007 · Air India 182 (Kanishka) · JAL 123 · Pan Am 103 · United 232 · USAir 427 · American 965 (Cali) · ValuJet 592 · Charkhi Dadri mid-air · Birgenair 301 · Aeroperú 603 · SilkAir 185 · Korean Air 801 (Guam) · TWA 800 · Swissair 111 · Concorde · Alaska 261 · American 587 · Linate · China Airlines 611 · Überlingen · Helios 522 · Air France 447 · Colgan 3407 · Asiana 214 · MH370 · MH17 · AirAsia 8501 · Germanwings 9525 · Lion Air 610 · Ethiopian 302 · Air India Express 812 · Jeju Air 2216 · Air India 171.

**Survivable / famous saves:** Gimli Glider (Air Canada 143) · British Airways 9 (volcanic ash) · Aloha 243 · United 811 · British Airways 5390 · TACA 110 · US Airways 1549 (Hudson) · Air Transat 236 · Cathay Pacific 780 · Qantas 32 · LOT 016 · Southwest 1380 · Japan Airlines 516 (Haneda).

## How to extend it

All data lives in the `DATA` array near the top of the `<script>` in [`index.html`](index.html). Add an object and the filters, stats and decade chart populate automatically. New occurrence categories just need a colour added to the `ACCENT` map. YouTube links are generated from the flight name (search links, so they don't go stale). The glossary, process steps and channels are simple arrays right below `DATA`.

## Tech

A single `index.html` — vanilla HTML/CSS/JS, **no build step, no dependencies, no tracking**. Works offline by opening the file directly. Deployed via GitHub Pages (Settings → Pages → *Deploy from a branch* → `main` / root).

## Disclaimer

This is an **educational, non-commercial reference**. Figures are drawn from official accident reports; for any operational, legal or research use, always consult the primary final report. Cases marked *Ongoing / Preliminary* have no final probable cause yet — findings shown are provisional. These are real tragedies; the registry exists to help understand and prevent the next one.
