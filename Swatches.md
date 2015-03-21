Holds 6 hexagonal 'color slots', and a central cell where the color that is about to be picked is displayed.
Adjusting the ColorSliders changes the color in the currently active slot.

![http://wiki.gpick.googlecode.com/hg/images/swatches.png](http://wiki.gpick.googlecode.com/hg/images/swatches.png)

# Keys and Mouse #

  * `Space    ` add to palette, copy to clipboard and/or rotate swatch. The behaviour of this shortcut key is configured in Options dialog Picker tab.
  * `Left    ` Activate the slot before this one. ie. Move counterclockwise.
  * `Right    ` Activate the slot after this one. ie. Move clockwise.
  * `Leftclick    ` Activate the clicked-on swatch
  * `Drag from central cell    ` Activate floating color picker
  * `Drag from other cell    ` Drag a standard color, droppable on another cell, any color panel or in the [PaletteList](PaletteList.md).
  * `1-6    ` Activate one of the numbered slots.
  * `A    ` Add all colors to palette
  * `E    ` Edit the color in textual format, eg. "rgb(0, 176, 0)". Uses whichever format is chosen for Display in the 'Edit Converters' dialog.

# Tips #

  * Display filters only effect the colors displayed in the swatch, not the underlying color values which are used
> > when adding, copying, and pasting colors. Therefore if you want to add a filtered color to the palette, you can drag from the central cell
> > to any of the surrounding cells to add that cell. This is a normal color-picking operation, so be sure to end the drag
> > on an area which is blank color (rather than containing some of the pixels making up a digit 1-6)


# See also #

  * ColorPicker
  * ColorSliders