---
title: Air Quality at 2021-05-27 09:20:00
layout: single
permalink: /myairq/
---
### The Current Air Quality

<html xmlns="https://www.w3.org/1999/xhtml">
<head>
<title>MergedID104c7b80d511</title>
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
<!-- Thu May 27 09:20:06 2021 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableID104c628c4501 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
23.57,
54.13,
996.59,
5000,
5.7,
2.9
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
function gvisDataLineChartID104c1d567d90 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,27,9,14,0),
24.41,
50.84
],
[
new Date(2021,4,27,9,15,0),
24.41,
50.82
],
[
new Date(2021,4,27,9,16,0),
24.36,
51.3
],
[
new Date(2021,4,27,9,17,0),
24.24,
51.64
],
[
new Date(2021,4,27,9,18,0),
24.23,
51.74
],
[
new Date(2021,4,27,9,19,0),
23.95,
53.36
],
[
new Date(2021,4,27,9,20,0),
23.57,
54.13
] 
];
data.addColumn('datetime','time');
data.addColumn('number','Temperature');
data.addColumn('number','Humidity');
data.addRows(datajson);
return(data);
}


// jsData 
function gvisDataAreaChartID104c6ccbd583 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,27,9,14,0),
996.54,
"#9B59B6"
],
[
new Date(2021,4,27,9,15,0),
996.54,
"#9B59B6"
],
[
new Date(2021,4,27,9,16,0),
996.59,
"#9B59B6"
],
[
new Date(2021,4,27,9,17,0),
996.63,
"#9B59B6"
],
[
new Date(2021,4,27,9,18,0),
996.56,
"#9B59B6"
],
[
new Date(2021,4,27,9,19,0),
996.57,
"#9B59B6"
],
[
new Date(2021,4,27,9,20,0),
996.59,
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
function gvisDataAreaChartID104c2152bb96 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,27,9,14,0),
410,
"#4E89F6"
],
[
new Date(2021,4,27,9,15,0),
410,
"#4E89F6"
],
[
new Date(2021,4,27,9,16,0),
5000,
"#5D6D7E"
],
[
new Date(2021,4,27,9,17,0),
5000,
"#5D6D7E"
],
[
new Date(2021,4,27,9,18,0),
5000,
"#5D6D7E"
],
[
new Date(2021,4,27,9,19,0),
5000,
"#5D6D7E"
],
[
new Date(2021,4,27,9,20,0),
5000,
"#5D6D7E"
] 
];
data.addColumn('datetime','time');
data.addColumn('number','CO2');
data.addColumn({type: 'string', role: 'style'});
data.addRows(datajson);
return(data);
}


// jsData 
function gvisDataColumnChartID104c27c0c02a () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,27,9,20,0),
5.7,
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
function gvisDataColumnChartID104c1da657a3 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2021,4,27,9,20,0),
2.9,
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
function drawChartTableID104c628c4501() {
var data = gvisDataTableID104c628c4501();
var options = {};
options["allowHtml"] = true;
options["width"] = 600;


    var chart = new google.visualization.Table(
    document.getElementById('TableID104c628c4501')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartLineChartID104c1d567d90() {
var data = gvisDataLineChartID104c1d567d90();
var options = {};
options["allowHtml"] = true;
options["title"] = "Temperature and Humidity";
options["series"] = [{color:'#F6614E', targetAxisIndex:0},
                                  {color:'#4E89F6', targetAxisIndex:1}];
options["vAxes"] = [{title:'Temp. (C)'},{title:'Hum. (%)'}];
options["width"] = 600;


    var chart = new google.visualization.LineChart(
    document.getElementById('LineChartID104c1d567d90')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartAreaChartID104c6ccbd583() {
var data = gvisDataAreaChartID104c6ccbd583();
var options = {};
options["allowHtml"] = true;
options["title"] = "Air Pressure";
options["vAxis"] = {title:'(hPa)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.AreaChart(
    document.getElementById('AreaChartID104c6ccbd583')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartAreaChartID104c2152bb96() {
var data = gvisDataAreaChartID104c2152bb96();
var options = {};
options["allowHtml"] = true;
options["title"] = "CO2 Level";
options["vAxis"] = {title:'(ppm)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.AreaChart(
    document.getElementById('AreaChartID104c2152bb96')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartColumnChartID104c27c0c02a() {
var data = gvisDataColumnChartID104c27c0c02a();
var options = {};
options["allowHtml"] = true;
options["title"] = "PM 10";
options["vAxis"] = {title:'(ug/m3)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.ColumnChart(
    document.getElementById('ColumnChartID104c27c0c02a')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartColumnChartID104c1da657a3() {
var data = gvisDataColumnChartID104c1da657a3();
var options = {};
options["allowHtml"] = true;
options["title"] = "PM 2.5";
options["vAxis"] = {title:'(ug/m3)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.ColumnChart(
    document.getElementById('ColumnChartID104c1da657a3')
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
callbacks.push(drawChartTableID104c628c4501);
})();
function displayChartTableID104c628c4501() {
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
callbacks.push(drawChartLineChartID104c1d567d90);
})();
function displayChartLineChartID104c1d567d90() {
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
callbacks.push(drawChartAreaChartID104c6ccbd583);
})();
function displayChartAreaChartID104c6ccbd583() {
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
callbacks.push(drawChartAreaChartID104c2152bb96);
})();
function displayChartAreaChartID104c2152bb96() {
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
callbacks.push(drawChartColumnChartID104c27c0c02a);
})();
function displayChartColumnChartID104c27c0c02a() {
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
callbacks.push(drawChartColumnChartID104c1da657a3);
})();
function displayChartColumnChartID104c1da657a3() {
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
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID104c628c4501"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartLineChartID104c1d567d90"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartAreaChartID104c6ccbd583"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartAreaChartID104c2152bb96"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartColumnChartID104c27c0c02a"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartColumnChartID104c1da657a3"></script>
 
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
  
<div id="TableID104c628c4501" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
<tr>
<td>

<!-- divChart -->
  
<div id="LineChartID104c1d567d90" 
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
  
<div id="AreaChartID104c6ccbd583" 
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
  
<div id="AreaChartID104c2152bb96" 
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
  
<div id="ColumnChartID104c27c0c02a" 
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
  
<div id="ColumnChartID104c1da657a3" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
</table>
 <div><span>Data: various &#8226; Chart ID: <a href="Chart_MergedID104c7b80d511.html">MergedID104c7b80d511</a> &#8226; <a href="https://github.com/mages/googleVis">googleVis-0.6.4</a></span><br /> 
<!-- htmlFooter -->
<span> 
  R version 3.5.2 (2018-12-20) 
  &#8226; <a href="https://developers.google.com/terms/">Google Terms of Use</a> &#8226; Data Policy: See individual charts
</span></div>
</body>
</html>
