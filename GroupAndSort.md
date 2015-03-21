Group and Sort groups colors according to similarity in the channel you choose, and then sorts each group.
As with [MixColors](MixColors.md), [Generate](Generate.md), and [Variations](Variations.md), shows a realtime preview of the result.

If you have used a recent version of the GIMP Palette Sort plugin, the idea is very similar; the main difference is that GIMP's Palette Sort uses 'partitioning', which finds contiguous blocks of the palette which have similar values in the specified channel, whereas GPick uses 'grouping', which selects all of the colors in the palette, contiguous or not, which have similar values in the specified channel. The difference is very much like the difference between Fuzzy Select tool and Select By Color in GIMP; GIMP's palette sort finds local groups, GPick's Group and Sort finds global groups.

# Configuration #

![http://wiki.gpick.googlecode.com/hg/images/group-and-sort.png](http://wiki.gpick.googlecode.com/hg/images/group-and-sort.png)

Several options are available:

  * **Group type** controls which channel the colors are grouped by. It can be set to _None_ (meaning no grouping is done; the selection is sorted as if it were a single big group), or any of the channels _R G B H S L L A B L C H_, or _RGB Greyscale_ (which uses the average of the R G B values)
  * **Grouping sensitivity** controls the threshold of similarity; how similar two colors have to be in terms of the selected channel, in order to be considered part of the same group. Less sensitivity results in bigger groups. It's expressed as a percentage of the gamut of the channel specified by _group type_.
  * **Maximum number of groups** sets an upper bound on the number of groups created. If more groups than this are found, the groups that are most similar are merged until there are only this many groups.
  * **Sort type** controls the sorting within each group. It has all the same options as _Group type_ , except _None_ is not available.
  * You have the option to **Reverse group order** and/or **Reverse order inside groups**.
    * **Reverse group order** controls in what order the groups are returned - for example if you are grouping by Red, the first group will be the one with the lowest overall Red value, but if _Reverse group order_ is checked, it will instead be the group with the highest overall Red value.
    * **Reverse order inside groups** has a similar effect on the main sorting: if you are sorting on Green, the group will be sorted from the color with highest Green value to the color with the lowest Green value, rather than vice versa.

  * PLACEHOLDER (Is the sort stable? we should note whether the sort is stable or not here.)

# See Also #

  * `Reverse` command in PaletteList context menu : reverse the ordering of the entire selection.