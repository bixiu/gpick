Generates color blends based on 3 input colors. Unlike 'Mix colors', this provides enough context to
get an accurate preview of how a color ramp will work overall (for example, if it's made up of 4 individual 'blends'; you
want to see how the ramp you're working on fits with the next segment.)

![http://wiki.gpick.googlecode.com/hg/images/blend-colors.png](http://wiki.gpick.googlecode.com/hg/images/blend-colors.png)

# Options #

  * `Start`, `Middle`, and `End` colors: The waypoints making up the color blend
  * `Start steps` : how many intermediate colors to calculate between Start and Middle (including Middle, so steps=2 produces 1 intermediate color)
  * `End steps` : how many intermediate colors to calculate between Middle and End (including End)
  * `Type` : Blending type. Identical to the Type found in [MixColors](MixColors.md)

# Actions #

  * The `Middle` panel has a 'Reset' action available in context menu which resets it to a 50% mix of Start and End.
  * Preview supports all the standard ColorPanel actions.

# Examples #

![http://wiki.gpick.googlecode.com/hg/images/blend-colors-e1.png](http://wiki.gpick.googlecode.com/hg/images/blend-colors-e1.png)
![http://wiki.gpick.googlecode.com/hg/images/blend-colors-e2.png](http://wiki.gpick.googlecode.com/hg/images/blend-colors-e2.png)
![http://wiki.gpick.googlecode.com/hg/images/blend-colors-e3.png](http://wiki.gpick.googlecode.com/hg/images/blend-colors-e3.png)

# See Also #

  * [MixColors](MixColors.md) : Generate blends between each of an arbitrary number of colors.
  * [ColorSliders](ColorSliders.md) : Includes a description of the differences between the colorspaces you can choose for Type.