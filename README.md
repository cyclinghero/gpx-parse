ch-gpx-parse [![NPM Version](https://badge.fury.io/js/ch-gpx-parse.png)](https://badge.fury.io/js/ch-gpx-parse) ========

A library for parsing gpx data. Forked from https://github.com/elliotstokes/gpx-parse

#Installation

	$ npm install ch-gpx-parse

#Or with bower

	$ bower install ch-gpx-parse

#Usage

The module has been designed to work within node but you can also use it on the client side using the browserfy version that can be found in the dist folder.

```javascript
var gpxParse = require("gpx-parse");

//from file
gpxParse.parseGpxFromFile("/path/to/gpxFile", function(error, data) {
	//do stuff
});

//or from string
gpxParse.parseGpx("<gpx></gpx>", function(error, data) {
	//do stuff
});

// or an external file via HTTP(S)
gpxParse.parseRemoteGpxFile("http://host.tld/my.gpx", function(error, data) {
    //do stuff
});

```

#Tests

Tests are written with nodeunit. To test make sure you have the dev dependencies installed and just run:

	$ npm test
