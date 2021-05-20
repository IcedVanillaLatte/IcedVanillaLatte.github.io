---
title: Air Quality at 2021-05-21 08:00:00
layout: single
permalink: /myairq/
---
### The Current Air Quality

<html xmlns="https://www.w3.org/1999/xhtml">
<head>
<title>MergedID76f13651e7a</title>
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
<!-- Fri May 21 08:00:06 2021 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableID76f4c99e2d3 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
26.31,
57.61,
1000.47,
2197,
17.8,
1.5
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
function gvisDataLineChartID76f6a5d2447 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,21,7,51,0),
26.39,
56.51
],
[
new Date(2021,4,21,7,52,0),
26.38,
56.73
],
[
new Date(2021,4,21,7,53,0),
26.36,
57.13
],
[
new Date(2021,4,21,7,54,0),
26.34,
57.32
],
[
new Date(2021,4,21,7,55,0),
26.33,
57.34
],
[
new Date(2021,4,21,7,56,0),
26.32,
57.05
],
[
new Date(2021,4,21,7,57,0),
26.32,
57.39
],
[
new Date(2021,4,21,7,58,0),
26.31,
57.49
],
[
new Date(2021,4,21,7,59,0),
26.3,
57.66
],
[
new Date(2021,4,21,8,0,0),
26.31,
57.61
] 
];
data.addColumn('datetime','time');
data.addColumn('number','Temperature');
data.addColumn('number','Humidity');
data.addRows(datajson);
return(data);
}


// jsData 
function gvisDataAreaChartID76f3dd58ff () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,21,7,51,0),
1000.31,
"#9B59B6"
],
[
new Date(2021,4,21,7,52,0),
1000.36,
"#9B59B6"
],
[
new Date(2021,4,21,7,53,0),
1000.39,
"#9B59B6"
],
[
new Date(2021,4,21,7,54,0),
1000.37,
"#9B59B6"
],
[
new Date(2021,4,21,7,55,0),
1000.37,
"#9B59B6"
],
[
new Date(2021,4,21,7,56,0),
1000.43,
"#9B59B6"
],
[
new Date(2021,4,21,7,57,0),
1000.39,
"#9B59B6"
],
[
new Date(2021,4,21,7,58,0),
1000.44,
"#9B59B6"
],
[
new Date(2021,4,21,7,59,0),
1000.45,
"#9B59B6"
],
[
new Date(2021,4,21,8,0,0),
1000.47,
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
function gvisDataAreaChartID76f547aa4 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,21,7,51,0),
410,
"#4E89F6"
],
[
new Date(2021,4,21,7,52,0),
2030,
"#F6614E"
],
[
new Date(2021,4,21,7,53,0),
2032,
"#F6614E"
],
[
new Date(2021,4,21,7,54,0),
2073,
"#F6614E"
],
[
new Date(2021,4,21,7,55,0),
2133,
"#F6614E"
],
[
new Date(2021,4,21,7,56,0),
2171,
"#F6614E"
],
[
new Date(2021,4,21,7,57,0),
2174,
"#F6614E"
],
[
new Date(2021,4,21,7,58,0),
2176,
"#F6614E"
],
[
new Date(2021,4,21,7,59,0),
2184,
"#F6614E"
],
[
new Date(2021,4,21,8,0,0),
2197,
"#F6614E"
] 
];
data.addColumn('datetime','time');
data.addColumn('number','CO2');
data.addColumn({type: 'string', role: 'style'});
data.addRows(datajson);
return(data);
}


