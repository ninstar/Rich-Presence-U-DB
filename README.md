# Rich Presence U - Database

Title database for https://github.com/ninstar/Rich-Presence-U.

**Pull requests** are welcome, but before doing so, read the section below.

## How to

Below are links to the table of titles for each platform:

- Wii U - [titles_wiiu.csv](/titles_wiiu.csv)
- Nintendo Switch - [titles_nswitch.csv](//titles_nswitch.csv)
- Nintendo 3DS - [titles_n3ds.csv](/titles_n3ds.csv)

Each line is for a different title, regions are separated by columns:

- US - *Americas*
- EU - *Europe*
- JP - *Japan*

You must fill out at least one cell in one of the columns that end with sufix ``TITLE``. You can leave them blank if there's no different name for other regions.

Example:

| US_TITLE			| EU_TITLE			| JP_TITLE
|-------------------|-------------------|--------------
| Super Mario		|					| スーパーマリオ

The first column (``INDEX``) is used to set a unique ID for the icon displayed on your status. **The file name of your icon should be the same** as the ``INDEX`` with a region identifier at the very ending.

Example:

| INDEX	 | ... | US_TITLE	 | EU_TITLE	| JP_TITLE
|--------|-----|-------------|----------|--------------
| smario | ... | Super Mario |			| スーパーマリオ

If that case the filename for the icons should be:

- smario_us.png
- smario_jp.png

> You need an icon for at least one region.

You can ignore all other columns, those are only set after your icons are uploaded to Developer's Portal.

After modifying a ``.csv``, you will have to include **a link for the icon of the newly added title in the description of your pull request**. The minimum accepted size is **512x512** pixels.
- If the source image is too blurry or pixelated, the use of super-resolution for upscaling is preferable.

☕ After that you will just have to be patient, I'll manually add your icon to the Discord Developer's Portal. You can find all icons uploaded so far on this [drive folder](https://drive.google.com/drive/folders/1YfFO31--WDTFfD387-nJxnO88RQFs6tO?usp=sharing).

> ⚠ This repository is not meant for hosting icons, only the strings for the titles used by the application.

## Credits

All resources provided here were made possible thanks to the contribution of the following people:

* Nin★ (NinStar)
* Majesty
* Sneethan
* Lakelimbo
* Luxen
* CodeBarre
* issey
* Peach774
* Sup3r-M4rio
* ShadowzI
* Schitzel9000
