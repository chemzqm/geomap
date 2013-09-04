
# geomap

  svg geomap using jquery and raphael

  DEMO: <http://xbingoz.com/demo/geomap/>

## Installation

  Install with [component(1)](http://component.io):

    $ component install chemzqm/geomap

## API

## Example

``` js
var Geomap = require('geomap');
var $ = require('jquery');
var map = new Geomap({
  //指定地图渲染位置
  container: '#map',
  mapStyle: {
    stroke: '#fff'
  },
  //指定横纵缩放比
  scale: {
    x: 9,
    y: 9
  }
});
$.ajax({
  url: '/china-province.geojson',
  dataType: 'json'
}).done(function(json) {
  map.load(json);
  map.render();
});
```

## License

  MIT
