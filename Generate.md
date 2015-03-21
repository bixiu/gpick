For each color in the selection, generates a color scheme. Essentially an enhanced version of the SchemeGeneration ToolPanel / tab.

Here's an example with one color, hex code #7f7fff, selected; 3 colors are generated.
![http://wiki.gpick.googlecode.com/hg/images/generate.png](http://wiki.gpick.googlecode.com/hg/images/generate.png)

From the base color — which is always the first in the generated set — Color theory is used to calculate a set of related colors on the color wheel.
You have a choice of how many colors to generate — usually you want an amount that matches the 'Type' (eg 4 for Square, 3 for Triadic).

`Type `and `Color Wheel ` are explained in the SchemeGeneration page.

In addition, you have these options:
  * `Chaos    `Amount of randomness to introduce into the result. This only effects relative position on the color wheel.
  * `Seed    `Random seed used when calculating Chaos. Using the same seed allows you to get 'predictable randomness' — the same sequence of perturbations.
  * `Reverse    `Reverse the order of outputted colors (except for the base color)


# Examples #

With 3 colors selected (hex codes: #7f7fff #9d7a6c #6dbe00 ); 9 colors are generated.

![http://wiki.gpick.googlecode.com/hg/images/generate-3colors.png](http://wiki.gpick.googlecode.com/hg/images/generate-3colors.png)

Here's an example of the difference between using RGB and RYB color wheels;
RYB matches the color wheels used traditionally by painters. No other settings or input colors were changed.

![http://wiki.gpick.googlecode.com/hg/images/generate-3colors-ryb.png](http://wiki.gpick.googlecode.com/hg/images/generate-3colors-ryb.png)

# See Also #
  * The SchemeGeneration page covers the topic of generating color schemes in more detail, with several examples.