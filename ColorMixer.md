Applies a single color to 3 input colors, generating 3 output colors.

This can be useful for matching colors to a theme (eg. applying overall shadow and light colors)

![http://wiki.gpick.googlecode.com/hg/images/color-mixer.png](http://wiki.gpick.googlecode.com/hg/images/color-mixer.png)

# Options #

  * 3 input colors
  * Overlay color: the color which is applied using a 'layer mode'
  * Application mode: One of **Normal**, **Multiply**, **Add**, **Difference**, **Hue**, **Saturation**, **Lightness**

# Actions #

  * All the standard ColorPanel actions are supported.

# Examples #

![http://wiki.gpick.googlecode.com/hg/images/color-mixer-e1.png](http://wiki.gpick.googlecode.com/hg/images/color-mixer-e1.png)
![http://wiki.gpick.googlecode.com/hg/images/color-mixer-e2.png](http://wiki.gpick.googlecode.com/hg/images/color-mixer-e2.png)
![http://wiki.gpick.googlecode.com/hg/images/color-mixer-e3.png](http://wiki.gpick.googlecode.com/hg/images/color-mixer-e3.png)

# Mixing a color from 3 or more input colors #

To get a weighted mix of N colors, you can perform consecutive mixes.
For example, supposing you want a 33%, 33%, 33% mix of colors A B C:

  * First generate an A+B 50% mix . We'll call this [R0](https://code.google.com/p/gpick/source/detail?r=0), and drag it back to one of the input panels for mixing in the next step.
  * Then generate an [R0](https://code.google.com/p/gpick/source/detail?r=0)+C mix (33%, which means 66% [R0](https://code.google.com/p/gpick/source/detail?r=0), 33% C) into the palette. This is the final color.

This can be generalized to mix however many colors you want. GPick stores colors internally in floating point format,
so there is no noticable loss of accuracy from the multiple operations.

More examples (numeric precision is limited for the sake of brevity):

  * 33% A, 16% B, 50% C :  (A + 33% B) + 50% C   (ie. overall A amount = 66 **.5 = 33, B amount = 33** .5 == 16)
  * 50% A, 25% B, 12.5% C, 12.5% D :  ((C + 50% D) + 50% B) + 50% A   (overall C amount and D amount = 50 **.5** .5 == 12, B amount = 50 **.5 == 25)
  * 10% A, 60% B, 30% C :  (A + 85% B) + 30% C   (overall A amount = 14** .7 == 10, B amount = 85 **.7 == 60)
  * 25% A, 25% B, 25% C, 25% D :  (A + 50% B) + 50% (C + 50% D)   (overall A,B,C,D amounts = 50** .5 == 25)
  * 33% A, 33% B, 33% C :  (A + 50% B) + 33% C   (overall A,B amounts = 50 **.66 == 33)
  * 10% A, 20% B, 30% C, 40% D:  (A + 66% B) + 70% (C + 57% D)   (overall A amount = 33** .3 == 10, B = 66 **.3 == 20, C = 42** .7 == 30, D = 57 **.7 == 40)**

From these examples, you may have understood that this method is based on nesting partitions, as in:

  * 50% [50% B, [50% C, 50% D]], 50% A
    * 50% [50% B, [50% C, 50% D]], 50% A  is equivalent to 50% A, 25% B, 12% C, 12% D (the second example listed above)
      * Proof: 50 **.5 (ie. B) = 25; 50** .5 **.5 (ie. C, D) = 12.**


# See Also #

  * [MixColors](MixColors.md) : Generate blends between each of an arbitrary number of colors.
  * [BlendColors](BlendColors.md) : Generate blends with context.