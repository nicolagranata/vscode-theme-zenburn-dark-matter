# `Zenburn Dark Matter` Theme Change Log 

> Note 1: This Changelog is for the whole **Dark Matter Suite**, not just for this specific Theme.

> Note 2: [`Development`] and [`UI Manager`] sections in *Changelog* are addressed to the developer to remind him of any important changes that occurred during the writing of the code and do not always concern improvements made to the extension or to the theme.

## [1.1.159]
- [`Development`] Optimized Preview Generator;

## [1.1.158]
- [`Development`] Fix Preview Generator;

## [1.1.157]
- [`Theme`] Improved `editorBracketMatch` highlight color;
- [`Development`] Addedd `editorBracketMatch` as independent from automatic colorization keywords;
- [`Development`] Added Daily / Hourly / Delta foresights to statistics table;
- [`Readme`] Added some new fonts: "Dank Mono", "Ginotronic", "Monego" family, "M+ 2m" Family, "Operator Mono Lig", "Monaco", "BPmono", "Bitstream Vera Sans Mono", "Luculent", "Whois mono", "NotCourierSans", "KawKab Mono", "Metrickal";

## [1.1.155]
- [`Theme`] Added `tab.lastPinnedBorder` color (VSCode 1.50);
- [`Theme`] Fix some UI and Token colors;
- [`Readme`] Fix some issue and improved Fonts Data Sheet table readability. Removed Font Weight from columns to prevent a partial cut-out of Fonts Table in Marketplace;
- [`Readme`] Added some new fonts, revised some parameters of the existing ones;
- [`Development`] Added `Famous Quotes from Movies` to `Fake UI` to better show font applied in fake screenshot;
- [`Development`] Fix Fake UI elements due to browser or html2canvas.js improvements (partially hidden UI objects or wrong location in rendering);
- [`Development`] Minor bugs fixed;

## [1.1.151]
- [`Theme`] Fix some UI and Token colors;
- [`Readme`] Added some new fonts, revised some parameters of the existing ones;
- [`Readme`] Fix some issue and improved Fonts Data Sheet table readability;
- [`Development`] Some code improvements;
- [`Development`] Fix for some randomizations of `Fake UI`;
- [`Development`] Added `Search` to `Fake UI` Activity Bar and removed from Panel according to `VSCode 1.46.00 Insider Preview`;
- [`Development`] Added `Week Days` to survey data weekly (count of each week day from publication, downloads in week day from publication, average downloads in week day, peak of the week)
- [`Development`] Added `Delta` (&Delta;) to get difference between last values and previous values, `Week Day of Downloads Peak`, `Survays Numbers` (with previous value stored in `Days from Publication`) columns to `Stats` table and fixed value of `Days from Publication`;

## [1.1.147]

- [`Theme`] Added new theme colors for `VS Code 1.45.00`;
- [`Development`] Fixed some visual bugs in `Fake UI` (Minimap and Indent Guides);
- [`Development`] Optimized `Stats` columns generation;
- [`Development`] Added last `n` (default = 30) surveys downloads trend and column color for `Last Interval Survey`;

## [1.1.146]

- [`Readme`] Fixed some issues in  `README.md` and `CHANGELOG.md` generation.

## [1.1.144]

- [`Readme`] A little improvement to table of `Suggested fonts`, repeating headers every 10 items for more readability;
- [`Readme`] Waiting for GitHub and VS Code Market to agree on how to generate the ids for the internal hyperlinks of the table of contents, I tried to optimize (as it was some version ago) the title text so that the hyperlinks are working both on the Marketplace ceh on Github (and not only on Github)
- [`Theme`] I know, the need was not felt, but I created a new theme for my favorite tokencolors. `Apophis Monolith` and `Zenburn Monolith` are based on a single color in various intensities for each skin;
- [`Theme`] Renamed skins `Golem` to  `Morion`, `Monolith` to  `Aquamarine` and `Salamander` to  `Sulfur`;
- [`Development`] Improved function `alphamatte` and `alphaifbright` for better color results;

