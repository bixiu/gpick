There is a Variations dialog (available by rightclicking in the PaletteList)
and also a Variations panel (selectable as the Secondary Panel). They work differently.

# PaletteList context menu item #

![http://wiki.gpick.googlecode.com/hg/images/variations.png](http://wiki.gpick.googlecode.com/hg/images/variations.png)

  * `Drag : `Add individual colors to palette

Variations presents a `start,end `pair for each of lightness and saturation.
For each input color, `Steps `output colors are generated, blending between `start` and `end `values of Lightness and Saturation simultaneously.

How these are generated depends on the '**U**`se Multiplication`' checkbox.

When it's enabled,  the input color lightness and saturation is **multiplied** by the blend lightness and saturation;
Otherwise, the blend lightness and saturation is **added** to the input color lightness and saturation.

The start/end adjusters are configured to allow values above 1 and below 0; The former is necessary to allow multiplying to brighten/ saturate colors; the latter is necessary to allow addition to darken/desaturate colors.


# ToolPanel tool #

The 'Variations' panel available as a tool is rather different from the one you can access with a rightclick in the PaletteList.

![http://wiki.gpick.googlecode.com/hg/images/variations-tool.png](http://wiki.gpick.googlecode.com/hg/images/variations-tool.png)

The central column of four color areas comprises one special area at the top, and three ordinary color areas. Dropping a color on the topmost area loads that color into all 3 of the other slots.

In each of the three rows, the areas to the left cumulatively reduce the selected color component, while the areas to the right cumulatively increases the selected color component.
The strength of this effect is controlled by the slider labelled "Strength"

`Rightclick`ing on the central color will offer you (among other standard context-menu commands) the option to select which color component is varied in that row.

You may select between:
  * Hue (in HSL colorspace)
  * Saturation (in HSL colorspace)
  * Lightness (in HSL colorspace)
  * Lightness (in LAB colorspace)