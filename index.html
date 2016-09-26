<!DOCTYPE html>
<meta charset="utf-8">
<style>

html, body {
  width: 100%;
  height: 100%;
}

.graticule {
  fill: none;
  stroke: #777;
  stroke-width: 0.5px;
  stroke-opacity: 0.5;
}

.land {
  fill: #424242;

}

.boundary {
  fill: none;
  stroke: none;
  stroke-width: 0.5px;
}

svg {
  background-color: #212121;
}

</style>
<body>
<script src="//d3js.org/d3.v4.0.0-alpha.50.min.js"></script>
<script src="//d3js.org/topojson.v1.min.js"></script>
<script>

var wrapper = d3.select("body")

var width   = wrapper.node().getBoundingClientRect().width,
height  = wrapper.node().getBoundingClientRect().height;

/*var width = 960,
    height = 480;*/

var projection = d3.geoEquirectangular()
    .scale(height / Math.PI)
    .translate([width / 2, height / 2]);

var path = d3.geoPath()
    .projection(projection);

/*var graticule = d3.geoGraticule();*/

var svg = d3.select("body").append("svg")
    .attr("width", width)
    .attr("height", height);

/*svg.append("path")
    .datum(graticule)
    .attr("class", "graticule")
    .attr("d", path);*/

d3.json("world-50m.json", function(error, world) {
  if (error) throw error;

  svg.insert("path", ".graticule")
      .datum(topojson.feature(world, world.objects.land))
      .attr("class", "land")
      .attr("d", path);

  svg.insert("path", ".graticule")
      .datum(topojson.mesh(world, world.objects.countries, function(a, b) { return a !== b; }))
      .attr("class", "boundary")
      .attr("d", path);
});

</script>
