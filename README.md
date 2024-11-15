# Rich Presence U - Database

Title database for https://github.com/ninstar/Rich-Presence-U.

**Pull requests** are welcome, but before doing so, read the section below.

## How to

Here are the list of games/softwares for each platform:

- Wii U - [wup.csv](titles/wup.csv)
- Nintendo Switch - [hac.csv](titles/hac.csv)
- Nintendo 3DS - [ctr.csv](titles/ctr.csv)

> Cells are separated by commas ``,`` and delimited by double quotation marks ``"``.

Cells in columns 2, 3 and 4 (from left-to-right) should be ignored and left empty as [they are filled after an icon is added to an application client](#addition-process).

### Localizations

Each line is for a different game/software, regions are separated by columns with the following prefixes:

- **US** for America
- **EU** for Europe
- **JP** for Japan

You must fill out at least one of the cells in one of the `TITLE` columns. You don't have to fill the other cells if the title localization is the same for other regions (unless that region has an [unique icon](#icons)).

**Example**

| ... | US TITLE | EU TITLE | JP TITLE |
| --- | --- | --- | --- |
| ... | Super Mario |     | スーパーマリオ |

### Icons

The very first column is used to set an unique identification for the icon associated with the game/software, the filename of the icon should be the same, but with a region sufix appended.

**Example**

For a game/software entry like this:

| ID | ... | US TITLE | EU TITLE | JP TITLE |
| --- | --- | --- | --- | --- |
| smario | ... | Super Mario |     | スーパーマリオ |

The filename of the icons should be like this:

- ``smario_us.png``
- ``smario_jp.png``

To avoid duplicates, when a game/software has a different title in one region region but happens to have the exact same icon in all of them it is only necessary to provide the icon for only one region, that being the region with the highest priority, the order of priority is the following:

- **US ➜ EU ➜ JP**

Applying this to example above, only ``smario_us.png`` would be required.

**Icon requirements**

- You need an icon for at least one region.
- The filename of the icon should be the same as the `ID` with a region suffix appended at the end.
- The minimum accepted size is **512x512** pixels.
- The aspect ratio must be **1:1** (Square).
- If the source image is low-res, the use of super-resolution for upscaling is preferable.

**Note:** This repository isn't meant for hosting icons, you will have to include a link or attachment of the icon in the description of your pull request.

## Addition process

After making the changes and submitting your pull request you will just have to be patient, I'll manually add the new icons to an application client in the Discord Developer's Portal, after that is done I'll set the client indexes to the corresponding cells (columns 2, 3 and 4).

The reason why this is done is because each application client has a limit of 300 icons (minus two considering the tooltip image for friend codes and the default platform logo for in-app custom entries), icons are distributed to the clients with available slots and these numbered cells represent the index of the Discord application client the icon is hosted, the list of client IDs for each platform and their respective indexes can be found in the [clients.cfg](clients.cfg)

> Approved icons are also added to this [archive](https://drive.google.com/file/d/1xZd9W63jLR-vvI73lcIWh4S-aj06DFXP/view?usp=sharing) for easy public access, they are separated by their assigned clients.

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
- gilramot
- K1rbYat1Na
- Kcroyals3
- Peach774
- Sup3r-M4rio
- ShadowzI
- Schitzel9000
- squihb
- teemerae
- yurisasc
- Zushi11
- Zyliqx
