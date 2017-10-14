# sharp11-jazz-parser

This module parses files in the .jazz format into [Sharp11 chart objects](https://github.com/jsrmath/sharp11/blob/master/docs/chart.md).  It was designed specifically for parsing the [iRb Jazz Corpus](https://musiccog.ohio-state.edu/home/index.php/iRb_Jazz_Corpus), the output of which is hosted in [sharp11-irb](https://github.com/jsrmath/sharp11-irb).  I made this parser as a quick-and-dirty solution for a particular project where I needed to parse the iRb corpus, so it is not yet feature complete.

# Usage
```
var jazzParser = require('sharp11-jazz-parser');
var chart;

chart = jazzParser.parseString(str); // Parse a string representation of a .jazz file
chart = jazzParser.parseFile(path); // Parse a .jazz file given a file path
```