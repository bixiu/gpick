The Color Sliders subpane mainly includes sliders which alter the color in the active [swatch](Swatches.md) slot. Exactly which colorspaces the sliders are shown for can be configured in the [Preferences](Preferences.md) ('Enabled color spaces' in the 'Picker' tab.)

A few secondary functions that this subpane performs are:
  * Allow you to tweak the color picker behaviour (radius to sample from, sample weighting falloff, and zoom level of the magnified display.)
  * Show the name of the nearest named-color in GPick's database of named colors.
  * Provide a panel to measure contrast (both visually and numerically)

![http://wiki.gpick.googlecode.com/hg/images/colorsliders.png](http://wiki.gpick.googlecode.com/hg/images/colorsliders.png)

# Adjust colors #

## Color models available ##

Not all of these may be shown, according to your selection in the [Preferences](Preferences.md) ('Enabled color spaces' in the 'Picker' tab.)


  * [RGB](http://en.wikipedia.org/wiki/RGB) : standard sRGB color model used for image data.
  * [HSV, HSL](http://en.wikipedia.org/wiki/HSL_and_HSV) : mapping of the RGB colorspace onto a cylinder. HSV correlates more predictably with RGB, while HSL is more predictable to the eye with regard to Saturation.
  * [CMYK](http://en.wikipedia.org/wiki/CMYK) : Naive print ink modelling. Naive because the characteristics of actual CMYK printers are more complex than simply 'overlapped inverse of RGB values'
  * [Lab](http://en.wikipedia.org/wiki/Lab_color_space) : Most 'perceptually predictable' color space available; Least vulnerable to incurring apparent hue, saturation, or lightness variation as a result of adjusting an unrelated component. However, not all valid Lab colors are valid RGB colors. In this screenshot, the 'mask out-of-gamut colors' option is turned on -- it shows a striped pattern in areas where the given Lab color is incompatible with RGB colorspace.
  * [LCH](http://en.wikipedia.org/wiki/LCH_color_space) : Like HSL is a polar transform of the RGB colorspace, this is a polar transform of the Lab colorspace. It has similar advantages to HSL: hue and vividness (called 'Chroma' in the LCH colorspace) are separately adjustable. As with Lab, some colors are not reproduceable in RGB, so be attentive.

## Sliders ##

  * `Click`ing or `drag`ging on a slider changes the color in the active swatch slot.
  * `Click`ing on either the numbers or the channel labels next to the sliders pops up a dialog where you can edit the exact values of the individual channels in that colormodel.
  * `Right Click`ing offers you the option of Copy or Paste (as well as the Edit function). Be aware that each color model has different characteristics, and copy/pasting between the sliders of different color models consequently may not do what you expect.

# Tweak color picker behaviour #

The following settings are available:
  * **Oversample**: what size area the color is measured over. Oversample = 0 gets the exact color of the single pixel under the pointer. Oversample = 1 measures the color over a 3x3 square, Oversample = 2 over a 5x5 square, etc.
  * **Falloff**: how the weight of each pixel in the sampled area decreases as it becomes more distant from the central pixel.
    * _None_ : Every pixel is equally weighted, no falloff occurs.
    * The other types, _Linear_, _Cubic_, _Quadratic_ and _Exponential_ are relatively self explanatory -- look at their icons:
      * ![http://wiki.gpick.googlecode.com/hg/images/falloff-types.png](http://wiki.gpick.googlecode.com/hg/images/falloff-types.png)
  * **Zoom**: the zoom level used in the ZoomArea and the floating color picker.

# Estimate contrast #

In the 'Info' section, there is a color panel with text overlaid, reading "Sample". Dropping a color onto this panel sets the panel color. The text color is determined by the color in the active swatch slot. Next to this, a percentage indicates how much contrast there is between the text and the background, as measured by the CIE94 color difference function.

# See Also #

  * [Swatches](Swatches.md)