// jsData 
function gvisDataColumnChartID76fd6b29de () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,21,8,0,0),
17.8,
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
function gvisDataColumnChartID76f4bad175d () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,21,8,0,0),
1.5,
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
function drawChartTableID76f4c99e2d3() {
var data = gvisDataTableID76f4c99e2d3();
var options = {};
options["allowHtml"] = true;
options["width"] = 600;


    var chart = new google.visualization.Table(
    document.getElementById('TableID76f4c99e2d3')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartLineChartID76f6a5d2447() {
var data = gvisDataLineChartID76f6a5d2447();
var options = {};
options["allowHtml"] = true;
options["title"] = "Temperature and Humidity";
options["series"] = [{color:'#F6614E', targetAxisIndex:0},
                                  {color:'#4E89F6', targetAxisIndex:1}];
options["vAxes"] = [{title:'Temp. (C)'},{title:'Hum. (%)'}];
options["width"] = 600;


    var chart = new google.visualization.LineChart(
    document.getElementById('LineChartID76f6a5d2447')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartAreaChartID76f3dd58ff() {
var data = gvisDataAreaChartID76f3dd58ff();
var options = {};
options["allowHtml"] = true;
options["title"] = "Air Pressure";
options["vAxis"] = {title:'(hPa)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.AreaChart(
    document.getElementById('AreaChartID76f3dd58ff')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartAreaChartID76f547aa4() {
var data = gvisDataAreaChartID76f547aa4();
var options = {};
options["allowHtml"] = true;
options["title"] = "CO2 Level";
options["vAxis"] = {title:'(ppm)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.AreaChart(
    document.getElementById('AreaChartID76f547aa4')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartColumnChartID76fd6b29de() {
var data = gvisDataColumnChartID76fd6b29de();
var options = {};
options["allowHtml"] = true;
options["title"] = "PM 10";
options["vAxis"] = {title:'(ug/m3)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.ColumnChart(
    document.getElementById('ColumnChartID76fd6b29de')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartColumnChartID76f4bad175d() {
var data = gvisDataColumnChartID76f4bad175d();
var options = {};
options["allowHtml"] = true;
options["title"] = "PM 2.5";
options["vAxis"] = {title:'(ug/m3)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.ColumnChart(
    document.getElementById('ColumnChartID76f4bad175d')
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
callbacks.push(drawChartTableID76f4c99e2d3);
})();
function displayChartTableID76f4c99e2d3() {
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
callbacks.push(drawChartLineChartID76f6a5d2447);
})();
function displayChartLineChartID76f6a5d2447() {
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
callbacks.push(drawChartAreaChartID76f3dd58ff);
})();
function displayChartAreaChartID76f3dd58ff() {
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
callbacks.push(drawChartAreaChartID76f547aa4);
})();
function displayChartAreaChartID76f547aa4() {
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
callbacks.push(drawChartColumnChartID76fd6b29de);
})();
function displayChartColumnChartID76fd6b29de() {
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
callbacks.push(drawChartColumnChartID76f4bad175d);
})();
function displayChartColumnChartID76f4bad175d() {
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
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID76f4c99e2d3"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartLineChartID76f6a5d2447"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartAreaChartID76f3dd58ff"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartAreaChartID76f547aa4"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartColumnChartID76fd6b29de"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartColumnChartID76f4bad175d"></script>
 
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
  
<div id="TableID76f4c99e2d3" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
<tr>
<td>

<!-- divChart -->
  
<div id="LineChartID76f6a5d2447" 
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
  
<div id="AreaChartID76f3dd58ff" 
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
  
<div id="AreaChartID76f547aa4" 
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
  
<div id="ColumnChartID76fd6b29de" 
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
  
<div id="ColumnChartID76f4bad175d" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
</table>
 <div><span>Data: various &#8226; Chart ID: <a href="Chart_MergedID76f13651e7a.html">MergedID76f13651e7a</a> &#8226; <a href="https://github.com/mages/googleVis">googleVis-0.6.4</a></span><br /> 
<!-- htmlFooter -->
<span> 
  R version 3.5.2 (2018-12-20) 
  &#8226; <a href="https://developers.google.com/terms/">Google Terms of Use</a> &#8226; Data Policy: See individual charts
</span></div>
</body>
</html>