## [1.1.140]

- [`Theme`] Added skins `Golem`, `Monolith` and `Salamander`, based on a single color in various intensities;
- [`Development`] Added function `alphamatte` wich use `color_blend` function with current background color, to fix issue with VSCode terminal colors that do not accept alpha channel and render color as full white;
- [`Development`] Added function `alphaifbright` function which reduces the alpha if the color is too white;;

## [1.1.136]

- [`Theme`] Improved some UI skin's main colors;
- [`Readme`] Found a little mistake that involving my `Table o Contents` generator: `GitHub` and `Visual Studio Marketplace` not uses same method to `hash bookmarks`: offline, in `VSCode`, `MD preview` seems to behave like `GitHub`, but once published, no: when `README.md` showed in preview or in Extension Documentation or on GitHub, bookmarks works correctly, but in the same version, in Marketplace, some bookmarks not working (those that have some particular characters that GitHub replaces each with a `-`, while Marketplace replaces all those sequential with a single `-`):
	- e.g.: # **All work [ and no play ] makes Jack a dull boy**:
		- GitHub / Markdown Preview on VSCode 	» `#all-work---and-no-play---makes-jack-a-dull-boy`;
		- Visual Studio Marketplace 			» `#all-work-and-no-play-makes-jack-a-dull-boy`;
- [`Readme`] Added `tab` char to `Suggested fonts` default settings and symbols for font properies;
- [`Readme`] Added font properties columns `Zero Slashed or Dotted`, `Serif` and `Cursive` in table of `Suggested fonts`. Also some new fonts added;
- [`Development`] Added `skinUiColorsOverrides` array. This array takes priority over some colors already calculated, to better adapt some shades to the main color of single skin;

## [1.1.134]

- [`Theme`] Added `Kronos` skin's main color;
- [`Theme`] Added `Equinox` skin's sub-set, with Deep Dark/Blue background and desatured token colors;
- [`Theme`] Satured `Viserion` skins's main color;
- [`Theme`] Some improvements to theme colors (highlights, errors ad badges color) fol all themes and some tokencolor scopes for *Apophis*;
- [`Readme`] Now `Suggested fonts` shows the default settings in `JSON` format, to quickly test the fonts in `Settings.ini` with reasonable minimum values, for each of them, to limit visual fatigue;
- [`UI Manager`] Added `Console Log Monitor` for check the progress of skin's rendering in `html2canvas`;
- [`UI Manager`] Added `Incremental Counter Monitor` for check the progress of skin's rendering in page;
- [`UI Manager`] Added checkbox to enable randomization of `Fake UI` elements;
- [`Development`] Fixed a bug in the `README.md` / `Table of Contents` generator: the bookmarks, under certain conditions, were not generated correctly.
- [`Development`] Each preview is generated using a different font from those listed among the fonts suggested on this page. ;
- [`Development`] Added `HTML` example master file for `Fake UI` generator;
- [`Development`] Added function to randomize `Fake UI` elements while maintaining consistency between sections;
- [`Development`] Improved function to exclude themes by generation, for themes without expected imminent improvements;
- [`Development`] Functions and visual improvements (colors, tokencolors, new elements and icons) for `Fake UI Generator`;
- [`Development`] Improved function for cleaning SVG icons for theme-dependent coloring;
- [`Development`] Improved function for `Alpha Blend Color` calculation (previously called `Middle Color`) between two colors. This function, in combination with the `Text Color` function, returns the most suitable color for text on a given background, better than previously function versions;
- [`Development`] Improved function for `Text Color` calculation on background color (based on better `Luminosity Contrast` and no longer on `Luminance`);
- [`Development`] Added `Equalize` color function to equalize color to near gray color, used for foreground text color based on satured main color.

## [1.1.132]

- [`Theme`] Some improvements to theme colors;
- [`Theme`] Some improvements to token colors;
- [`Readme`] Added new fonts suggestion in `README.md`;
- [`Development`] Some improvements to `Markdown Table Maker`;
- [`UI Manager`] Added button to go directly to marketplace of extension (override the label of first SVG badge).

