# Super Awesome Vertical Timeline

**Timeline** shows a series of events in a vertically time-sorted structure.

Timeline utilizes a handful of super cool libraries, including [Tabletop.js](http://github.com/jsoma/tabletop) (for the data storage) and [Isotope](http://isotope.metafizzy.co/) for the layout.

A running example can be found [here](http://builtbybalance.com/github-timeline/).

## How to Use

### 1) Set up your data using Tabletop.js

Create a Google Spreadsheet with the following columns:
* title
* date
* display date
* photo url
* caption
* body 
* read more url

**Please note that the the _display date_ column must be in the format _Month day, Year_ (April 25, 2012) for proper javascript parsing.**
**Also, all columns must be _plain text_ format, including the two date columns.**

Now follow the instructions over at Tabletop.js to publish the Spreadsheet.

The Spreadsheet used in the example index.html file is at [https://docs.google.com/spreadsheet/ccc?key=0AsmHVq28GtVJdG1fX3dsQlZrY18zTVA2ZG8wTXdtNHc](https://docs.google.com/spreadsheet/ccc?key=0AsmHVq28GtVJdG1fX3dsQlZrY18zTVA2ZG8wTXdtNHc)

### 2) Insert the Spreadsheet key into script.js

Find your Spreadsheet key (see Tabletop.js for instructions), and replace the sample key on line 3 of `js/script.js` with the key to your Spreadsheet.

You also need to update the name of the spreadsheet 'sheet' that holds the data on line 4 of 'js/script.js'.

### 3) Enjoy!

## Bugs 

* None? Tested on Chrome, Firefox, Safari, & IE 7-9.

## Possible Improvements

* Turn this into a jQuery plugin.
* Remove hard coded Tabletop.js Spreadsheet key
* Remove hard coded `#timeline` element from script, and allow for multiple Timelines per page

## Credits

[Balance Media](http://www.builtbybalance.com) for the design and coding.

The following plugins/libraries are used:
[jQuery](http://jquery.com/), [Isotope](http://isotope.metafizzy.co), [Tabletop.js](http://github.com/jsoma/tabletop), [Handlebars.js](http://handlebarsjs.com/), [jQuery imagesLoaded plugin](http://github.com/desandro/imagesloaded), and [jQuery resize event](http://benalman.com/projects/jquery-resize-plugin/)

NOTE: All of the elements are free for non-commercial use. Commercial use of [Isotope](http://isotope.metafizzy.co) requires a $25 [license](http://metafizzy.co/#isotope-license).