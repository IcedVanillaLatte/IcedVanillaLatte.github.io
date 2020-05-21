---
title: Air Quality at 2020-05-21 16:00:00
layout: single
permalink: /myairq/
---
### The Current Air Quality

<html xmlns="https://www.w3.org/1999/xhtml">
<head>
<title>MergedID76a485267ab</title>
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
<!-- Thu May 21 16:00:05 2020 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableID76a44bb5ebeb () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
25.68,
50.61,
998.94,
528,
4.1,
3.7
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
function gvisDataLineChartID76a4629a16ab () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2020,4,21,15,39,0),
25.61,
49.75
],
[
new Date(2020,4,21,15,40,0),
25.62,
49.87
],
[
new Date(2020,4,21,15,41,0),
25.62,
50.04
],
[
new Date(2020,4,21,15,42,0),
25.63,
50.11
],
[
new Date(2020,4,21,15,43,0),
25.62,
50.07
],
[
new Date(2020,4,21,15,44,0),
25.62,
50.18
],
[
new Date(2020,4,21,15,45,0),
25.63,
50.24
],
[
new Date(2020,4,21,15,46,0),
25.62,
50.24
],
[
new Date(2020,4,21,15,47,0),
25.63,
50.29
],
[
new Date(2020,4,21,15,48,0),
25.58,
50.31
],
[
new Date(2020,4,21,15,49,0),
25.52,
50.47
],
[
new Date(2020,4,21,15,50,0),
25.5,
50.58
],
[
new Date(2020,4,21,15,51,0),
25.51,
50.62
],
[
new Date(2020,4,21,15,52,0),
25.61,
50.41
],
[
new Date(2020,4,21,15,53,0),
25.6,
50.45
],
[
new Date(2020,4,21,15,54,0),
25.62,
50.51
],
[
new Date(2020,4,21,15,55,0),
25.6,
50.68
],
[
new Date(2020,4,21,15,56,0),
25.59,
50.71
],
[
new Date(2020,4,21,15,57,0),
25.63,
50.57
],
[
new Date(2020,4,21,15,58,0),
25.61,
50.7
],
[
new Date(2020,4,21,15,59,0),
25.64,
50.63
],
[
new Date(2020,4,21,16,0,0),
25.68,
50.61
] 
];
data.addColumn('datetime','time');
data.addColumn('number','Temperature');
data.addColumn('number','Humidity');
data.addRows(datajson);
return(data);
}


