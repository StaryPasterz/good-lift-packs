# Good Lift food packs

Data packs for the optional food diary of Good Lift, a personal training app. The app
downloads `catalog.json` from this repository and the pack archives from its releases; it never
needs this repository for daily use, and every pack can also be imported from a file.

A pack is a ZIP holding `manifest.json` and a read-only SQLite database. The app checks the
archive's SHA-256 from the catalog, then each file's size and SHA-256 from the manifest, before
it replaces an installed pack.

## Packs

| Pack | Contents | Sources and licence |
|---|---|---|
| `foods-pl` | Common foods with Polish names, aliases and household portions; Polish dishes computed from recipes | Values: USDA FoodData Central, SR Legacy (2018), CC0 1.0. A few Polish dairy products carry typical Polish label values where SR Legacy has no match, marked in each food's source. Names, portions and recipes: Apache License 2.0. |

Attribution: U.S. Department of Agriculture, Agricultural Research Service. FoodData Central,
SR Legacy (2018). https://fdc.nal.usda.gov/

The packs are built from the curation files and scripts in the app's repository
(`tools/nutrition/`).
