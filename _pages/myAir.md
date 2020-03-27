---
title: Visualization on Air Quality
layout: single
permalink: /myair/
---

<html xmlns="https://www.w3.org/1999/xhtml">
<head>
<title>MergedID2ca940241f16</title>
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
<body>
 <!-- LineChart generated in R 3.5.2 by googleVis 0.6.4 package -->
<!-- Sat Mar 28 00:40:05 2020 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataLineChartID2ca924f153e0 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2020,2,28,0,0,0),
24.1,
64.14
],
[
new Date(2020,2,28,0,1,0),
24.11,
64.16
],
[
new Date(2020,2,28,0,2,0),
24.09,
64.13
],
[
new Date(2020,2,28,0,3,0),
24.09,
64.23
],
[
new Date(2020,2,28,0,4,0),
24.07,
63.95
],
[
new Date(2020,2,28,0,4,0),
24.06,
63.99
],
[
new Date(2020,2,28,0,5,0),
24.06,
63.99
],
[
new Date(2020,2,28,0,6,0),
24.06,
64.11
],
[
new Date(2020,2,28,0,7,0),
24.06,
64.09
],
[
new Date(2020,2,28,0,8,0),
24.07,
64.22
],
[
new Date(2020,2,28,0,9,0),
24.08,
64.25
],
[
new Date(2020,2,28,0,10,0),
24.07,
64.09
],
[
new Date(2020,2,28,0,11,0),
24.1,
64.08
],
[
new Date(2020,2,28,0,12,0),
24.1,
64.01
],
[
new Date(2020,2,28,0,13,0),
24.09,
63.91
],
[
new Date(2020,2,28,0,14,0),
24.11,
63.83
],
[
new Date(2020,2,28,0,15,0),
24.09,
63.94
],
[
new Date(2020,2,28,0,16,0),
24.11,
64.33
],
[
new Date(2020,2,28,0,17,0),
24.14,
64.18
],
[
new Date(2020,2,28,0,18,0),
24.15,
64.17
],
[
new Date(2020,2,28,0,19,0),
24.15,
64.06
],
[
new Date(2020,2,28,0,20,0),
24.15,
64.09
],
[
new Date(2020,2,28,0,21,0),
24.14,
64.05
],
[
new Date(2020,2,28,0,22,0),
24.13,
64.08
],
[
new Date(2020,2,28,0,23,0),
24.12,
64.14
],
[
new Date(2020,2,28,0,24,0),
24.11,
64.26
],
[
new Date(2020,2,28,0,25,0),
24.1,
64.19
],
[
new Date(2020,2,28,0,26,0),
24.1,
64.28
],
[
new Date(2020,2,28,0,27,0),
24.09,
64.3
],
[
new Date(2020,2,28,0,28,0),
24.11,
64.26
],
[
new Date(2020,2,28,0,29,0),
24.09,
64.11
],
[
new Date(2020,2,28,0,30,0),
24.09,
64.23
],
[
new Date(2020,2,28,0,31,0),
24.08,
64.23
],
[
new Date(2020,2,28,0,32,0),
24.08,
64.21
],
[
new Date(2020,2,28,0,33,0),
24.08,
64.35
],
[
new Date(2020,2,28,0,34,0),
24.07,
64.29
],
[
new Date(2020,2,28,0,35,0),
24.07,
64.2
],
[
new Date(2020,2,28,0,36,0),
24.06,
64.14
],
[
new Date(2020,2,28,0,37,0),
24.07,
64.02
],
[
new Date(2020,2,28,0,38,0),
24.05,
63.89
],
[
new Date(2020,2,28,0,39,0),
24.05,
64.13
],
[
new Date(2020,2,28,0,40,0),
24.04,
64.12
] 
];
data.addColumn('datetime','time');
data.addColumn('number','Temperature');
data.addColumn('number','Humidity');
data.addRows(datajson);
return(data);
}


