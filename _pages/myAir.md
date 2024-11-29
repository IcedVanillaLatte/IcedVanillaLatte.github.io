---
title: Air Quality at 2024-11-29 17:50:00
layout: single
permalink: /myair/
---
### The Current Air Quality

<html xmlns="https://www.w3.org/1999/xhtml">
<head>
<title>MergedID7536c1fcba1</title>
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
<body> <!-- Table generated in R 4.2.2 by googleVis 0.7.3 package -->
<!-- Fri Nov 29 17:50:09 2024 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableID7532c6f602a () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
23.07,
47.53,
1007.56,
719,
11.2,
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
function gvisDataLineChartID753170c059c () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2024,10,29,17,41,0),
22.96,
47.07
],
[
new Date(2024,10,29,17,42,0),
22.97,
47.09
],
[
new Date(2024,10,29,17,43,0),
22.97,
47.14
],
[
new Date(2024,10,29,17,44,0),
22.98,
47.2
],
[
new Date(2024,10,29,17,45,0),
23,
47.25
],
[
new Date(2024,10,29,17,46,0),
23.01,
47.3
],
[
new Date(2024,10,29,17,47,0),
23.03,
47.37
],
[
new Date(2024,10,29,17,48,0),
23.03,
47.43
],
[
new Date(2024,10,29,17,49,0),
23.05,
47.46
],
[
new Date(2024,10,29,17,50,0),
23.07,
47.53
] 
];
data.addColumn('datetime','time');
data.addColumn('number','Temperature');
data.addColumn('number','Humidity');
data.addRows(datajson);
return(data);
}


// jsData 
function gvisDataAreaChartID75379cbcff0 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2024,10,29,17,41,0),
1007.56,
"#9B59B6"
],
[
new Date(2024,10,29,17,42,0),
1007.56,
"#9B59B6"
],
[
new Date(2024,10,29,17,43,0),
1007.58,
"#9B59B6"
],
[
new Date(2024,10,29,17,44,0),
1007.58,
"#9B59B6"
],
[
new Date(2024,10,29,17,45,0),
1007.6,
"#9B59B6"
],
[
new Date(2024,10,29,17,46,0),
1007.64,
"#9B59B6"
],
[
new Date(2024,10,29,17,47,0),
1007.65,
"#9B59B6"
],
[
new Date(2024,10,29,17,48,0),
1007.65,
"#9B59B6"
],
[
new Date(2024,10,29,17,49,0),
1007.68,
"#9B59B6"
],
[
new Date(2024,10,29,17,50,0),
1007.56,
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
function gvisDataAreaChartID7536bb44b05 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2024,10,29,17,41,0),
660,
"#3DC948"
],
[
new Date(2024,10,29,17,42,0),
682,
"#3DC948"
],
[
new Date(2024,10,29,17,43,0),
686,
"#3DC948"
],
[
new Date(2024,10,29,17,44,0),
680,
"#3DC948"
],
[
new Date(2024,10,29,17,45,0),
690,
"#3DC948"
],
[
new Date(2024,10,29,17,46,0),
710,
"#F6EA4E"
],
[
new Date(2024,10,29,17,47,0),
710,
"#F6EA4E"
],
[
new Date(2024,10,29,17,48,0),
723,
"#F6EA4E"
],
[
new Date(2024,10,29,17,49,0),
731,
"#F6EA4E"
],
[
new Date(2024,10,29,17,50,0),
719,
"#F6EA4E"
] 
];
data.addColumn('datetime','time');
data.addColumn('number','CO2');
data.addColumn({type: 'string', role: 'style'});
data.addRows(datajson);
return(data);
}


