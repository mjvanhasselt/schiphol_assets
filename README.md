# Schiphol Assets — GitHub Pages

Hosting van mobiele inspectiekaarten voor Schiphol, via GitHub Pages.

## URL's

Elke gegenereerde HTML is beschikbaar op:
```
https://mjvanhasselt.github.io/schiphol_assets/<bestandsnaam>.html
```

## Hoe werkt het?

HTML-bestanden worden gegenereerd door de `assets_in_map_mobile` repo:

```
1. Teken polygoon in route-tool → exporteer GeoJSON
2. ./maak_ronde.sh <polygon.geojson> "Ronde naam"  (vanuit assets_in_map_mobile)
3. Script genereert HTML, kopieert naar deze repo, commit + push
4. GitHub Pages publiceert automatisch
```

## Gerelateerde repos

| Repo | Doel |
|---|---|
| **route-tool** | Desktop kaart met polygoon-tekentools |
| **assets_in_map_mobile** | Mobiele HTML generator (Python + template) |
| **schiphol_assets** (deze repo) | GitHub Pages hosting |
