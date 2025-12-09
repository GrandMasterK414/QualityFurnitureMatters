# Quality Furniture Matters

A RimWorld 1.6 mod that makes the quality of end tables and dressers matter by adding rest effectiveness bonuses to linked beds.

## Features

Quality-based rest effectiveness bonuses from linked end tables and dressers:

| Quality | Rest Effectiveness Bonus |
|---------|-------------------------|
| Awful | -2% |
| Poor | -1% |
| Normal | 0% |
| Good | +1% |
| Excellent | +2% |
| Masterwork | +4% |
| Legendary | +8% |

## Linkable limits per bed

- Max 1 Dresser
- Max 2 End Tables

## Maximum potential bonus

With 2 legendary end tables + 1 legendary dresser = +24% rest effectiveness

---

For installation, building from source, compatibility notes, license, and author details see the `About` folder and `About/About.xml` in this repository.

---

## Steam Workshop Upload

An optional helper script `upload_workshop.ps1` is included in this mod root to generate a Steam Workshop VDF and upload the mod using `steamcmd`.

- **Defaults:** RimWorld AppID `294100` (change with `-AppId` if different).
- **Usage (interactive):** run PowerShell from the mod folder and execute:

```
.\upload_workshop.ps1
```

- **Usage (non-interactive):** provide parameters (must have `steamcmd` installed):

```
.\upload_workshop.ps1 -SteamCmdPath 'C:\steamcmd\steamcmd.exe' -AppId 294100 -PublishedFileId 1234567890
```

- The script reads `About/About.xml` to populate the workshop title and description and writes `workshop_build.vdf`.
- For security the script sends the login command to `steamcmd` via stdin (not on the command line), which avoids putting your plaintext password in the process command line. The script does not write your password to disk.
- **Security:** the script prompts for your Steam credentials locally. Do not paste your Steam password into this chat; run the script locally on your machine.

Recommended workflow: run the script from the mod folder (the script uses the script folder as the content folder), verify the created `workshop_build.vdf`, then allow the script to call `steamcmd` to perform the upload.

---

## Workshop Item

- **PublishedFileID:** `3620514068`
- **Workshop link:** https://steamcommunity.com/sharedfiles/filedetails/?id=3620514068

You can use this link to view the Workshop item, subscribe, or manually edit the item's description via the Steam web UI.

````

