# arctica
![Arctica's refined color set](colors.bmp)

Nord theme, but better.

Arctica seeks to be entirely aesthetically compatible with Nord, but to have a much better implementation, with colors added and dropped as needed.

## Why?
The Nord theme is ridiculously disorganized and the documentation is nonsensical. While the colors are great, it becomes a herculean effort to neatly integrate them into stuff.

### Highlighting Conflicts
For example, the [documentation states](https://www.nordtheme.com/docs/colors-and-palettes#nord2) that `nord2`, an "Even more brighter shade color of `nord0`" (Grammar 100) should be used both for highlighting text, *and* coloring the active line. The issue with this ridiculous approach is that the text selection becomes invisible on the currently selected line. This makes editing impossible. Strangely, this idiotic advice was actually implemented in the gedit theme, and probably a lot of other themes.

### The Forbidden Nord -1
On the [Nord theme website](https://nordtheme.com), you can experience a forbidden Nord color in the site background by clicking on the crescent moon to switch to dark mode. (What *is* a CSS media query, anyway?). The color is darker than `nord0`. Perhaps dark mode is off by default on the site in an attempt to hide this intriguing color. I think it should be added as the 17th color and named `nord -1`.

### Imbalanced Dark/Light Colors
On second thought, it shouldn't. Why? Well, it seems that in an effort to keep the palette 16 colors long, Arctic Ice Studios had to include 4 dark colors, and only 3 light colors. This is bizarre, because when reading through the documentation, it seems as if they intended Polar Night and Snowstorm to  be equivalents of eachother, to be used for dark mode and light mode respectively. Unfortunately, since the colors are imbalanced 4:3 (5:3 if you count `nord -1`) they're not exactly hot swappable.

### The Nord Theme Blues
What they couldn't do for the white colors, Arctic Ice Studios certainly made up for in the blues! [Frost](https://www.nordtheme.com/docs/colors-and-palettes#frost), the "heart palette of Nord", is composed of *four* slightly different shades of blue. While they are all clearly distinct colors, did we really need all of them? *Did we?*

### What About Terminals?
This issue is rather simple. Terminals want 16 colors, only 4 of those being gray/white/black. Nord does not have dark versions of the aurora colors, thus not enough colors to theme a terminal.

### Conclusion
This is nothing short of tragic, because Nord is probably one of the most aesthetically pleasing color palettes in existence.

Thus, this project.

---

## Polar Midnight
A implementation of the original Polar Midnight colors, this time starting in a deeper key. Designed to be entirely equivalent to Arctica's own Snow Storm.

### Arctica 0
`2B303C`

Background, equivalent to Arctica 7

#### Dark themes
* As a background
* As a shadow
* Rarely, to break up lighter colors

#### Light themes
* Do not use this color in light themes

### Arctica 1
`2e3440`

Secondary background, equivalent to Arctica 6

#### Dark themes
* As a secondary background
* To break up lighter colors

#### Light themes
* As text, icons, etc

### Arctica 2
`3b4252`

Lifted background, equivalent to Arctica 5

#### Dark themes
* For lifted elements, such as popups, some buttons/inputs, etc
* For highlighting the current line

#### Light themes
* Can be used for text, icons, etc with less prominence, but it is recommended that Arctica 3 be used for this purpose

### Arctica 3
`4c566a`

Highlight, equivalent to Arctica 4

#### Dark themes
* For text highlighting/selecting
* To denote selection in general

#### Light themes
* Text, icons, etc with less prominence