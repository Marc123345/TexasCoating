# Texas Commercial Coating — Territory Map

Interactive territory map for commercial roof coating coverage across North, East, and West Texas.

**Zones covered**

- US-75 Corridor Core (Sherman/Denison + semiconductor build-out)
- East Wing — 50 mi (Bonham → Paris)
- West Wing — 50 mi (Gainesville → Bowie)
- East Texas Pockets (poultry / dairy / food processing belt + Greenville I-30 connector)
- West Texas Expansion (Wichita Falls, Abilene, San Angelo, Lubbock, Amarillo)
- Oil-Rich Zones (Permian Basin, East Texas Oil Field / Haynesville, historic North Texas fields)

**Stack:** single static `index.html` + vendored [Leaflet](https://leafletjs.com) 1.9.4 + CARTO dark basemap. No build step.

**Run locally:** open `index.html` in a browser, or `python3 -m http.server` in the repo root.

**Deploy:** push to GitHub and import into [Vercel](https://vercel.com) (framework preset: *Other*, no build command, output dir: root).

Prepared by [RoofCoat Leads](https://roofcoatleads.com).
