# File #

  * **N**`ew    ` Start a new palette. Note that this does not prompt you if you want to save, if changes were made; so make sure you saved at an appropriate point.
  * **O**`pen    ` Open a palette in GPA, GPL, or ASE format.
  * `Re`**v**`ert    ` Revert to the most recently saved version of this palette.
  * **S**`ave`and`Save `**A**`s    ` Save the palette in GPA, GPL or ASE format.
  * `Ex`**p**`ort    ` exports the entire palette in GPA, GPL, MTL or ASE format.
  * `Expo`**r**`t Selection    ` is like `Ex`**p**`ort `, but it only exports the selected colors.
  * **I**`mport    ` reads in the contents and //appends// it to the active palette (compare with **O**`pen`, where the content replaces the current palette)
  * **Q**`uit    ` There would be no need to explain this, except for the fact that GPick supports (since 0.2.5) '**auto-save/load**'. On quitting, the current palette is saved to` autosave.gpa` inside the `~/.config/.gpick `directory in your home dir, if the appropriate option in [Preferences](Preferences.md) is enabled.

# Edit #

  * `Edit `**C**`onverters    ` Configure the formats used by color info and 'Copy to Clipboard'
  * ![http://wiki.gpick.googlecode.com/hg/images/editconverters.png](http://wiki.gpick.googlecode.com/hg/images/editconverters.png)
    * 1. You can reorder the list by dragging.
    * 2. Controls which format is used to display color info (found in the [ColorInfo](ColorInfo.md) display and various large color panels) and represent colors when copying to text format.
    * 3. Controls which format is used to describe a color in the [PaletteList](PaletteList.md).
    * 4. Checking the 'Copy' column shows this item in the [PaletteList](PaletteList.md) `Copy to Clipboard` context submenu. First item with 'Copy' enabled is used when the `Ctrl+C` `Copy to Clipboard` shortcut is invoked.
    * 5. Checking the 'Paste' column tells the Paste command to accept pastes in this format.
  * `Display `**F**`ilters`
    * This dialog allows you to adjust the display of colors according to filters.
    * It's pretty straightforward. You can add, remove, or reorder filters, and adjust their parameters by doubleclicking on a filter. Newly added filters appear at the end.
    * The available filters are demonstrated in [DisplayFilters](DisplayFilters.md)
    * You can also toggle whether the filter stack is active or not.
    * All flat color areas except the ones in the [PaletteList](PaletteList.md) are affected. [ColorSliders](ColorSliders.md) and the [ColorWheel](ColorWheel.md) are not affected.
    * Shortcuts:
      * `Delete    ` Remove the currently selected filter
      * `Enter     ` Show configuration for currently selected filter

  * **P**[references](Preferences.md)

# View #
  * **P**`alette    ` Toggle the visibility of the [PaletteList](PaletteList.md) (`Ctrl+Shift+P`)
  * In newer versions of GPick, the '**S**`econdary View`' submenu is also found here, which allows you to choose which tool appears in the [ToolPanel](ToolPanel.md) :
    * None `Shift+Ctrl+N`
    * Blend colors `Shift+Ctrl+B`
    * Brightness Darkness `Shift+Ctrl+D`
    * Color mixer `Shift+Ctrl+M`
    * Scheme generation `Shift+Ctrl+G`
    * Layout preview `Shift+Ctrl+L`
    * Variations `Shift+Ctrl+V`

# Tools #
  * `Palette from `**i**`mage`
    * ![http://wiki.gpick.googlecode.com/hg/images/palettefromimage.png](http://wiki.gpick.googlecode.com/hg/images/palettefromimage.png)
    * Builds a palette from an image file using the median cut algorithm in XYZ colorspace.
    * Responds to adjustment of the Colors setting in real-time.
    * Note that the generated palette is appended to the current palette; it does not replace it.
    * After importing a palette, you may want to arrange it with the help of [GroupAndSort](GroupAndSort.md)

# Help #
  * This document is not recursive ;)
