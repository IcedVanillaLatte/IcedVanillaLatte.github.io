---
title: Air Quality at 2021-05-04 10:50:00
layout: single
permalink: /myairq/
---
### The Current Air Quality

<html xmlns="https://www.w3.org/1999/xhtml">
<head>
<title>MergedID3873c466e8b</title>
<meta http-equiv="content-type" content="text/html;charset=utf-8" />
<style type="text/css">
body {
  color: #444444;
  font-family: Arial,Helvetica,sans-serif;
  font-size: 75%;
  }
  a {
  color: #4D87C7;
  text-decoration: none;
}
</style>
</head>
<body> <!-- Table generated in R 3.5.2 by googleVis 0.6.4 package -->
<!-- Tue May  4 10:50:06 2021 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableID38731befb88f () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
24.11,
46.47,
1007.16,
655,
7.3,
4.3
] 
];
data.addColumn('number','Temperature (C)');
data.addColumn('number','Humidity (%)');
data.addColumn('number','Pressure (hPa)');
data.addColumn('number','CO2 (ppm)');
data.addColumn('number','PM10 (ug/m3)');
data.addColumn('number','PM2.5 (ug/m3)');
data.addRows(datajson);
return(data);
}


// jsData 
function gvisDataLineChartID38732ce9e58e () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,4,10,34,0),
23.35,
47.58
],
[
new Date(2021,4,4,10,43,0),
23.83,
46.89
],
[
new Date(2021,4,4,10,44,0),
23.88,
46.63
],
[
new Date(2021,4,4,10,45,0),
23.91,
46.62
],
[
new Date(2021,4,4,10,46,0),
23.96,
46.38
],
[
new Date(2021,4,4,10,47,0),
24,
46.48
],
[
new Date(2021,4,4,10,48,0),
24.04,
46.52
],
[
new Date(2021,4,4,10,49,0),
24.07,
46.53
],
[
new Date(2021,4,4,10,50,0),
24.11,
46.47
] 
];
data.addColumn('datetime','time');
data.addColumn('number','Temperature');
data.addColumn('number','Humidity');
data.addRows(datajson);
return(data);
}


// jsData 
function gvisDataAreaChartID3873304bc904 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,4,10,34,0),
1007.47,
"#9B59B6"
],
[
new Date(2021,4,4,10,43,0),
1007.26,
"#9B59B6"
],
[
new Date(2021,4,4,10,44,0),
1007.24,
"#9B59B6"
],
[
new Date(2021,4,4,10,45,0),
1007.3,
"#9B59B6"
],
[
new Date(2021,4,4,10,46,0),
1007.38,
"#9B59B6"
],
[
new Date(2021,4,4,10,47,0),
1007.39,
"#9B59B6"
],
[
new Date(2021,4,4,10,48,0),
1007.34,
"#9B59B6"
],
[
new Date(2021,4,4,10,49,0),
1007.23,
"#9B59B6"
],
[
new Date(2021,4,4,10,50,0),
1007.16,
"#9B59B6"
] 
];
data.addColumn('datetime','time');
data.addColumn('number','Pressure');
data.addColumn({type: 'string', role: 'style'});
data.addRows(datajson);
return(data);
}


// jsData 
function gvisDataAreaChartID387350b6e927 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,4,10,34,0),
625,
"#3DC948"
],
[
new Date(2021,4,4,10,43,0),
639,
"#3DC948"
],
[
new Date(2021,4,4,10,44,0),
642,
"#3DC948"
],
[
new Date(2021,4,4,10,45,0),
644,
"#3DC948"
],
[
new Date(2021,4,4,10,46,0),
648,
"#3DC948"
],
[
new Date(2021,4,4,10,47,0),
650,
"#3DC948"
],
[
new Date(2021,4,4,10,48,0),
651,
"#3DC948"
],
[
new Date(2021,4,4,10,49,0),
652,
"#3DC948"
],
[
new Date(2021,4,4,10,50,0),
655,
"#3DC948"
] 
];
data.addColumn('datetime','time');
data.addColumn('number','CO2');
data.addColumn({type: 'string', role: 'style'});
data.addRows(datajson);
return(data);
}


// jsData 
function gvisDataColumnChartID38731636cbf3 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,4,10,50,0),
7.3,
"#4E89F6"
] 
];
data.addColumn('datetime','time');
data.addColumn('number','PM10');
data.addColumn({type: 'string', role: 'style'});
data.addRows(datajson);
return(data);
}


