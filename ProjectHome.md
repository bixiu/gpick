**Gpick** is an advanced color picker.

![http://wiki.gpick.googlecode.com/hg/images/main-page-gpick-screenshot.png](http://wiki.gpick.googlecode.com/hg/images/main-page-gpick-screenshot.png)

## Get Gpick ##
[![](http://wiki.gpick.googlecode.com/hg/images/get-gpick.png)](http://code.google.com/p/gpick/wiki/Installing)

  * Version 0.2.5 has been released
  * Updated Debian packages released
  * Updated source tarball

## On the web ##
A very nice article by Alexandre Prokoudine, describes almost all Gpick functionality http://libregraphicsworld.org/articles.php?article_id=31

## Screenshots ##
http://picasaweb.google.com/thezbyg/GpickScreenshots?feat=directlink

## Features: ##
  * Create palettes from images
  * Color scheme creation tools
  * Fast color picking
  * Magnification
  * Colors automatically named
    * Closest color name is found using CIE94 color difference function, which is closer to the way humans interpret color differences, than difference of red, green and blue color amounts
  * Export to following formats
    * Inkscape/Gimp Palette (`*.gpl`)
    * Adobe Swatch Exchange (`*.ase`)
    * Alias/WaveFront Material (`*.mtl`)
  * Import from following formats:
    * Inkscape/Gimp Palette (`*.gpl`)
    * Adobe Swatch Exchange (`*.ase`)
  * Picked colors can be copied to clipboard in multiple formats
    * Hexadecimal notation - #rrggbb
    * Functional RGB notation - rgb(red, green, blue)
    * Functional HSL notation - hsl(hue, saturation, lightness)
    * Custom conversions can be done, but requires some [Lua](http://www.lua.org/) language knowledge
  * Oversampling with five falloff types
    * Multiple pixel values are averaged to help picking colors from sources with noise, patterns and etc, where each pixel is different and overall color is produced by different amounts of particular color
  * Mix two or more colors using variable number of steps and different mixing types
  * Create lightness and/or saturation variations
  * Create harmonious colors
  * Create color schemes

_Note: some of listed features may only be available in current version from Mercurial repository_

## Contribution: ##
If you have an idea how I or you could improve this project, don't hesitate, contact me using my email address, join discussion at [mailing-list](http://groups.google.com/group/gpick) or add an issue. Your ideas and feedback is highly appreciated.

## Bugs & Features ##
File bugs & feature enhancements using the 'Issues' tab above, you will need a google.com account (gmail accounts work as well). If you do not have one, you can sign up for one, or you can send bugs directly to me : thezbyg\_AT\_gmail\_DOT\_com.

## Source ##
The latest source is available from the 'Source' tab above. Also, you can browse the latest sources [online](http://code.google.com/p/gpick/source/browse/)

&lt;wiki:gadget url="http://www.ohloh.net/p/481069/widgets/project\_users.xml?style=blue" height="100" border="0"/&gt;
&lt;wiki:gadget url="http://www.ohloh.net/p/481069/widgets/project\_partner\_badge.xml" height="53" border="0"/&gt;