// jsData 
function gvisDataColumnChartID753211e58b0 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2024,10,29,17,50,0),
11.2,
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
function gvisDataColumnChartID7532ba74489 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2024,10,29,17,50,0),
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
function drawChartTableID7532c6f602a() {
var data = gvisDataTableID7532c6f602a();
var options = {};
options["allowHtml"] = true;
options["width"] = 600;


    var chart = new google.visualization.Table(
    document.getElementById('TableID7532c6f602a')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartLineChartID753170c059c() {
var data = gvisDataLineChartID753170c059c();
var options = {};
options["allowHtml"] = true;
options["title"] = "Temperature and Humidity";
options["series"] = [{color:'#F6614E', targetAxisIndex:0},
                                  {color:'#4E89F6', targetAxisIndex:1}];
options["vAxes"] = [{title:'Temp. (C)'},{title:'Hum. (%)'}];
options["width"] = 600;


    var chart = new google.visualization.LineChart(
    document.getElementById('LineChartID753170c059c')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartAreaChartID75379cbcff0() {
var data = gvisDataAreaChartID75379cbcff0();
var options = {};
options["allowHtml"] = true;
options["title"] = "Air Pressure";
options["vAxis"] = {title:'(hPa)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.AreaChart(
    document.getElementById('AreaChartID75379cbcff0')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartAreaChartID7536bb44b05() {
var data = gvisDataAreaChartID7536bb44b05();
var options = {};
options["allowHtml"] = true;
options["title"] = "CO2 Level";
options["vAxis"] = {title:'(ppm)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.AreaChart(
    document.getElementById('AreaChartID7536bb44b05')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartColumnChartID753211e58b0() {
var data = gvisDataColumnChartID753211e58b0();
var options = {};
options["allowHtml"] = true;
options["title"] = "PM 10";
options["vAxis"] = {title:'(ug/m3)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.ColumnChart(
    document.getElementById('ColumnChartID753211e58b0')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartColumnChartID7532ba74489() {
var data = gvisDataColumnChartID7532ba74489();
var options = {};
options["allowHtml"] = true;
options["title"] = "PM 2.5";
options["vAxis"] = {title:'(ug/m3)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.ColumnChart(
    document.getElementById('ColumnChartID7532ba74489')
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
callbacks.push(drawChartTableID7532c6f602a);
})();
function displayChartTableID7532c6f602a() {
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
callbacks.push(drawChartLineChartID753170c059c);
})();
function displayChartLineChartID753170c059c() {
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
callbacks.push(drawChartAreaChartID75379cbcff0);
})();
function displayChartAreaChartID75379cbcff0() {
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
callbacks.push(drawChartAreaChartID7536bb44b05);
})();
function displayChartAreaChartID7536bb44b05() {
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
callbacks.push(drawChartColumnChartID753211e58b0);
})();
function displayChartColumnChartID753211e58b0() {
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
callbacks.push(drawChartColumnChartID7532ba74489);
})();
function displayChartColumnChartID7532ba74489() {
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
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID7532c6f602a"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartLineChartID753170c059c"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartAreaChartID75379cbcff0"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartAreaChartID7536bb44b05"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartColumnChartID753211e58b0"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartColumnChartID7532ba74489"></script>
 
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
  
<div id="TableID7532c6f602a" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
<tr>
<td>

<!-- divChart -->
  
<div id="LineChartID753170c059c" 
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
  
<div id="AreaChartID75379cbcff0" 
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
  
<div id="AreaChartID7536bb44b05" 
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
  
<div id="ColumnChartID753211e58b0" 
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
  
<div id="ColumnChartID7532ba74489" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
</table>
 <div><span>Data: various &#8226; Chart ID: <a href="Chart_MergedID7536c1fcba1.html">MergedID7536c1fcba1</a> &#8226; <a href="https://mages.github.io/googleVis/">googleVis-0.7.3</a></span><br /> 
<!-- htmlFooter -->
<span> 
  R version 4.2.2 Patched (2022-11-10 r83330) 
  &#8226; <a href="https://developers.google.com/terms/">Google Terms of Use</a> &#8226; Data Policy: See individual charts
</span></div>
</body>
</html>
