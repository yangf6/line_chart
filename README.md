# multiChart.js API Reference

Line_chart that you could change line, area color

## Initialize

```javascript
var mychart = multiChart().x(function(d) { return formatDate.parse(d.date); })
                        .y(function(d) { return +d.price; })
                           .yLabel("temp");

var formatDate = d3.time.format("%b %Y");

d3.csv("data/sp500.csv", function(data) {
var chartWrapper = d3.select("#example")
.datum(data)
.call(mychart);
chartWrapper.datum(data).call(mychart)

```

## API Function


\#*chart*.**yLabel**(name)
>Assign the `name` to the Y axis


\#*chart*.**areaColor**(name)
>Assign the `name` to the color of the area

\#*chart*.**lineColor**(name)
>Assign the `name` to the color of the line

\#*chart*.**width(number)
>Adjust the `number` width to the chart

\#*chart*.**height(number)
>Adjust the `number` height to the chart

\#*chart*.**x (arr)
>refill the x axis with value

\#*chart*.**y = function(arr)
>refil the y axis with value