// jsData 
function gvisDataAreaChartID76a449c96c70 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2020,4,21,15,39,0),
999.28,
"#9B59B6"
],
[
new Date(2020,4,21,15,40,0),
999.27,
"#9B59B6"
],
[
new Date(2020,4,21,15,41,0),
999.27,
"#9B59B6"
],
[
new Date(2020,4,21,15,42,0),
999.31,
"#9B59B6"
],
[
new Date(2020,4,21,15,43,0),
999.25,
"#9B59B6"
],
[
new Date(2020,4,21,15,44,0),
999.26,
"#9B59B6"
],
[
new Date(2020,4,21,15,45,0),
999.19,
"#9B59B6"
],
[
new Date(2020,4,21,15,46,0),
999.17,
"#9B59B6"
],
[
new Date(2020,4,21,15,47,0),
999.13,
"#9B59B6"
],
[
new Date(2020,4,21,15,48,0),
999.2,
"#9B59B6"
],
[
new Date(2020,4,21,15,49,0),
999.1,
"#9B59B6"
],
[
new Date(2020,4,21,15,50,0),
999.11,
"#9B59B6"
],
[
new Date(2020,4,21,15,51,0),
999.04,
"#9B59B6"
],
[
new Date(2020,4,21,15,52,0),
999.07,
"#9B59B6"
],
[
new Date(2020,4,21,15,53,0),
999.01,
"#9B59B6"
],
[
new Date(2020,4,21,15,54,0),
999.01,
"#9B59B6"
],
[
new Date(2020,4,21,15,55,0),
999.03,
"#9B59B6"
],
[
new Date(2020,4,21,15,56,0),
999.06,
"#9B59B6"
],
[
new Date(2020,4,21,15,57,0),
999.04,
"#9B59B6"
],
[
new Date(2020,4,21,15,58,0),
998.96,
"#9B59B6"
],
[
new Date(2020,4,21,15,59,0),
998.92,
"#9B59B6"
],
[
new Date(2020,4,21,16,0,0),
998.94,
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
function gvisDataAreaChartID76a42aa1202b () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2020,4,21,15,39,0),
514,
"#3DC948"
],
[
new Date(2020,4,21,15,40,0),
516,
"#3DC948"
],
[
new Date(2020,4,21,15,41,0),
518,
"#3DC948"
],
[
new Date(2020,4,21,15,42,0),
521,
"#3DC948"
],
[
new Date(2020,4,21,15,43,0),
520,
"#3DC948"
],
[
new Date(2020,4,21,15,44,0),
523,
"#3DC948"
],
[
new Date(2020,4,21,15,45,0),
526,
"#3DC948"
],
[
new Date(2020,4,21,15,46,0),
528,
"#3DC948"
],
[
new Date(2020,4,21,15,47,0),
526,
"#3DC948"
],
[
new Date(2020,4,21,15,48,0),
526,
"#3DC948"
],
[
new Date(2020,4,21,15,49,0),
523,
"#3DC948"
],
[
new Date(2020,4,21,15,50,0),
513,
"#3DC948"
],
[
new Date(2020,4,21,15,51,0),
507,
"#3DC948"
],
[
new Date(2020,4,21,15,52,0),
502,
"#3DC948"
],
[
new Date(2020,4,21,15,53,0),
509,
"#3DC948"
],
[
new Date(2020,4,21,15,54,0),
516,
"#3DC948"
],
[
new Date(2020,4,21,15,55,0),
517,
"#3DC948"
],
[
new Date(2020,4,21,15,56,0),
519,
"#3DC948"
],
[
new Date(2020,4,21,15,57,0),
522,
"#3DC948"
],
[
new Date(2020,4,21,15,58,0),
523,
"#3DC948"
],
[
new Date(2020,4,21,15,59,0),
525,
"#3DC948"
],
[
new Date(2020,4,21,16,0,0),
528,
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
function gvisDataColumnChartID76a4557db559 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2020,4,21,15,40,0),
4.2,
"#4E89F6"
],
[
new Date(2020,4,21,15,50,0),
4.3,
"#4E89F6"
],
[
new Date(2020,4,21,16,0,0),
4.1,
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
function gvisDataColumnChartID76a447a8b78f () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2020,4,21,15,40,0),
3.8,
"#4E89F6"
],
[
new Date(2020,4,21,15,50,0),
3.9,
"#4E89F6"
],
[
new Date(2020,4,21,16,0,0),
3.7,
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
function drawChartTableID76a44bb5ebeb() {
var data = gvisDataTableID76a44bb5ebeb();
var options = {};
options["allowHtml"] = true;
options["width"] = 600;


    var chart = new google.visualization.Table(
    document.getElementById('TableID76a44bb5ebeb')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartLineChartID76a4629a16ab() {
var data = gvisDataLineChartID76a4629a16ab();
var options = {};
options["allowHtml"] = true;
options["title"] = "Temperature and Humidity";
options["series"] = [{color:'#F6614E', targetAxisIndex:0},
                                  {color:'#4E89F6', targetAxisIndex:1}];
options["vAxes"] = [{title:'Temp. (C)'},{title:'Hum. (%)'}];
options["width"] = 600;


    var chart = new google.visualization.LineChart(
    document.getElementById('LineChartID76a4629a16ab')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartAreaChartID76a449c96c70() {
var data = gvisDataAreaChartID76a449c96c70();
var options = {};
options["allowHtml"] = true;
options["title"] = "Air Pressure";
options["vAxis"] = {title:'(hPa)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.AreaChart(
    document.getElementById('AreaChartID76a449c96c70')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartAreaChartID76a42aa1202b() {
var data = gvisDataAreaChartID76a42aa1202b();
var options = {};
options["allowHtml"] = true;
options["title"] = "CO2 Level";
options["vAxis"] = {title:'(ppm)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.AreaChart(
    document.getElementById('AreaChartID76a42aa1202b')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartColumnChartID76a4557db559() {
var data = gvisDataColumnChartID76a4557db559();
var options = {};
options["allowHtml"] = true;
options["title"] = "PM 10";
options["vAxis"] = {title:'(ug/m3)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.ColumnChart(
    document.getElementById('ColumnChartID76a4557db559')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartColumnChartID76a447a8b78f() {
var data = gvisDataColumnChartID76a447a8b78f();
var options = {};
options["allowHtml"] = true;
options["title"] = "PM 2.5";
options["vAxis"] = {title:'(ug/m3)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.ColumnChart(
    document.getElementById('ColumnChartID76a447a8b78f')
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
callbacks.push(drawChartTableID76a44bb5ebeb);
})();
function displayChartTableID76a44bb5ebeb() {
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
callbacks.push(drawChartLineChartID76a4629a16ab);
})();
function displayChartLineChartID76a4629a16ab() {
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
callbacks.push(drawChartAreaChartID76a449c96c70);
})();
function displayChartAreaChartID76a449c96c70() {
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
callbacks.push(drawChartAreaChartID76a42aa1202b);
})();
function displayChartAreaChartID76a42aa1202b() {
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
callbacks.push(drawChartColumnChartID76a4557db559);
})();
function displayChartColumnChartID76a4557db559() {
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
callbacks.push(drawChartColumnChartID76a447a8b78f);
})();
function displayChartColumnChartID76a447a8b78f() {
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
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableID76a44bb5ebeb"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartLineChartID76a4629a16ab"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartAreaChartID76a449c96c70"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartAreaChartID76a42aa1202b"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartColumnChartID76a4557db559"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartColumnChartID76a447a8b78f"></script>
 
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
  
<div id="TableID76a44bb5ebeb" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
<tr>
<td>

<!-- divChart -->
  
<div id="LineChartID76a4629a16ab" 
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
  
<div id="AreaChartID76a449c96c70" 
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
  
<div id="AreaChartID76a42aa1202b" 
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
  
<div id="ColumnChartID76a4557db559" 
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
  
<div id="ColumnChartID76a447a8b78f" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
</table>
 <div><span>Data: various &#8226; Chart ID: <a href="Chart_MergedID76a485267ab.html">MergedID76a485267ab</a> &#8226; <a href="https://github.com/mages/googleVis">googleVis-0.6.4</a></span><br /> 
<!-- htmlFooter -->
<span> 
  R version 3.5.2 (2018-12-20) 
  &#8226; <a href="https://developers.google.com/terms/">Google Terms of Use</a> &#8226; Data Policy: See individual charts
</span></div>
</body>
</html>
