# Extrudix Catalogs

This repository contains the catalog data used by the [Extrudix](https://www.extrudix.com) app for iOS and macOS. The app syncs these files automatically to populate its filament, parts, and printer reference catalogs.

## Files

| File | Description |
|------|-------------|
| `catalog_filaments.csv` | Filament catalog — brand, material, color, pricing, and spool specs |
| `catalog_parts.csv` | Parts catalog — nozzles, build plates, hardware, and consumables |
| `catalog_printers.csv` | Printer catalog — brand, model, build volume, and specifications |
| `catalog_versions.json` | Package version manifest — read by the app to display installed vs. available versions |

## Versioning

Each release of the catalog package is tracked in `catalog_versions.json`. The file contains a version string per catalog:

```json
{"filaments": "0.0.1", "parts": "0.0.1", "printers": "0.0.1"}
```

The Extrudix app reads this file when you open the Catalog Updates screen and displays your installed version alongside the available version for each catalog. When versions differ, the app shows an update indicator. Individual catalog versions are bumped when that catalog's data changes — not all three need to change together.

## Usage

Catalog files are fetched by the Extrudix app via **Settings → Data & Storage → Catalog Updates**. You do not need to download or modify these files manually — the app handles syncing automatically. An internet connection is required to fetch updates.

## Catalog Coverage

| Catalog | Entries | Brands / Models |
|---------|---------|-----------------|
| Filaments | 489 | 29 brands (Bambu Lab, Prusament, eSUN, Polymaker, Hatchbox, Overture, Sunlu, ColorFabb, MatterHackers, and more) |
| Parts | 469 | 40 brands (E3D, Slice Engineering, Micro Swiss, Phaetus, Bondtech, Orbiter, Capricorn, BigTreeTech, Bambu Lab, Prusa Research, Creality, LDO, and more) |
| Printers | 157 | Bambu Lab, Prusa, Creality, AnkerMake, Voron, Elegoo, Qidi, Flashforge, Raise3D, Ultimaker, Anycubic, Artillery, Sovol, RatRig, Snapmaker, FLSun, and more |

> **Note:** Catalog data is sample/reference data. Always verify specifications, pricing, and availability with the manufacturer or retailer before purchasing.

## Contributing

If you'd like to suggest additions or corrections to the catalog data, you can contribute via the Extrudix app itself:

- **Menu → Info → Contribute to the Catalog** — share your inventory CSV, share the catalog CSV, or submit via Google Form
- Email: extrudix@gmail.com

## Data Updates

Catalog data is maintained and updated by the Extrudix developer. Updates may include:

- New filament brands, materials, and colorways
- New printer models and specifications
- Expanded parts and hardware coverage
- Pricing and spec corrections

## All Catalogs Version History

### 0.0.1 — March 26, 2026
- Initial public release
- 489 filament entries across 29 brands
- 469 parts entries across 40 brands
- 157 printer models
- `catalog_versions.json` manifest added

## Filaments Catalog Version History

### 0.0.2 — March 29, 2026
- Added some UPCs

### 0.0.1 — March 26, 2026
- Initial public release
- 489 filament entries across 29 brands
- 469 parts entries across 40 brands
- 157 printer models
- `catalog_versions.json` manifest added

## Parts Catalog Version History

### 0.0.2 — March 29, 2026
- Added some UPCs

### 0.0.1 — March 26, 2026
- Initial public release
- 489 filament entries across 29 brands
- 469 parts entries across 40 brands
- 157 printer models
- `catalog_versions.json` manifest added

## Printers Catalog Version History

### 0.0.1 — March 26, 2026
- Initial public release
- 489 filament entries across 29 brands
- 469 parts entries across 40 brands
- 157 printer models
- `catalog_versions.json` manifest added

## License & Usage Rights

This catalog data is maintained by the Extrudix developer for use with the Extrudix app. The data may be read freely but may not be redistributed, repackaged, or used to build competing products without prior written permission.

© 2026 Extrudix. All rights reserved.
