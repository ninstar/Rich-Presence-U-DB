# Rich Presence U - Database

Title database for https://github.com/ninstar/Rich-Presence-U.

## How to contribute

This is a list of the currently supported platforms:

- Nintendo 3DS - [ctr.csv](titles/ctr.csv)
- Nintendo Switch - [hac.csv](titles/hac.csv)
- Nintendo Switch 2 - [bee.csv](titles/bee.csv)
- Wii U - [wup.csv](titles/wup.csv)

> [!Important]
>  Cells are separated by commas ``,`` and delimited by double quotation marks ``"``.

### Titles

Each line is used for a different software, regions are separated by columns with the following prefixes:

- **US** for America
- **EU** for Europe
- **JP** for Japan

You must fill out at least one of the cells in one of the `TITLE` columns. You don't have to fill the other cells if the title localization is the same for other regions (unless the region has a [unique icon](#icons) for the title being added).

**Example**

| ... | US TITLE | EU TITLE | JP TITLE |
| --- | --- | --- | --- |
| ... | Super Mario |     | スーパーマリオ |

### Icons

The first column is used to define a unique ID for the icon associated with the software. The icon filename should be the same, but with a region suffix appended.

**Example**

For a software entry like this:

| ID | US | EU | JP | US TITLE | EU TITLE | JP TITLE |
| --- | --- | --- | --- | --- | --- | --- |
| smario | ✓ |  | ✓ | Super Mario |     | スーパーマリオ |

The filename of the icons should be like this:

- ``smario.us.jpg``
- ``smario.jp.jpg``

> [!Warning]
> ``default`` and ``id`` are reserved internally, therefore you should not use them as the ID or filename of an icon.

The cells in columns 2, 3, and 4 (from left to right) should be populated with a character to indicate when a corresponding icon is available. It can be any character, but I recommend using a check mark (``✓``).

To avoid duplicates, when a software has different titles in different regions but shares the same icon in two or more of them, it is only necessary to provide an icon for only one region, this being the region with the highest priority. The order of priority is as follows:

- **US ➜ EU ➜ JP**

Applying this to the example above, only ``smario.us.png`` would be required.

**Icon requirements**

The guidelines for submitting icons are:

- An icon for at least one region.
- The file extension of the icon must be **.jpg**.
- The filename of the icon must be the same as the unique ID, with a region suffix added to the left of the file extension. (``*ID*.*REGION*.jpg``)
- The icon size must be **512x512** pixels (1:1) or larger.
  - Icons smaller than that should be enlarged using nearest neighbor scaling if they are evenly divisible by the 512x512, otherwise it is preferable to upscale them using bilinear or lanczos interpolation or other super-resolution methods.

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
- catfxngs
