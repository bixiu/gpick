A panel shown below the main panel, containing a selectable color generation tool.
Depending on the size and arrangement of the GPick window, may include a scrollbar.

Most tools have context-menu items in common:

  * **A**`dd to palette` (equivalent to doubleclicking on the color)
  * `A`**d**`d All to palette`
  * **C**`opy to Clipboard`

##### Configuration #####

Allows you to select which dialog is shown in this panel:

Historical versions of GPick have a 'View' menu directly above the [ToolPanel](ToolPanel.md) for this purpose.
Newer versions move this into the main 'View' menu as the 'Secondary View' submenu.

Available tools:
  * None (`Shift+Ctrl+N`): Useful if you don't use the ToolPanel and want to save space.
  * [Blend Colors](BlendColors.md) (`Shift+Ctrl+B`): Generate a gradient from 3 end-points. The number of steps A->B and B->C are individually adjustable
  * [Brightness Darkness](BrightnessDarkness.md) (`Shift+Ctrl+D`): Generate 4 brighter and 4 darker shades; the contrast in the 'darker' and 'brighter' ranges is individually adjustable.
  * [Color Mixer](ColorMixer.md) (`Shift+Ctrl+M`): Apply a color to <=3 base colors using a "layer blending mode"
  * **Scheme Generation** (`Shift+Ctrl+G`): Exactly the same as the [Scheme Generation](SchemeGeneration.md) tab. Since this is a separate dialog, both can be shown at once with individual settings, so it's possible to compare generated schemes quickly.
  * **Layout Preview** (`Shift+Ctrl+L`): Exactly the same as the [Layout Preview](LayoutPreview.md) tab. Since this is a separate dialog, both can be shown at once with individual settings, so it's possible to compare layouts quickly.
  * [Variations](Variations.md) (`Shift+Ctrl+V`): More flexible and interactive version of the Variations generator that you can access in the [PaletteList](PaletteList.md).
