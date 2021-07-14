# Rich Presence U - Database

Title database for https://github.com/ninstar/Rich-Presence-U.

**Pull requests** are welcome, but before doing so, read the section below.

## How to

Below are links to the table of titles for each platform:

- Wii U - [titles_wiiu.csv](/titles_wiiu.csv)
- Nintendo Switch - [titles_nswitch.csv](//titles_nswitch.csv)
- Nintendo 3DS - [titles_n3ds.csv](/titles_n3ds.csv)

Each line is for a different title, columns are separated by regions:

- US - *Americas*
- EU - *Europe*
- JP - *Japan*

You must fill in at least one cell in one of the columns that end with``TITLE`` as their header. If there's no different name for other regions, you can leave them blank.

Example:

| US_TITLE			| EU_TITLE			| JP_TITLE
|-------------------|-------------------|--------------
| Super Mario		|					| スーパーマリオ

The first column (``INDEX``) is used to set a unique ID for the title's icon. **The file name of your icon** should be the same as the ``INDEX`` with a region identifier at the very ending.

Example:

| INDEX	 | ... | US_TITLE	 | EU_TITLE	| JP_TITLE
|--------|-----|-------------|----------|--------------
| smario | ... | Super Mario |			| スーパーマリオ

If that case the filename for the icons should be:

- smario_us.png
- smario_jp.png

> You need to have an icon for at least one region.

You can ignore all other columns, those are only set after your icons are uploaded to Developer's Portal.

After modifying a ``.csv`` you have to include a **link for the icon of the newly added title on the description of your pull request**. If you forget to do that you can still submit your icon through this [drive folder](https://drive.google.com/drive/folders/1YfFO31--WDTFfD387-nJxnO88RQFs6tO?usp=sharing) or [this form](https://forms.gle/SztU5GdQEgwx45GX8).

The minimum size needs to be **512x512** pixels.
- If the source image is too blurry or pixelated the use of super-resolution for upscaling or a manual recreation is preferable.

☕ After that you just have to be patient, I'll manually upload your icon to Discord Developer's Portal.

> ⚠ This repository is not meant for hosting icons, only title and references are hosted here.

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
* Sneethan
