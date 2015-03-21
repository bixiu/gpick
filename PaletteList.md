The PaletteList is usually the rightmost pane in a GPick window, listing the colors in the palette,
1 per row. (multiple colors per row is planned, but not implemented yet.)
You can toggle its visibility by pressing `Ctrl+Shift+P` or via the `Palette` entry in the `View` menu.

Each row shows:

  * Color (visually)
  * Color (textual format, configured in "[Edit Converters](Menu.md)")
  * Name

Example PaletteList:

![http://wiki.gpick.googlecode.com/hg/images/palette-list.png](http://wiki.gpick.googlecode.com/hg/images/palette-list.png)

# Actions #

  * `DoubleClick    ` Set color in active [swatch](Swatches.md) slot to first of the selected colors
  * `1-6    ` Activate numbered [swatch](Swatches.md) slot and set it to the first of the selected colors
  * `Ctrl+1-6    ` Replace the first color of the selected colors with the color from the numbered [swatch](Swatches.md) slot
  * `Ctrl+A    ` Select all colors.
  * `Delete    ` Remove selected colors.
  * `Ctrl+C    ` Copy currently selected color into clipboard as text. Uses first enabled converter to convert colors. If multiple colors are selected, one line is produced for each color.
  * `Rightclick (context menu)    `:
    * ![http://wiki.gpick.googlecode.com/hg/images/palettelist-menu.png](http://wiki.gpick.googlecode.com/hg/images/palettelist-menu.png)
    * **C**`opy to clipboard    ` Copy currently selected color into clipboard as text. Uses first enabled converter to convert colors. If multiple colors are selected, one line is produced for each color. Equivalent to pressing `Ctrl+C`.
    * **M**[ix Colors](MixColors.md), **V**[ariations](Variations.md), and **G**[enerate](Generate.md) have their own pages.
    * **R**`emove `and `Remove `**A**`ll    ` remove the selected colors or all colors, respectively.
    * `C`**l**`ear names (E)    `, which empties the names of all selected colors,
    * `Auto`**n**`umber (A)    `, which prompts you for a name and either replaces or appends to the name, "NAME-NUMBER", eg 'Bricks-1', for every selected color.
      * The number is determined by index in the selection (so the 3rd selected item gets numbered 3, etc).
      * You can choose the number to start at (eg, if starting number is set to 9, the first selected color will be numbered 9)
      * You can also choose the width to zero-pad the numbers to. 2 is the default, which will format the numbers as 01..99..100...
      * Finally, you can choose whether the numbering will decrease or increase (ie. whether the numbering is like `foo03 foo02 foo01` or `foo01 foo02 foo03`
    * `Autona`**m**`e (N)    `, which sets the color name according to GPick's internal color-name database. This can be useful when the name is something un-memorable or entirely empty.  See also the [Preferences](Preferences.md) for settings relating to the default naming of colors generated by tools.
    * `R`**e**`verse (V)    `, which simply reverses the order of the the colors in the selection.
    * [Group and ](GroupAndSort.md)**S**[ort](GroupAndSort.md)` (G)    ` allows you to sort one or more groups in the palette.

  * You can press `E`, `A`, `N`, `V`, or `G` in the palette list to invoke the respective functions above, without needing to bring up the context menu.

  * `Drop    `Add color to list at pointer location. The color will be automatically assigned a name (eg 'Limeade') by matching it to a builtin list of color names.
  * `Drag,(Drop inside colorlist)    ` Copy one or more colors to another place
  * `Shift+Drag,(Drop inside colorlist)   ` Move one or more colors to another place.
  * `Ctrl+Drag,(Drop inside colorlist)   ` Replace the destination color with the source color.
  * **NOTE: Because Shift and Ctrl are used both for selection and dragging, what you usually want is to do the final click in your selection and hold it down and start the drag operation, rather than releasing the button and then doing the drag and drop in a separate motion. This is because otherwise you may end up changing the selection.**
  * In particular, when Ctrl+dragging a single color, you want to just click+drag immediately; otherwise the second click with Ctrl will deselect the color and nothing will happen because no colors are selected.
  * `Drag(+Drop outside colorlist)    ` Send color to target.
    * Possible targets:
      * An external application that accepts drops of colors. Only the first color in the selection will be sent, in this case.
      * An external application that accepts text. The color(s) will be sent in the format specified in the [Converter](Menu.md) configuration. Default is HTML-style hex codes (#RRGGBB).
      * A [swatch](Swatches.md) slot (only the first color in the selection will be used)
      * The PaletteList of another GPick instance
      * A color panel inside the [ToolPanel](ToolPanel.md) (only the first color in the selection will be used).