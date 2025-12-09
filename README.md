# Quality Furniture Matters

A small release is available: **v0.1.0** — download the packaged mod ZIP from the GitHub Releases page:

[https://github.com/GrandMasterK414/QualityFurnitureMatters/releases/tag/v0.1.0](https://github.com/GrandMasterK414/QualityFurnitureMatters/releases/tag/v0.1.0)

A RimWorld 1.6 mod that makes the quality of end tables and dressers matter by adding rest effectiveness bonuses to linked beds.

## Features

**Quality-based rest effectiveness bonuses** from linked end tables and dressers:

| Quality | Rest Effectiveness Bonus |
|---------|-------------------------|
| Awful | -2% |
| Poor | -1% |
| Normal | 0% |
| Good | +1% |
| Excellent | +2% |
| Masterwork | +4% |
| Legendary | +8% |

**Linkable limits per bed:**
- Max 1 Dresser
- Max 2 End Tables

**Maximum potential bonus:** With 2 legendary end tables + 1 legendary dresser = **+24% rest effectiveness**

## Installation

1. Download or clone this repository
2. Place the `QualityFurnitureMatters` folder in your RimWorld `Mods` directory
3. Enable the mod in RimWorld's mod menu

## Building from Source (manual)

If you want to modify the C# code and build the DLL locally, run the following from PowerShell in this repository:

```powershell
cd Source
dotnet restore "QualityFurnitureMatters.csproj"
dotnet build -c Release
```

The compiled DLL will be placed in the `Assemblies` folder. Note: CI was previously considered but has been intentionally disabled; builds are done locally instead.

## Requirements

- RimWorld 1.6

## Compatibility

If other mods add furniture that should be treated like an end table or dresser for the purposes of this mod, you can register those def names with a small Def. Create a Def (in your mod or here) of type `QualityFurnitureMatters.QualityFurnitureConfig` and list the def names. Example:

```xml
<Defs>
	<QualityFurnitureMatters.QualityFurnitureConfig>
		<defName>QualityFurnitureMattersConfig</defName>
		<endTableDefNames>
			<li>MyMod_EndTableVariant</li>
		</endTableDefNames>
		<dresserDefNames>
			<li>MyMod_DresserVariant</li>
		</dresserDefNames>
		<otherFacilityDefNames>
			<li>MyMod_BedsideLamp</li>
		</otherFacilityDefNames>
	</QualityFurnitureMatters.QualityFurnitureConfig>
</Defs>
```

The mod will consult that Def at runtime and prefer configured entries when classifying linked furniture; it will still fall back to safe heuristics if no config is present.

## License

MIT License - See [LICENSE](LICENSE) file for details.

## Author

Dakota Copas
