# Quality Furniture Matters

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

## Building from Source

If you want to modify the C# code:

```powershell
cd Source
dotnet build -c Release
```

The compiled DLL will be placed in the `Assemblies` folder.

## Requirements

- RimWorld 1.6

## License

MIT License - See [LICENSE](LICENSE) file for details.

## Author

Dakota Copas
