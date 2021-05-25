---
title: Air Quality at 2021-05-26 07:50:00
layout: single
permalink: /myairq/
---
### The Current Air Quality

<html xmlns="https://www.w3.org/1999/xhtml">
<head>
<title>MergedID47314c4b067</title>
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
<!-- Wed May 26 07:50:09 2021 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableID47335f5bee3 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
25.83,
52.16,
1006.75,
2281,
2.7,
1.9
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
function gvisDataLineChartID473d8049a3 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,26,7,36,0),
26,
51.5
],
[
new Date(2021,4,26,7,37,0),
26.02,
51.72
],
[
new Date(2021,4,26,7,40,0),
26.01,
51.65
],
[
new Date(2021,4,26,7,41,0),
26,
51.47
],
[
new Date(2021,4,26,7,42,0),
26,
51.58
],
[
new Date(2021,4,26,7,43,0),
25.99,
51.83
],
[
new Date(2021,4,26,7,44,0),
25.98,
51.77
],
[
new Date(2021,4,26,7,45,0),
25.99,
51.95
],
[
new Date(2021,4,26,7,46,0),
25.97,
51.73
],
[
new Date(2021,4,26,7,47,0),
25.94,
52.41
],
[
new Date(2021,4,26,7,48,0),
25.88,
52.54
],
[
new Date(2021,4,26,7,49,0),
25.85,
52.39
],
[
new Date(2021,4,26,7,50,0),
25.83,
52.16
] 
];
data.addColumn('datetime','time');
data.addColumn('number','Temperature');
data.addColumn('number','Humidity');
data.addRows(datajson);
return(data);
}


