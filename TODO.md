# TODO

## Repo herstructurering

Er zijn drie repos die overlappend doel hebben en beter samengevoegd/gestructureerd kunnen worden:

1. **route-tool** — polygoon tekenen, route berekenen, desktop HTML genereren
2. **assets_in_map_mobile** — mobiele HTML generator + template
3. **schiphol_assets** (deze repo) — GitHub Pages hosting van gegenereerde HTML's

De workflow werkt (route-tool → generate_mobile.py → GitHub Pages), maar data (Excel assets) en code (point-in-polygon) zijn gedupliceerd. Overwegingen:
- Eén repo met gedeelde data en tooling?
- Of duidelijke scheiding met de huidige repos maar minder duplicatie?
