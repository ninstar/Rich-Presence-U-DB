# Rich Presence U - Database

Title database for https://github.com/ninstar/Rich-Presence-U.

**Pull requests** are welcome, but before doing so, read the section below.

## How to

Here are the list of games/softwares for each platform:

- Wii U - [wup.csv](titles/wup.csv)
- Nintendo Switch - [hac.csv](titles/hac.csv)
- Nintendo 3DS - [ctr.csv](titles/ctr.csv)

> Cells are separated by commas ``,`` and delimited by double quotation marks ``"``.

### Localizations

Each line is for a different game/software, regions are separated by columns with the following prefixes:

- **US** for America
- **EU** for Europe
- **JP** for Japan

You must fill out at least one of the cells in one of the `TITLE` columns. You don't have to fill the other cells if the title localization is the same for other regions.

*Example*

| ... | US_TITLE | EU_TITLE | JP_TITLE |
| --- | --- | --- | --- |
| ... | Super Mario |     | スーパーマリオ |

### Icons

The very first column is used to set an unique identification for the icon associated with the game/software, the filename of the icon should be the same, but with a region sufix appended.

*Example:* For a game/software entry like this:

| ID | ... | US_TITLE | EU_TITLE | JP_TITLE |
| --- | --- | --- | --- | --- |
| smario | ... | Super Mario |     | スーパーマリオ |

The filename of the icons should be like this:

> smario_us.png
> smario_jp.png

Here are the **requirements** for submitting icons:

- You need an icon for at least one region.
- The filename of the icon should be the same as the `ID` with a region suffix appended at the end.
- The minimum accepted size is **512x512** pixels.
- The aspect ratio must be **1:1** (Square).
- If the source image is low-res, the use of super-resolution for upscaling is preferable.

> ⚠ This repository isn't meant for hosting icons, you will have to include **a link for the icon in the description of your pull request**.

After making changes and submitting your pull request you will just have to be patient, I'll manually add the new icons to the *Discord Developer's Portal*. ☕

> All approved icons are also uploaded to this [drive folder](https://drive.google.com/drive/folders/1YfFO31--WDTFfD387-nJxnO88RQFs6tO?usp=sharing) for easy public access.

## Credits

All resources provided here were made possible thanks to the contribution of the following people:

- NinStar
- Majesty
- Sneethan
- Lakelimbo
- Luxen
- CodeBarre
- issey
- AbBrittus
- Peach774
- Sup3r-M4rio
- ShadowzI
- Schitzel9000
- Zyliqx