// jsData 
function gvisDataAreaChartID2ca9635c312b () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2020,2,28,0,0,0),
1005.92,
"#9B59B6"
],
[
new Date(2020,2,28,0,1,0),
1005.91,
"#9B59B6"
],
[
new Date(2020,2,28,0,2,0),
1005.94,
"#9B59B6"
],
[
new Date(2020,2,28,0,3,0),
1005.89,
"#9B59B6"
],
[
new Date(2020,2,28,0,4,0),
1005.87,
"#9B59B6"
],
[
new Date(2020,2,28,0,4,0),
1005.95,
"#9B59B6"
],
[
new Date(2020,2,28,0,5,0),
1005.87,
"#9B59B6"
],
[
new Date(2020,2,28,0,6,0),
1005.93,
"#9B59B6"
],
[
new Date(2020,2,28,0,7,0),
1005.94,
"#9B59B6"
],
[
new Date(2020,2,28,0,8,0),
1005.96,
"#9B59B6"
],
[
new Date(2020,2,28,0,9,0),
1005.84,
"#9B59B6"
],
[
new Date(2020,2,28,0,10,0),
1005.86,
"#9B59B6"
],
[
new Date(2020,2,28,0,11,0),
1005.79,
"#9B59B6"
],
[
new Date(2020,2,28,0,12,0),
1005.78,
"#9B59B6"
],
[
new Date(2020,2,28,0,13,0),
1005.8,
"#9B59B6"
],
[
new Date(2020,2,28,0,14,0),
1005.88,
"#9B59B6"
],
[
new Date(2020,2,28,0,15,0),
1005.83,
"#9B59B6"
],
[
new Date(2020,2,28,0,16,0),
1005.8,
"#9B59B6"
],
[
new Date(2020,2,28,0,17,0),
1005.85,
"#9B59B6"
],
[
new Date(2020,2,28,0,18,0),
1005.85,
"#9B59B6"
],
[
new Date(2020,2,28,0,19,0),
1005.82,
"#9B59B6"
],
[
new Date(2020,2,28,0,20,0),
1005.86,
"#9B59B6"
],
[
new Date(2020,2,28,0,21,0),
1005.86,
"#9B59B6"
],
[
new Date(2020,2,28,0,22,0),
1005.75,
"#9B59B6"
],
[
new Date(2020,2,28,0,23,0),
1005.69,
"#9B59B6"
],
[
new Date(2020,2,28,0,24,0),
1005.66,
"#9B59B6"
],
[
new Date(2020,2,28,0,25,0),
1005.56,
"#9B59B6"
],
[
new Date(2020,2,28,0,26,0),
1005.59,
"#9B59B6"
],
[
new Date(2020,2,28,0,27,0),
1005.57,
"#9B59B6"
],
[
new Date(2020,2,28,0,28,0),
1005.59,
"#9B59B6"
],
[
new Date(2020,2,28,0,29,0),
1005.65,
"#9B59B6"
],
[
new Date(2020,2,28,0,30,0),
1005.69,
"#9B59B6"
],
[
new Date(2020,2,28,0,31,0),
1005.7,
"#9B59B6"
],
[
new Date(2020,2,28,0,32,0),
1005.74,
"#9B59B6"
],
[
new Date(2020,2,28,0,33,0),
1005.77,
"#9B59B6"
],
[
new Date(2020,2,28,0,34,0),
1005.72,
"#9B59B6"
],
[
new Date(2020,2,28,0,35,0),
1005.76,
"#9B59B6"
],
[
new Date(2020,2,28,0,36,0),
1005.78,
"#9B59B6"
],
[
new Date(2020,2,28,0,37,0),
1005.81,
"#9B59B6"
],
[
new Date(2020,2,28,0,38,0),
1005.84,
"#9B59B6"
],
[
new Date(2020,2,28,0,39,0),
1005.72,
"#9B59B6"
],
[
new Date(2020,2,28,0,40,0),
1005.75,
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
function gvisDataAreaChartID2ca9121771c6 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2020,2,28,0,0,0),
2455,
"#F6614E"
],
[
new Date(2020,2,28,0,1,0),
2448,
"#F6614E"
],
[
new Date(2020,2,28,0,2,0),
2449,
"#F6614E"
],
[
new Date(2020,2,28,0,3,0),
2444,
"#F6614E"
],
[
new Date(2020,2,28,0,4,0),
2441,
"#F6614E"
],
[
new Date(2020,2,28,0,4,0),
2444,
"#F6614E"
],
[
new Date(2020,2,28,0,5,0),
2444,
"#F6614E"
],
[
new Date(2020,2,28,0,6,0),
2448,
"#F6614E"
],
[
new Date(2020,2,28,0,7,0),
2449,
"#F6614E"
],
[
new Date(2020,2,28,0,8,0),
2452,
"#F6614E"
],
[
new Date(2020,2,28,0,9,0),
2465,
"#F6614E"
],
[
new Date(2020,2,28,0,10,0),
2462,
"#F6614E"
],
[
new Date(2020,2,28,0,11,0),
2466,
"#F6614E"
],
[
new Date(2020,2,28,0,12,0),
2478,
"#F6614E"
],
[
new Date(2020,2,28,0,13,0),
2488,
"#F6614E"
],
[
new Date(2020,2,28,0,14,0),
2486,
"#F6614E"
],
[
new Date(2020,2,28,0,15,0),
2490,
"#F6614E"
],
[
new Date(2020,2,28,0,16,0),
2489,
"#F6614E"
],
[
new Date(2020,2,28,0,17,0),
2492,
"#F6614E"
],
[
new Date(2020,2,28,0,18,0),
2482,
"#F6614E"
],
[
new Date(2020,2,28,0,19,0),
2482,
"#F6614E"
],
[
new Date(2020,2,28,0,20,0),
2481,
"#F6614E"
],
[
new Date(2020,2,28,0,21,0),
2478,
"#F6614E"
],
[
new Date(2020,2,28,0,22,0),
2486,
"#F6614E"
],
[
new Date(2020,2,28,0,23,0),
2512,
"#F6614E"
],
[
new Date(2020,2,28,0,24,0),
2537,
"#F6614E"
],
[
new Date(2020,2,28,0,25,0),
2569,
"#F6614E"
],
[
new Date(2020,2,28,0,26,0),
2622,
"#F6614E"
],
[
new Date(2020,2,28,0,27,0),
2650,
"#F6614E"
],
[
new Date(2020,2,28,0,28,0),
2699,
"#F6614E"
],
[
new Date(2020,2,28,0,29,0),
2731,
"#F6614E"
],
[
new Date(2020,2,28,0,30,0),
2749,
"#F6614E"
],
[
new Date(2020,2,28,0,31,0),
2766,
"#F6614E"
],
[
new Date(2020,2,28,0,32,0),
2748,
"#F6614E"
],
[
new Date(2020,2,28,0,33,0),
2721,
"#F6614E"
],
[
new Date(2020,2,28,0,34,0),
2647,
"#F6614E"
],
[
new Date(2020,2,28,0,35,0),
2593,
"#F6614E"
],
[
new Date(2020,2,28,0,36,0),
2569,
"#F6614E"
],
[
new Date(2020,2,28,0,37,0),
2557,
"#F6614E"
],
[
new Date(2020,2,28,0,38,0),
2555,
"#F6614E"
],
[
new Date(2020,2,28,0,39,0),
2552,
"#F6614E"
],
[
new Date(2020,2,28,0,40,0),
2559,
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
function gvisDataColumnChartID2ca944c5745e () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2020,2,28,0,2,0),
4.8,
"#4E89F6"
],
[
new Date(2020,2,28,0,6,0),
4.16,
"#4E89F6"
],
[
new Date(2020,2,28,0,11,0),
5.36,
"#4E89F6"
],
[
new Date(2020,2,28,0,16,0),
9.16,
"#4E89F6"
],
[
new Date(2020,2,28,0,21,0),
5.78,
"#4E89F6"
],
[
new Date(2020,2,28,0,26,0),
7.34,
"#4E89F6"
],
[
new Date(2020,2,28,0,31,0),
3.92,
"#4E89F6"
],
[
new Date(2020,2,28,0,36,0),
5.14,
"#4E89F6"
],
[
new Date(2020,2,28,0,39,30),
5.05,
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
function gvisDataColumnChartID2ca97e0c7048 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2020,2,28,0,2,0),
2.5,
"#4E89F6"
],
[
new Date(2020,2,28,0,6,0),
2.08,
"#4E89F6"
],
[
new Date(2020,2,28,0,11,0),
2.68,
"#4E89F6"
],
[
new Date(2020,2,28,0,16,0),
2.54,
"#4E89F6"
],
[
new Date(2020,2,28,0,21,0),
2.5,
"#4E89F6"
],
[
new Date(2020,2,28,0,26,0),
2.74,
"#4E89F6"
],
[
new Date(2020,2,28,0,31,0),
2.4,
"#4E89F6"
],
[
new Date(2020,2,28,0,36,0),
2.78,
"#4E89F6"
],
[
new Date(2020,2,28,0,39,30),
2.65,
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
function drawChartLineChartID2ca924f153e0() {
var data = gvisDataLineChartID2ca924f153e0();
var options = {};
options["allowHtml"] = true;
options["title"] = "Temperature and Humidity";
options["series"] = [{color:'#F6614E', targetAxisIndex:0},
                                  {color:'#4E89F6', targetAxisIndex:1}];
options["vAxes"] = [{title:'Temp. (C)'},{title:'Hum. (%)'}];
options["width"] = 600;


    var chart = new google.visualization.LineChart(
    document.getElementById('LineChartID2ca924f153e0')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartAreaChartID2ca9635c312b() {
var data = gvisDataAreaChartID2ca9635c312b();
var options = {};
options["allowHtml"] = true;
options["title"] = "Air Pressure";
options["vAxis"] = {title:'(hPa)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.AreaChart(
    document.getElementById('AreaChartID2ca9635c312b')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartAreaChartID2ca9121771c6() {
var data = gvisDataAreaChartID2ca9121771c6();
var options = {};
options["allowHtml"] = true;
options["title"] = "CO2 Level";
options["vAxis"] = {title:'(ppm)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.AreaChart(
    document.getElementById('AreaChartID2ca9121771c6')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartColumnChartID2ca944c5745e() {
var data = gvisDataColumnChartID2ca944c5745e();
var options = {};
options["allowHtml"] = true;
options["title"] = "PM 10";
options["vAxis"] = {title:'(ug/m3)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.ColumnChart(
    document.getElementById('ColumnChartID2ca944c5745e')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartColumnChartID2ca97e0c7048() {
var data = gvisDataColumnChartID2ca97e0c7048();
var options = {};
options["allowHtml"] = true;
options["title"] = "PM 2.5";
options["vAxis"] = {title:'(ug/m3)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.ColumnChart(
    document.getElementById('ColumnChartID2ca97e0c7048')
    );
    chart.draw(data,options);
    

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
callbacks.push(drawChartLineChartID2ca924f153e0);
})();
function displayChartLineChartID2ca924f153e0() {
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
callbacks.push(drawChartAreaChartID2ca9635c312b);
})();
function displayChartAreaChartID2ca9635c312b() {
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
callbacks.push(drawChartAreaChartID2ca9121771c6);
})();
function displayChartAreaChartID2ca9121771c6() {
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
callbacks.push(drawChartColumnChartID2ca944c5745e);
})();
function displayChartColumnChartID2ca944c5745e() {
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
callbacks.push(drawChartColumnChartID2ca97e0c7048);
})();
function displayChartColumnChartID2ca97e0c7048() {
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
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartLineChartID2ca924f153e0"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartAreaChartID2ca9635c312b"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartAreaChartID2ca9121771c6"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartColumnChartID2ca944c5745e"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartColumnChartID2ca97e0c7048"></script>
 
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
  
<div id="LineChartID2ca924f153e0" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
<tr>
<td>

<!-- divChart -->
  
<div id="AreaChartID2ca9635c312b" 
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
  
<div id="AreaChartID2ca9121771c6" 
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
  
<div id="ColumnChartID2ca944c5745e" 
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
  
<div id="ColumnChartID2ca97e0c7048" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
</table>
 <div><span>Data: various &#8226; Chart ID: <a href="Chart_MergedID2ca940241f16.html">MergedID2ca940241f16</a> &#8226; <a href="https://github.com/mages/googleVis">googleVis-0.6.4</a></span><br /> 
<!-- htmlFooter -->
<span> 
  R version 3.5.2 (2018-12-20) 
  &#8226; <a href="https://developers.google.com/terms/">Google Terms of Use</a> &#8226; Data Policy: See individual charts
</span></div>
</body>
</html>
