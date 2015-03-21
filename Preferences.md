# _Main #
  * **S**`ingle Instance    `Invoking GPick while there is already a GPick instance running will have no effect (another GPick instance will not be created.).  Useful in conjunction with the 'System Tray' options
  * `Save / `**R**`estore palette    `Automatically load from ~/.config/gpick/autosave.gpa when invoked with no parameters, and save to ~/.config/gpick/autosave.gpa at exit._

## System Tray ##
  * **M**`inimize to system tray    `When the GPick window is minimized, it becomes a system tray icon
  * **C**`lose to system tray    `When the GPick window is closed, it becomes a system tray icon
  * **S**`tart in system tray    `Send GPick to the system tray as soon as it is launched.

**NOTE:** You can pick colors and add them to your palette even with GPick in its system-tray state.
Just click and drag on the GPick icon, moving to wherever you want to pick from. This will show the [floating color picker](ColorPicker.md). It's also convenient to
use the measuring function (`M`, `Ctrl+M`) via this method.

# _Picker #_

## Display ##
  * **R**`efresh Rate    `How often the zoom area is updated. Default 15hz, ie. 15 times per second.
  * `Magnified area si`**z**`e    `Size in pixels of the zoom area (the area where a zoomed display of the area around the mouse is shown).

## Floating picker color behaviour ##
  * **A**`dd to palette`
  * `Co`**p**`y to Clipboard`
these options are as described in the "'Spacebar' button behaviour" section below, except that they occur when you have just used the **floating** colorpicker.

## 'Spacebar' button behaviour ##

`Space` can be used to quickly pick multiple colors. After the picking occurs, there are three actions
that may be automatically taken, according to whether they are enabled in the preferences:

  * `A`**d**`d to palette    ` Add the eyedropped color to the palette.
  * `Cop`**y**` to Clipboard    ` Copy the color to the clipboard in textual format (according to the format of the first converter with 'Copy' enabled)
  * `Rotate s`**w**`atch    ` After storing the color in the active swatch slot, make the next slot active. This helps you to quickly test various color schemes — just hit Space to grab this color and go to the next, repeatedly. Remember you can apply the picker to GPick's window too — this means you can quickly test rearrangements of a color scheme already in your palette.

## Enabled color spaces ##

Determines which sets of sliders are available in the main color picker panel
Currently the following color spaces are supported:
  * CMYK
  * HSL
  * HSV
  * LAB
  * LCH
  * RGB

If you have no use for one or more of these, you can disable them; The slider will then be absent from the color picker panel.

## Lab settings ##

Controls the **I**`lluminant `and **O**`bserver` used when transforming from/to LAB colorspace.
Common settings are D50, 2 or D65, 2.
If you don't know what this setting does, chances are you don't need to change it.

## Other settings ##

  * **M**`ask out of gamut colors    `Limits the colors shown in the LCH and LAB color selectors to the sRGB gamut. Areas outside gamut are shown as black and white stripes.

# _Color Names #_

  * **I**`mprecision postfix    `When auto-choosing a name for a color, add "~" to the end if the match is not exact.
  * Tool color naming: When adding colors to the palette from the various tools (see [ToolPanel](ToolPanel.md) and [PaletteList](PaletteList.md)), how are the color names set?
    * **E**`mpty    `(blank name)
    * **A**`utomatic Name    `(Match the color to a name using GPick's database of named colors)
    * **T**`ool specific    `(A name specific to the tool, for example "Pompadour 25 mix 75 Firebrick")