# Texas & Southern Oklahoma Commercial Coating — Territory Map

Interactive territory map for commercial roof coating coverage across North, East and West Texas, plus southern Oklahoma over the Red River.

**Southern Oklahoma** — added over the Red River, and deliberately NOT the
whole state.

- **Red River Band (OK)** — everything inside 60 road miles of the Denison
  centre line: Ardmore (55 mi — closer than Paris, TX, and a bigger industrial
  market: Michelin tyre plant, Valero refinery, I-35 distribution), Durant
  (23 mi — Choctaw Nation HQ, casino resort, manufacturing), Colbert, Madill,
  Tishomingo, Atoka.
- **Oklahoma Second Ring** — 75–135 road miles, the same reach as the East
  Texas pockets: Hugo, Ada, McAlester (Army Ammunition Plant), Idabel, Shawnee.

What is deliberately left out, and why:

| | from Denison | why not |
|---|---|---|
| Oklahoma City | ~160 road mi | a day each way, against local contractors |
| Tulsa | ~206 road mi | same |
| Lawton, Duncan | ~148, ~117 mi | only 48 and 51 mi from **Wichita Falls** — they belong to that zone if it goes live |
| Enid, Woodward | ~241, ~299 mi | too far |
| Panhandle (Guymon) | ~420 mi | 105 mi from **Amarillo** — belongs to that end, not this one |

There is no Oklahoma band polygon on the map, on purpose: the southern edge of
this territory is the Red River, which wanders, and a straight-line band would
put half of Grayson County, TX inside an Oklahoma zone. The two runs are drawn
as routes — US-75/69 north and US-70/I-35 west — with working radii on the
three anchors, because that is how they would actually be worked.

**Texas zones****Texas zones**

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
