Generate a color scheme from a base color.

![http://wiki.gpick.googlecode.com/hg/images/generate-scheme.png](http://wiki.gpick.googlecode.com/hg/images/generate-scheme.png)

This demo image shows both colorscheme generation panes: The primary one, accessible via the tabbed
interface, and the secondary one, selectable via the View->Secondary View [Menu](Menu.md). These are identical in function.

More commonly you would have a different type of tool in the top and bottom panes; this setup was just for illustrative purposes.
The number of colors generated depends on what `Type` of scheme you select.

# Options #

  * `Hue`, `Saturation`, and `Lightness` allow you to directly modify the base color using the HSL color model.
  * `Type` is the most important option, it specifies what kind of colorscheme you want:
    * _Complementary_ generates the original color and the color opposite on the colorwheel (+180 degrees):
      * ![http://wiki.gpick.googlecode.com/hg/images/generate-complementary.png](http://wiki.gpick.googlecode.com/hg/images/generate-complementary.png)
    * _Analogous_ generates the original color and a set of 5 colors spaced 30 degrees apart. Therefore, the last color (30 **5 == 150 degrees offset from the start color) is 30 degrees away from the Complementary color (+180 degrees)
      * ![http://wiki.gpick.googlecode.com/hg/images/generate-analogous.png](http://wiki.gpick.googlecode.com/hg/images/generate-analogous.png)
    * _Triadic_ generates the original color and the other two points in the 'triangle' (spaced 120 degrees apart).
      * ![http://wiki.gpick.googlecode.com/hg/images/generate-triadic.png](http://wiki.gpick.googlecode.com/hg/images/generate-triadic.png)
    * _Split-Complementary_ generates the original color and the two colors spaced 30 degrees away from the complementary color (+180 degrees). So the second and third colors are at +150 degrees and +210 degrees respectively.
      * ![http://wiki.gpick.googlecode.com/hg/images/generate-splitcomp.png](http://wiki.gpick.googlecode.com/hg/images/generate-splitcomp.png)
    * _Rectangle (Tetradic)_ generates the original color and the remaining 3 colors in the set, positioned at +60, +180, and +240 degrees respectively. Overall these form two pairs of colors in which the distance between the members of each pair is 60 degrees, but the pairs are spaced 120 degrees apart.
      * ![http://wiki.gpick.googlecode.com/hg/images/generate-rectangle.png](http://wiki.gpick.googlecode.com/hg/images/generate-rectangle.png)
    * _Square_ generates the original color and the other three points in the 'square' (spaced 90 degrees apart).
      * ![http://wiki.gpick.googlecode.com/hg/images/generate-square.png](http://wiki.gpick.googlecode.com/hg/images/generate-square.png)
    * _Neutral_ generates the original color and a set of 5 colors spaced 15 degrees apart.
      * ![http://wiki.gpick.googlecode.com/hg/images/generate-neutral.png](http://wiki.gpick.googlecode.com/hg/images/generate-neutral.png)
    * _Clash_ generates the original color, a color at +90 degrees, and a color at -90 degrees. In other words, the original color and a complementary pair at +90 degrees.
      * ![http://wiki.gpick.googlecode.com/hg/images/generate-clash.png](http://wiki.gpick.googlecode.com/hg/images/generate-clash.png)
    * _Five-tone_ generates the original color and a set of 4 colors spaced 45 degrees apart beginning at +115 degrees
      * ![http://wiki.gpick.googlecode.com/hg/images/generate-5tone.png](http://wiki.gpick.googlecode.com/hg/images/generate-5tone.png)
    * _Six-tone_ generates 3 sets spaced 120 degrees apart, containing 2 colors spaced apart 30 degrees, including the original color.
      * ![http://wiki.gpick.googlecode.com/hg/images/generate-6tone.png](http://wiki.gpick.googlecode.com/hg/images/generate-6tone.png)
    * As to which is most appropriate, each have different visual effects and it's quite an involved subject. To get the most out of color scheme generation, it helps to educate yourself about [Color Theory](http://en.wikipedia.org/wiki/Color_Theory)
  * `Color wheel` allows you to select which color wheel to calculate the schemes using
    * `RGB` color wheel models the way light mixes, and is the usual choice for digital art. All of the screenshots above show an RGB wheel.
    * `RYB` color wheel models the way paint mixes. Traditional painters use this kind of color wheel.
    * There are two versions of RYB. The first is closest to traditional color wheels; the second has more balanced distribution without extreme changes in brightness:
      * ![http://wiki.gpick.googlecode.com/hg/images/rybv1-colorwheel.png](http://wiki.gpick.googlecode.com/hg/images/rybv1-colorwheel.png)
      * ![http://wiki.gpick.googlecode.com/hg/images/rybv2-colorwheel.png](http://wiki.gpick.googlecode.com/hg/images/rybv2-colorwheel.png)**

# Actions #

  * All the standard ColorPanel actions are available.
  * `Drop color (on one of the color panels)` : Recalculate color scheme. You can drop the color on any of the color panels; the other panels will update correspondingly. If you want to change the 'direction' that the scheme generator travels in, if applicable, dropping the color on the final color panel will have this effect.

# See Also #

  * [Generate](Generate.md) : Generate color schemes for each of the selected palette colors.
  * [Wikipedia on Color Schemes](http://en.wikipedia.org/wiki/Color_scheme)