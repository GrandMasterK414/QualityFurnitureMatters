# Quality Furniture Matters (v0.1.2)

Adds small, quality-based rest effectiveness bonuses to beds from linked furniture (end tables and dressers). Bonuses are calculated at runtime from furniture quality so furniture themselves do not expose a special `BedRestEffectiveness` stat — this improves compatibility with other mods and keeps the UI uncluttered.

## Highlights
- Runtime, quality-based bonuses (no new furniture stat shown)
- Conservative defaults to stay friendly to vanilla gameplay
- In-game settings for toggles, per-bed caps, and a global multiplier

## Default mapping (per-item additive bonus)

| Quality | Bonus |
|---------|-------:|
| Awful | -1% |
| Poor | -0.5% |
| Normal | 0% |
| Good | +0.5% |
| Excellent | +1% |
| Masterwork | +2% |
| Legendary | +4% |

## Default caps (per-bed)
- Max 1 Dresser
- Max 1 End Table
- Max 2 total furniture counted

These conservative defaults avoid large swings in rest effectiveness. Adjust them in-game via Mod Settings (Mods → Quality Furniture Matters → Settings).

## Installation
1. Download the latest release ZIP from the Releases page: https://github.com/GrandMasterK414/QualityFurnitureMatters/releases/tag/v0.1.2
2. Extract or copy the `QualityFurnitureMatters` folder into RimWorld's `Mods/` directory so the mod folder contains `About/`, `Assemblies/`, `Defs/`, and `Patches/`.
3. Start RimWorld and enable the mod in the Mods menu.

## Settings
Open `Mods` → `Quality Furniture Matters` → `Settings` to:
- Toggle end-table and dresser contributions
- Adjust per-bed caps (dresser / end table / total)
- Apply a global multiplier to tune balance

## Modder notes
- If you want this mod to treat additional furniture as dressers or end-tables, add their `defName` to `Defs/QualityFurnitureMattersConfigDefs.xml` or create a new Def of type `QualityFurnitureMatters.QualityFurnitureConfig`.

## Compatibility
- Target: RimWorld 1.6
- This mod does not add or modify furniture placement rules. It only computes small runtime bonuses based on furniture quality.

## Reporting issues & feedback
- Please open issues on GitHub: https://github.com/GrandMasterK414/QualityFurnitureMatters/issues

## License
MIT — see `LICENSE` for details.

## Changelog
See `CHANGELOG.md` for release notes. (This repository provides runtime-only releases; source has been moved to a private backup.)