## [1.1.129]

- [`Theme`] Satured `Mystic River` skin's main color and added to `Apophis Dark Matter Theme`;
- [`Theme`] Added `Cold`, `Flat`, `Warm` (Grays) skin's sub-set to `Apophis Dark Matter Theme`;
- [`UI Manager`] Added live badges strip under each theme panel.
- [`Development`] Added functions for get installs number dynamically from badges;
- [`Development`] Added functions for themes installs statistics;
- [`UI Manager`] Solved CSS issue with sticky header.

## [1.1.128]

- [`Development`] Improved function that determine `VSCode Themes Master` version based on each included file;
- [`Development`] Improved function for `Text Color` calculation on background color (based on `Luminance`);
- [`Development`] Improved function for Luminance calculation (with calculation of Middle Color when colors are overlayed and with transpacency);
- [`Development`] Added function for `Middle Color`: overlay result of foreground color wit opacity on background color whit/whitout opacity on default (deep) background color;
- [`Development`] Improved line highlight background for foreground readability.

## [1.1.127]

- [`Development`] Solved issue with export value of Notifications opacity;

## [1.1.125]

- [`Theme`] Added more opacity to selection background;
- [`Theme`] Tanks to bugfix [#85690](https://github.com/microsoft/vscode/issues/85690) in VSCode 1.42.0, added a bit of transparency to dropdown menu and notifications pop-up;
- [`Theme`] In all the themes, only for token colors, the saturation filter has been replaced with the alpha filter to better blend the colors of the tokens with the background color. This avoids (or reduces) non-harmonic overlaps of text with background;
- [`TokenColors`] Added `Apophis` tokencolors set an new Themes based on `Dark Matter` skins. `Apophis`, use only a subset of `Dark Matter` skins with which it is more in color harmony;
- [`Readme`] Added some font suggestion in `README.md`;
- [`UI Manager`] Added support for testing themes in VSCode insiders;
- [`UI Manager`] Added `Apply & URefresh` button for refresh page without regenerate UI colors and Fake UI previews and apply options (e.g. step-up version);
- [`UI Manager`] Added `Ultra Refresh` button for refresh page without regenerate UI colors previews and Fake UI previews;
- [`Development`] Fixed some comments in Token colors JSON: removed, with RegExp, encoded html chars and some PHP explicited tags to avoid conflicts with PHP scripts of `VSCode Themes Master`;
- [`Development`] Fixed some inaccuracies in the in PHP function **make_code_example** that emerged after the introduction of `Apophis` tokencolors;
- [`Development`] After introduction of `excluded_tokencolors_set_main`, `excluded_tokencolors_set_skin`, `excluded_tokencolors_set_combo`, added generation of UI colors preview for each tokencolors file.
- [`Development`] Added `excluded_tokencolors_set_main`, `excluded_tokencolors_set_skin`, `excluded_tokencolors_set_combo` arrays in `_cfg.themes.colors.php` wich respectively exclude:
  1. All token colors set in array from Main Theme (Group);
  1. All token colors set in array from Single Sub-Theme;
  1. All token colors set in array from Colors Combo for each Sub-Theme;
     This allows me to better manage the combined colors and exclude those that are not harmonic.
- [`Development`] Generic code bug fix and improvements;

## [1.1.122]

- [`Theme`] In `Low Blue` sub-theme, skin `Moai` was replaced by skin `Obsidian`;
- [`Theme`] Added `Obsidian` skin to some sub-themes;
- [`Readme`] Added big picture preview of a random skin of set;
- [`UI Manager`] Added `Quick Refresh` button for refresh page without regenerate Fake UI previews;
- [`Development`] Generic code bug fix and improvements;

## [1.1.114]

- [`Theme`] Some `keywords` changed;
- [`Readme`] Some `README.md` corrections;
- [`Development`] Improved function to get the harmonic colors;
- [`Development`] Generic code bug fix and improvements;

## [1.1.109]

- [`Readme`] Fixed bug in gallery with direct link of images preview;
- [`Development`] The gray-scale determination criteria have been modified to try to improve the readability of the text on some background colors in themes.
- [`Development`] Improved function to get the grayscale (using HSL instead of the common RGB to gray) of a background color to better evaluate the color of the text to be used on it.

## [1.1.106]

- [`Themes`] Removed `fontStyle`: `bold` from tokencolors: this make code more readable at low font size;
- [`Readme`] Added `Table of Contents`;
- [`Readme`] Added some informations about fonts rating;
- [`Development`] Fixed a bug in load and manage JSON export from Visual Studio Code. Added a code to remove special PHP symbols from JSON that can be recognized as "active code" by `VSCode Themes Master`;
- [`Development`] Added options to remove `fontStyle` => `bold`/`underline`/`italic` form Token Colors (`tokenColorsOptions` can be different for for each sub-theme);
- [`Development`] Implemented function to make hierarchical `Table of Contents`;
- [`Development`] Rewritten function to make `Themes Gallery` to solve a bug with table generation;
- [`Development`] Implemented function to manage suggested fonts for coding.

## [1.1.102]

- [`Themes`] Added `Insomnia` sub-theme, clone of Nadir, with flatten colors, low UI contrast, and ultra-satured token colors: although this skin is the opposite concept to the others, in conditions of excessive brightness of the room, it may be convenient to have a theme with greater contrasts;
- [`Readme`] Added sample color previews of UI (1st row) and Token Colors (2nd row) to UI previews;
- [`Readme`] The organization of the previews is more orderly;
- [`Readme`] Added font suggestion section;
- [`UI Manager`] Improved `Token colors Inspector`: now, if opacity is present, shows the same color in two swatches: with and without opacity;
- [`Development`] Implemented function to manage colors using HSL/HSV and improved some ColorMath functions;

## [1.1.101]

- [`Themes`] Added `Deep Sea` sub-theme, with extra deep blue background, flatten colors, low UI contrast, and ultra-desatured token colors;
- [`Themes`] Added `Nadir` sub-theme, with extra cold gray background, flatten colors, low UI contrast, and ultra-desatured token colors;
- [`Themes`] Change `Open a remote window` button colors (background and foreground);
- [`Themes`] Added/Changed some skin main colors;
- [`Development`] Some improvements to the README.md output;
- [`Development`] The assignment of some relative colors has been revised;
- [`Development`] Added selection menu to go to UI preview on the page and on page reload, to better recognize the impact of the changes applied to the skin;
- [`Development`] Improved function for UI colors override: now is possible to override main colors and apply transformations o apply only transformations without override;
- [`Development`] Addedd lastest 3 (but number si customizable) changelogs to README.md.

## [1.1.100]

- [`Development`] Solved graphic issue with rendering of background in Find/Replace Widget (Fake UI for preview generator);
- [`Development`] Minor bug fix and optimizations: solved issue with placeholder of "vscode_marketplace_url" variable in `master-readme.md`.

## [1.1.99]

- [`Themes`] Added colors for some UI improvements introduced in **_Visual Studio Code_** `1.40.0`;
- [`Themes`] Added `EclipseDS` sub-theme, pretty faithful to `Eclipse DevStyle` theme, with extra cold gray background and more ultra-desatured token colors;
- [`Themes`] Restyled icon and added Cover to `README.md`;
- [`Themes`] After some UI colors revision, removed some sub-themes combo from `Anthracite`, `Low Blue` and `Midnight`, for similarity to the others skins;
- [`Themes`] Downgrade of **Visual Studio Code** minimum required version from `1.33` to `1.29` to evaluate-it in **Code-OSS** (VSCode for Raspberry Pi/Raspbian, that have an issue in versions later than 1.29 at this time);
- [`Development`] Minor bug fix and optimizations;
- [`Development`] Improved function to generate at one time themes based on multiple tokencolors;
- [`Development`] Implemented the function to generate theme based on my UI color with JSON file token colors export directly from VSCode (e.g. Dark+ wich not have an on TextMate equivalent version);
- [`Development`] Implemented the function to generate previews in GIF/PNG/JPG of VSCode UI tanks to [HTML2Canvas](https://html2canvas.hertzen.com/) library;
- [`Development`] Implemented the function to generate previews in HTML of VSCode UI (in order to obtain greater fidelity to the final result without testing everytime);
- [`Development`] Fix some issues of `VSCode Themes Master` in PHP 7.3.9.

## [1.1.94]

- [`Themes`] `Dark Matter` suite only: added `Anthracite` sub-theme, with extra cold gray background;
- [`Themes`] Deprecated `Zenburn Cold Gray` in favor of `Zenburn in Grays`;
- [`Development`] Added function for deprecate old themes that insert deprecation in favor of theme indicated;
- [`Development`] Short badge on `README.md`;
- [`Development`] Improved VSCode Themes Master UI PHP and JS functions to auto-unselect harmful build options after build theme/extension.

## [1.1.85]

- [`Themes`] Reintroduced `Midnight` sub-theme on certain combination of colors for all my skins;
- [`Development`] Added code based on array `excluded_combo` that can exclude some combinations of color variants in sub-theme for unsightliness or similarity to other skin due to filtering: basically i've excluded some skins based on cold colors from `Low Blue` sub-theme and some skins based on warm colors from `Midnight` sub-theme.

## [1.1.83]

- [`Themes`] Dark Matter only: added `Midnight` sub-theme inspired by _Telegram X Midnight Theme_. Appearance of `In Grays` and `Cold Gray` skins with `Midnight` background is unsightly;
- [`Development`] Added variable that overwrites the relative colors of the user interface with the relativized colors of the sub-theme for a better management of the color combination;
- [`Development`] Added code that get sub-theme descriptions and insert them in `README.md`;
- [`Development`] Added function that send Themes directly in VS Code Extensions Folder and Kill Reload VS Code executable for testing theme without debugging: this solve the issue to to select secondary skin twice before VS Code load her correctly.

## [1.1.79]

- [`Themes`] Improvements to some UI colors;
- [`Development`] Optimized some functions for themes generation;

## [1.1.71]

- [`Themes`] Added Nirvana sub-theme group, with a warm variation like Low Blue Light but only on token colors;
- [`Themes`] Improvements to some UI colors;
- [`Themes`] Fix some colors in themes skins and in Setting;
- [`Development`] Add the function that rebuild missing generic token colors scopes, obtaining them from the analysis of different TextMate Themes. This function also build a global token scopes dictionary for futures implementations;
- [`Development`] Optimized some functions for themes generation;
- [`Development`] Automated assignmet of all Token Colors Themes to Skins based on type (dark/light);
- [`Development`] Added function that convert existing TextMate Token Colors Themes in VSCode Token Colors and apply it to skins.

## [1.1.59]

- [`Themes`] Fix some colors in themes skins;
- [`Development`] Update UI of `VSCode Themes Master`;
- [`Development`] Fix some bugs in `VSCode Themes Master`.

## [1.1.54]

- [`Development`] Fix links in README.md.

## [1.1.53]

- [`Themes`] Colors of Explorer relativized to editor background color and not to active border / active tab (based on theme);
- [`Development`] Themes rebuilt with integration of some colors.

## [1.0.10]

- [`Themes`] Restyled icon;
- [`Themes`] Themes rebuilt using my `VSCode Themes Master` (a localhost PHP Script);
- [`Themes`] Addedd some skins;
- [`Themes`] Renamed some skins;
- [`Themes`] Modified colors of skins.

## [1.0.6]

- [`Themes`] Restyled icon.

## [1.0.2]

- [`Themes`] Restyled icon;
- [`Themes`] `Sugar Paper` inactive color more brighten;
- [`Themes`] Editor background color darkened.

## [1.0.1]

- [`Themes`] The prefix `$` for PHP variables is more visible;
- [`Themes`] `Asphalt` secondary color darkened.

## [1.0.0]

- [`Themes`] First release of `Zenburn Cold Gray Theme`.
