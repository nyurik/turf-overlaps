# turf-ext-overlaps

find whether spatial features overlap


### `overlap(poly1, poly2)`

Takes two Linestring, Polygon or MultiPolygon features and finds whether they overlap.


### Parameters

| parameter | type    | description        |
| --------- | ------- | ------------------ |
| `poly1`   | Feature | the first Feature, containing LineString, Polygon or MultiPolygon geometry  |
| `poly2`   | Feature | the second Feature, containing LineString, Polygon or MultiPolygon geometry |


### Example

```js
var poly1 = turf.polygon([[
    [0, 0],
    [0, 2],
    [2, 2],
    [2, 0],
    [0, 0]
]]);

var poly2 = turf.polygon([[
    [1, 1],
    [1, 3],
    [3, 3],
    [3, 1],
    [1, 1]
]]);

var overlapping = overlaps(poly1, poly2);
```

## Tests

```sh
$ npm test
```

