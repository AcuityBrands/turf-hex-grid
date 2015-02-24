# turf-hex-grid

[![build status](https://secure.travis-ci.org/Turfjs/turf-hex-grid.png)](http://travis-ci.org/Turfjs/turf-hex-grid)




### `turf.hex-grid(bbox, cellWidth, units)`

Takes a bounding box and a cell size in degrees and returns a FeatureCollection of flat-topped
hexagons (Polygon features) aligned in an "odd-q" vertical grid as
described in [Hexagonal Grids](http://www.redblobgames.com/grids/hexagons/)


### Parameters

| parameter   | type           | description                                             |
| ----------- | -------------- | ------------------------------------------------------- |
| `bbox`      | Array.<number> | bounding box in [minX, minY, maxX, maxY] order          |
| `cellWidth` | Number         | width of cell in specified units                        |
| `units`     | String         | used in calculating cellWidth ('miles' or 'kilometers') |


### Example

```js
var bbox = [7.2669410, 43.695307, 7.2862529, 43.706476];
var cellWidth = 0.2;
var units = 'miles';

var hexgrid = turf.hexGrid(bbox, cellWidth, units);

//=hexgrid
```

## Installation

Requires [nodejs](http://nodejs.org/).

```sh
$ npm install turf-hex-grid
```

## Tests

```sh
$ npm test
```