// jsData 
function gvisDataColumnChartID38731c2c2333 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,4,10,50,0),
4.3,
"#4E89F6"
] 
];
data.addColumn('datetime','time');
data.addColumn('number','PM25');
data.addColumn({type: 'string', role: 'style'});
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartTableID38731befb88f() {
var data = gvisDataTableID38731befb88f();
var options = {};
options["allowHtml"] = true;
options["width"] = 600;


    var chart = new google.visualization.Table(
    document.getElementById('TableID38731befb88f')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartLineChartID38732ce9e58e() {
var data = gvisDataLineChartID38732ce9e58e();
var options = {};
options["allowHtml"] = true;
options["title"] = "Temperature and Humidity";
options["series"] = [{color:'#F6614E', targetAxisIndex:0},
                                  {color:'#4E89F6', targetAxisIndex:1}];
options["vAxes"] = [{title:'Temp. (C)'},{title:'Hum. (%)'}];
options["width"] = 600;


    var chart = new google.visualization.LineChart(
    document.getElementById('LineChartID38732ce9e58e')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartAreaChartID3873304bc904() {
var data = gvisDataAreaChartID3873304bc904();
var options = {};
options["allowHtml"] = true;
options["title"] = "Air Pressure";
options["vAxis"] = {title:'(hPa)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.AreaChart(
    document.getElementById('AreaChartID3873304bc904')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartAreaChartID387350b6e927() {
var data = gvisDataAreaChartID387350b6e927();
var options = {};
options["allowHtml"] = true;
options["title"] = "CO2 Level";
options["vAxis"] = {title:'(ppm)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.AreaChart(
    document.getElementById('AreaChartID387350b6e927')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartColumnChartID38731636cbf3() {
var data = gvisDataColumnChartID38731636cbf3();
var options = {};
options["allowHtml"] = true;
options["title"] = "PM 10";
options["vAxis"] = {title:'(ug/m3)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.ColumnChart(
    document.getElementById('ColumnChartID38731636cbf3')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartColumnChartID38731c2c2333() {
var data = gvisDataColumnChartID38731c2c2333();
var options = {};
options["allowHtml"] = true;
options["title"] = "PM 2.5";
options["vAxis"] = {title:'(ug/m3)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.ColumnChart(
    document.getElementById('ColumnChartID38731c2c2333')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "table";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartTableID38731befb88f);
})();
function displayChartTableID38731befb88f() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}


// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "corechart";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartLineChartID38732ce9e58e);
})();
function displayChartLineChartID38732ce9e58e() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}


// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "corechart";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartAreaChartID3873304bc904);
})();
function displayChartAreaChartID3873304bc904() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}


// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "corechart";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartAreaChartID387350b6e927);
})();
function displayChartAreaChartID387350b6e927() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}


// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "corechart";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartColumnChartID38731636cbf3);
})();
function displayChartColumnChartID38731636cbf3() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}


// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "corechart";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartColumnChartID38731c2c2333);
})();
function displayChartColumnChartID38731c2c2333() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID38731befb88f"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartLineChartID38732ce9e58e"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartAreaChartID3873304bc904"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartAreaChartID387350b6e927"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartColumnChartID38731636cbf3"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartColumnChartID38731c2c2333"></script>
 
<table border="0">
<tr>
<td>

<table border="0">
<tr>
<td>

<table border="0">
<tr>
<td>

<table border="0">
<tr>
<td>

<table border="0">
<tr>
<td>

<!-- divChart -->
  
<div id="TableID38731befb88f" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
<tr>
<td>

<!-- divChart -->
  
<div id="LineChartID38732ce9e58e" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
</table>

</td>
</tr>
<tr>
<td>

<!-- divChart -->
  
<div id="AreaChartID3873304bc904" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
</table>

</td>
</tr>
<tr>
<td>

<!-- divChart -->
  
<div id="AreaChartID387350b6e927" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
</table>

</td>
</tr>
<tr>
<td>

<!-- divChart -->
  
<div id="ColumnChartID38731636cbf3" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
</table>

</td>
</tr>
<tr>
<td>

<!-- divChart -->
  
<div id="ColumnChartID38731c2c2333" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
</table>
 <div><span>Data: various &#8226; Chart ID: <a href="Chart_MergedID3873c466e8b.html">MergedID3873c466e8b</a> &#8226; <a href="https://github.com/mages/googleVis">googleVis-0.6.4</a></span><br /> 
<!-- htmlFooter -->
<span> 
  R version 3.5.2 (2018-12-20) 
  &#8226; <a href="https://developers.google.com/terms/">Google Terms of Use</a> &#8226; Data Policy: See individual charts
</span></div>
</body>
</html>