// jsData 
function gvisDataAreaChartID473be31c67 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,26,7,36,0),
1006.9,
"#9B59B6"
],
[
new Date(2021,4,26,7,37,0),
1006.83,
"#9B59B6"
],
[
new Date(2021,4,26,7,40,0),
1006.94,
"#9B59B6"
],
[
new Date(2021,4,26,7,41,0),
1006.93,
"#9B59B6"
],
[
new Date(2021,4,26,7,42,0),
1006.91,
"#9B59B6"
],
[
new Date(2021,4,26,7,43,0),
1006.86,
"#9B59B6"
],
[
new Date(2021,4,26,7,44,0),
1006.89,
"#9B59B6"
],
[
new Date(2021,4,26,7,45,0),
1006.87,
"#9B59B6"
],
[
new Date(2021,4,26,7,46,0),
1006.85,
"#9B59B6"
],
[
new Date(2021,4,26,7,47,0),
1006.82,
"#9B59B6"
],
[
new Date(2021,4,26,7,48,0),
1006.78,
"#9B59B6"
],
[
new Date(2021,4,26,7,49,0),
1006.78,
"#9B59B6"
],
[
new Date(2021,4,26,7,50,0),
1006.75,
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
function gvisDataAreaChartID4731fdb196e () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,26,7,36,0),
2152,
"#F6614E"
],
[
new Date(2021,4,26,7,37,0),
2065,
"#F6614E"
],
[
new Date(2021,4,26,7,40,0),
2088,
"#F6614E"
],
[
new Date(2021,4,26,7,41,0),
2153,
"#F6614E"
],
[
new Date(2021,4,26,7,42,0),
2176,
"#F6614E"
],
[
new Date(2021,4,26,7,43,0),
2173,
"#F6614E"
],
[
new Date(2021,4,26,7,44,0),
2148,
"#F6614E"
],
[
new Date(2021,4,26,7,45,0),
2136,
"#F6614E"
],
[
new Date(2021,4,26,7,46,0),
2145,
"#F6614E"
],
[
new Date(2021,4,26,7,47,0),
2179,
"#F6614E"
],
[
new Date(2021,4,26,7,48,0),
2213,
"#F6614E"
],
[
new Date(2021,4,26,7,49,0),
2257,
"#F6614E"
],
[
new Date(2021,4,26,7,50,0),
2281,
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
function gvisDataColumnChartID4735f2eb65f () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,26,7,40,0),
5.6,
"#4E89F6"
],
[
new Date(2021,4,26,7,50,0),
2.7,
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
function gvisDataColumnChartID4736721175b () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,26,7,40,0),
1.4,
"#4E89F6"
],
[
new Date(2021,4,26,7,50,0),
1.9,
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
function drawChartTableID47335f5bee3() {
var data = gvisDataTableID47335f5bee3();
var options = {};
options["allowHtml"] = true;
options["width"] = 600;


    var chart = new google.visualization.Table(
    document.getElementById('TableID47335f5bee3')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartLineChartID473d8049a3() {
var data = gvisDataLineChartID473d8049a3();
var options = {};
options["allowHtml"] = true;
options["title"] = "Temperature and Humidity";
options["series"] = [{color:'#F6614E', targetAxisIndex:0},
                                  {color:'#4E89F6', targetAxisIndex:1}];
options["vAxes"] = [{title:'Temp. (C)'},{title:'Hum. (%)'}];
options["width"] = 600;


    var chart = new google.visualization.LineChart(
    document.getElementById('LineChartID473d8049a3')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartAreaChartID473be31c67() {
var data = gvisDataAreaChartID473be31c67();
var options = {};
options["allowHtml"] = true;
options["title"] = "Air Pressure";
options["vAxis"] = {title:'(hPa)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.AreaChart(
    document.getElementById('AreaChartID473be31c67')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartAreaChartID4731fdb196e() {
var data = gvisDataAreaChartID4731fdb196e();
var options = {};
options["allowHtml"] = true;
options["title"] = "CO2 Level";
options["vAxis"] = {title:'(ppm)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.AreaChart(
    document.getElementById('AreaChartID4731fdb196e')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartColumnChartID4735f2eb65f() {
var data = gvisDataColumnChartID4735f2eb65f();
var options = {};
options["allowHtml"] = true;
options["title"] = "PM 10";
options["vAxis"] = {title:'(ug/m3)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.ColumnChart(
    document.getElementById('ColumnChartID4735f2eb65f')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartColumnChartID4736721175b() {
var data = gvisDataColumnChartID4736721175b();
var options = {};
options["allowHtml"] = true;
options["title"] = "PM 2.5";
options["vAxis"] = {title:'(ug/m3)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.ColumnChart(
    document.getElementById('ColumnChartID4736721175b')
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
callbacks.push(drawChartTableID47335f5bee3);
})();
function displayChartTableID47335f5bee3() {
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
callbacks.push(drawChartLineChartID473d8049a3);
})();
function displayChartLineChartID473d8049a3() {
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
callbacks.push(drawChartAreaChartID473be31c67);
})();
function displayChartAreaChartID473be31c67() {
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
callbacks.push(drawChartAreaChartID4731fdb196e);
})();
function displayChartAreaChartID4731fdb196e() {
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
callbacks.push(drawChartColumnChartID4735f2eb65f);
})();
function displayChartColumnChartID4735f2eb65f() {
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
callbacks.push(drawChartColumnChartID4736721175b);
})();
function displayChartColumnChartID4736721175b() {
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
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID47335f5bee3"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartLineChartID473d8049a3"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartAreaChartID473be31c67"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartAreaChartID4731fdb196e"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartColumnChartID4735f2eb65f"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartColumnChartID4736721175b"></script>
 
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
  
<div id="TableID47335f5bee3" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
<tr>
<td>

<!-- divChart -->
  
<div id="LineChartID473d8049a3" 
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
  
<div id="AreaChartID473be31c67" 
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
  
<div id="AreaChartID4731fdb196e" 
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
  
<div id="ColumnChartID4735f2eb65f" 
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
  
<div id="ColumnChartID4736721175b" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
</table>
 <div><span>Data: various &#8226; Chart ID: <a href="Chart_MergedID47314c4b067.html">MergedID47314c4b067</a> &#8226; <a href="https://github.com/mages/googleVis">googleVis-0.6.4</a></span><br /> 
<!-- htmlFooter -->
<span> 
  R version 3.5.2 (2018-12-20) 
  &#8226; <a href="https://developers.google.com/terms/">Google Terms of Use</a> &#8226; Data Policy: See individual charts
</span></div>
</body>
</html>
