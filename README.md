# Texas & Oklahoma Commercial Coating — Territory Map

Interactive territory map for commercial roof coating coverage across North, East and West Texas, plus the whole state of Oklahoma.

**Coverage**

- **Entire state of Oklahoma** — added north of the Red River. Tulsa and Oklahoma City hold the metro warehouse and manufacturing stock; between them it is ag buildings, grain elevators, poultry and light industrial, in the same hail belt. Drawn from real boundary data (687 points, vendored in `data/oklahoma-outline.js`) — the panhandle and the Red River are why that is real data rather than a hand-drawn box.

**Texas zones**

- US-75 Corridor Core (Sherman/Denison + semiconductor build-out)
- East Wing — 50 mi (Bonham → Paris)
- West Wing — 50 mi (Gainesville → Bowie)
- East Texas Pockets (poultry / dairy / food processing belt + Greenville I-30 connector)
- West Texas Expansion (Wichita Falls, Abilene, San Angelo, Lubbock, Amarillo)

**Stack:** single static `index.html` + vendored [Leaflet](https://leafletjs.com) 1.9.4 + vendored state boundary + Esri dark basemap. No build step.

⚠ The basemap is **Esri World Dark Gray, not CARTO**. CARTO's keyless dark
tiles now return stamped "API KEY REQUIRED" across the whole canvas, which
looks like a rendering fault rather than a licensing one. An OSM layer swaps in
on `tileerror` as a fallback.

**Run locally:** open `index.html` in a browser, or `python3 -m http.server` in the repo root.

**Deploy:** push to GitHub and import into [Vercel](https://vercel.com) (framework preset: *Other*, no build command, output dir: root).

Prepared by [RoofCoat Leads](https://roofcoatleads.com).
