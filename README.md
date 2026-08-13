# Extrudix Catalogs

This repository contains the catalog data used by the [Extrudix](https://www.extrudix.com) app for iOS and macOS. The app syncs these files automatically to populate its filament, parts, and printer reference catalogs.

## Files

| File | Description |
|------|-------------|
| `catalog_filaments.csv` | Filament catalog: brand, material, color, pricing, and spool specs |
| `catalog_parts.csv` | Parts catalog: nozzles, build plates, hardware, and consumables |
| `catalog_printers.csv` | Printer catalog: brand, model, build volume, and specifications |
| `catalog_versions.json` | Package version manifest, read by the app to display installed vs. available versions |

## Versioning

Each release of the catalog package is tracked in `catalog_versions.json`. The file contains a version string per catalog:

```json
{"filaments": "0.0.6", "parts": "0.0.5", "printers": "0.0.2"}
```

The Extrudix app reads this file when you open the Catalog Updates screen and displays your installed version alongside the available version for each catalog. When versions differ, the app shows an update indicator. Individual catalog versions are bumped when that catalog's data changes, not all three need to change together.

## Usage

Catalog files are fetched by the Extrudix app via **Settings → Data & Storage → Catalog Updates**. You do not need to download or modify these files manually, the app handles syncing automatically. An internet connection is required to fetch updates.

> **Note:** Catalog data is sample/reference data. Always verify specifications, pricing, and availability with the manufacturer or retailer before purchasing.

## Contributing

If you'd like to suggest additions or corrections to the catalog data, you can contribute via the Extrudix app itself:

- **Menu → Info → Contribute to the Catalog**: share your inventory CSV, share the catalog CSV, or submit via Google Form
- Email: extrudix@gmail.com

## Data Updates

Catalog data is maintained and updated by the Extrudix developer. Updates may include:

- New filament brands, materials, and colorways
- New printer models and specifications
- Expanded parts and hardware coverage
- Pricing and spec corrections

## All Catalogs Version History

### 0.0.1 - March 26, 2026
- Initial public release
- 489 filament entries across 29 brands
- 469 parts entries across 40 brands
- 157 printer models
- `catalog_versions.json` manifest added

## Filaments Catalog Version History

### 0.0.6 - August 13, 2026
- Backfilled missing density values across several Bambu Lab lines (ABS-GF, ASA Aero and Basic, PETG CF and HF, PLA Aero)
- Added a UPC for Bambu Lab ABS-GF Gray

### 0.0.5 - June 19, 2026
- Added PA-6CF and some Matte Colors

### 0.0.4 - June 6, 2026
- Added TPU for AMS Neon Green China UPC

### 0.0.3 - March 30, 2026
- Added diameter column

### 0.0.2 - March 29, 2026
- Added some UPCs

## Parts Catalog Version History

### 0.0.5 - August 13, 2026
- Added three Bambu Lab parts: Cool Plate (SuperTack) for H2S, replacement PTFE tubing, and cleaning wipes
- Assigned a proper SKU and UPC to the Polymaker Filament Storage Box, replacing a duplicate placeholder row
- Corrected the compatibility note on two Bambu Lab build plates (Textured PEI, Smooth PEI) from "H2D and H2S" to "H2S"

### 0.0.4 - June 19, 2026
- Added Bambu Grease UPC

### 0.0.3 - June 6, 2026
- Added TPU feed assist module, BL liquid glue, and elmers glue stick.

### 0.0.2 - March 29, 2026
- Added some UPCs

## Printers Catalog Version History

### 0.0.2 - August 13, 2026
- Added Bambu Lab A2L, H2C, and X2D
- Removed redundant Bambu Lab bundle entries (A1 Combo, A1 Mini Combo, P1S Combo, X1 Carbon Combo) since these duplicated the specs of their standalone counterparts

### 0.0.1 - March 26, 2026
- Initial public release
- 489 filament entries across 29 brands
- 469 parts entries across 40 brands
- 157 printer models
- `catalog_versions.json` manifest added

## License & Usage Rights

This catalog data is maintained by the Extrudix developer for use with the Extrudix app. The data may be read freely but may not be redistributed, repackaged, or used to build competing products without prior written permission.

© 2026 Extrudix. All rights reserved.
