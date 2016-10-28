# ZedGraph #

This is a fork of https://github.com/saleyn/ZedGraph.git

The original project is LGPL copyrighted 2004-2009 by John Champion.
https://sourceforge.net/projects/zedgraph/

In this fork we had to make some custom changes for specific needs that come from our use case of MS-proteomics.
Especially we addressed the issue of high-range line plot data.
The original ZedGraph library had some hard restrains regarding "outragous" coordinates (for line plots these where +/- 5000000 for lines and +/- 1000000 for areas).
Allowing such high coordinate boundaries caused some serious performance issues in some of our default plots where we applied a default zoom to a small sub-section of the entire
Line plot.

## Added features ##

* Area Clipping in line plots if line exits the chart drawing area (instead of hard boundary +/- 1000000)
* Line interpolation for line plots if line exits the chart drawing area (instead of hard boundary +/- 5000000)


## Maintainer ##

Oliver Bernhardt
(https://github.com/oBernhardt/BGS-Modified-ZedGraph)

## LICENSE ##

LGPL v2.1

