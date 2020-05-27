---
title: Air Quality at 2020-05-27 21:50:00
layout: single
permalink: /myairq/
---
### The Current Air Quality

<html xmlns="https://www.w3.org/1999/xhtml">
<head>
<title>MergedIDbc45413c95a</title>
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
<!-- Wed May 27 21:50:06 2020 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataTableIDbc4ae1016c () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
26.81,
34.32,
995.23,
652,
3,
2.8
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
function gvisDataLineChartIDbc4f5d6c7d () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2020,4,27,17,44,0),
26.48,
45.51
],
[
new Date(2020,4,27,21,30,0),
27.22,
40.88
],
[
new Date(2020,4,27,21,31,0),
27.24,
40.21
],
[
new Date(2020,4,27,21,32,0),
27.23,
40.05
],
[
new Date(2020,4,27,21,33,0),
27.22,
39.93
],
[
new Date(2020,4,27,21,34,0),
27.21,
38.64
],
[
new Date(2020,4,27,21,35,0),
27.2,
39.32
],
[
new Date(2020,4,27,21,36,0),
27.21,
37.14
],
[
new Date(2020,4,27,21,37,0),
27.21,
38.5
],
[
new Date(2020,4,27,21,38,0),
27.2,
37.85
],
[
new Date(2020,4,27,21,39,0),
27.19,
37.2
],
[
new Date(2020,4,27,21,40,0),
27.16,
35.41
],
[
new Date(2020,4,27,21,41,0),
27.14,
35.85
],
[
new Date(2020,4,27,21,42,0),
27.1,
34.82
],
[
new Date(2020,4,27,21,43,0),
27.08,
35.35
],
[
new Date(2020,4,27,21,44,0),
27.01,
35.46
],
[
new Date(2020,4,27,21,45,0),
26.97,
34.62
],
[
new Date(2020,4,27,21,46,0),
26.92,
33.69
],
[
new Date(2020,4,27,21,47,0),
26.89,
33.94
],
[
new Date(2020,4,27,21,48,0),
26.87,
33.49
],
[
new Date(2020,4,27,21,49,0),
26.84,
33.59
],
[
new Date(2020,4,27,21,50,0),
26.81,
34.32
] 
];
data.addColumn('datetime','time');
data.addColumn('number','Temperature');
data.addColumn('number','Humidity');
data.addRows(datajson);
return(data);
}


// jsData 
function gvisDataAreaChartIDbc45268c4a2 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2020,4,27,17,44,0),
994.96,
"#9B59B6"
],
[
new Date(2020,4,27,21,30,0),
994.91,
"#9B59B6"
],
[
new Date(2020,4,27,21,31,0),
994.87,
"#9B59B6"
],
[
new Date(2020,4,27,21,32,0),
994.91,
"#9B59B6"
],
[
new Date(2020,4,27,21,33,0),
994.9,
"#9B59B6"
],
[
new Date(2020,4,27,21,34,0),
994.9,
"#9B59B6"
],
[
new Date(2020,4,27,21,35,0),
994.88,
"#9B59B6"
],
[
new Date(2020,4,27,21,36,0),
994.92,
"#9B59B6"
],
[
new Date(2020,4,27,21,37,0),
994.9,
"#9B59B6"
],
[
new Date(2020,4,27,21,38,0),
994.86,
"#9B59B6"
],
[
new Date(2020,4,27,21,39,0),
994.97,
"#9B59B6"
],
[
new Date(2020,4,27,21,40,0),
994.9,
"#9B59B6"
],
[
new Date(2020,4,27,21,41,0),
994.98,
"#9B59B6"
],
[
new Date(2020,4,27,21,42,0),
994.96,
"#9B59B6"
],
[
new Date(2020,4,27,21,43,0),
995.01,
"#9B59B6"
],
[
new Date(2020,4,27,21,44,0),
995.1,
"#9B59B6"
],
[
new Date(2020,4,27,21,45,0),
995.1,
"#9B59B6"
],
[
new Date(2020,4,27,21,46,0),
995.11,
"#9B59B6"
],
[
new Date(2020,4,27,21,47,0),
995.16,
"#9B59B6"
],
[
new Date(2020,4,27,21,48,0),
995.2,
"#9B59B6"
],
[
new Date(2020,4,27,21,49,0),
995.19,
"#9B59B6"
],
[
new Date(2020,4,27,21,50,0),
995.23,
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
function gvisDataAreaChartIDbc423665ec9 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2020,4,27,17,44,0),
410,
"#4E89F6"
],
[
new Date(2020,4,27,21,30,0),
824,
"#F6EA4E"
],
[
new Date(2020,4,27,21,31,0),
797,
"#F6EA4E"
],
[
new Date(2020,4,27,21,32,0),
777,
"#F6EA4E"
],
[
new Date(2020,4,27,21,33,0),
759,
"#F6EA4E"
],
[
new Date(2020,4,27,21,34,0),
736,
"#F6EA4E"
],
[
new Date(2020,4,27,21,35,0),
724,
"#F6EA4E"
],
[
new Date(2020,4,27,21,36,0),
710,
"#F6EA4E"
],
[
new Date(2020,4,27,21,37,0),
703,
"#F6EA4E"
],
[
new Date(2020,4,27,21,38,0),
693,
"#3DC948"
],
[
new Date(2020,4,27,21,39,0),
688,
"#3DC948"
],
[
new Date(2020,4,27,21,40,0),
681,
"#3DC948"
],
[
new Date(2020,4,27,21,41,0),
672,
"#3DC948"
],
[
new Date(2020,4,27,21,42,0),
664,
"#3DC948"
],
[
new Date(2020,4,27,21,43,0),
657,
"#3DC948"
],
[
new Date(2020,4,27,21,44,0),
654,
"#3DC948"
],
[
new Date(2020,4,27,21,45,0),
649,
"#3DC948"
],
[
new Date(2020,4,27,21,46,0),
650,
"#3DC948"
],
[
new Date(2020,4,27,21,47,0),
652,
"#3DC948"
],
[
new Date(2020,4,27,21,48,0),
651,
"#3DC948"
],
[
new Date(2020,4,27,21,49,0),
648,
"#3DC948"
],
[
new Date(2020,4,27,21,50,0),
652,
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
function gvisDataColumnChartIDbc466ea1eeb () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2020,4,27,21,30,0),
5.5,
"#4E89F6"
],
[
new Date(2020,4,27,21,40,0),
4.6,
"#4E89F6"
],
[
new Date(2020,4,27,21,50,0),
3,
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
function gvisDataColumnChartIDbc417ea6415 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2020,4,27,21,30,0),
3.6,
"#4E89F6"
],
[
new Date(2020,4,27,21,40,0),
3.1,
"#4E89F6"
],
[
new Date(2020,4,27,21,50,0),
2.8,
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
function drawChartTableIDbc4ae1016c() {
var data = gvisDataTableIDbc4ae1016c();
var options = {};
options["allowHtml"] = true;
options["width"] = 600;


    var chart = new google.visualization.Table(
    document.getElementById('TableIDbc4ae1016c')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartLineChartIDbc4f5d6c7d() {
var data = gvisDataLineChartIDbc4f5d6c7d();
var options = {};
options["allowHtml"] = true;
options["title"] = "Temperature and Humidity";
options["series"] = [{color:'#F6614E', targetAxisIndex:0},
                                  {color:'#4E89F6', targetAxisIndex:1}];
options["vAxes"] = [{title:'Temp. (C)'},{title:'Hum. (%)'}];
options["width"] = 600;


    var chart = new google.visualization.LineChart(
    document.getElementById('LineChartIDbc4f5d6c7d')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartAreaChartIDbc45268c4a2() {
var data = gvisDataAreaChartIDbc45268c4a2();
var options = {};
options["allowHtml"] = true;
options["title"] = "Air Pressure";
options["vAxis"] = {title:'(hPa)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.AreaChart(
    document.getElementById('AreaChartIDbc45268c4a2')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartAreaChartIDbc423665ec9() {
var data = gvisDataAreaChartIDbc423665ec9();
var options = {};
options["allowHtml"] = true;
options["title"] = "CO2 Level";
options["vAxis"] = {title:'(ppm)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.AreaChart(
    document.getElementById('AreaChartIDbc423665ec9')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartColumnChartIDbc466ea1eeb() {
var data = gvisDataColumnChartIDbc466ea1eeb();
var options = {};
options["allowHtml"] = true;
options["title"] = "PM 10";
options["vAxis"] = {title:'(ug/m3)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.ColumnChart(
    document.getElementById('ColumnChartIDbc466ea1eeb')
    );
    chart.draw(data,options);
    

}
  


// jsDrawChart
function drawChartColumnChartIDbc417ea6415() {
var data = gvisDataColumnChartIDbc417ea6415();
var options = {};
options["allowHtml"] = true;
options["title"] = "PM 2.5";
options["vAxis"] = {title:'(ug/m3)'};
options["legend"] = "none";
options["width"] = 600;


    var chart = new google.visualization.ColumnChart(
    document.getElementById('ColumnChartIDbc417ea6415')
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
callbacks.push(drawChartTableIDbc4ae1016c);
})();
function displayChartTableIDbc4ae1016c() {
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
callbacks.push(drawChartLineChartIDbc4f5d6c7d);
})();
function displayChartLineChartIDbc4f5d6c7d() {
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
callbacks.push(drawChartAreaChartIDbc45268c4a2);
})();
function displayChartAreaChartIDbc45268c4a2() {
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
callbacks.push(drawChartAreaChartIDbc423665ec9);
})();
function displayChartAreaChartIDbc423665ec9() {
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
callbacks.push(drawChartColumnChartIDbc466ea1eeb);
})();
function displayChartColumnChartIDbc466ea1eeb() {
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
callbacks.push(drawChartColumnChartIDbc417ea6415);
})();
function displayChartColumnChartIDbc417ea6415() {
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
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartTableIDbc4ae1016c"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartLineChartIDbc4f5d6c7d"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartAreaChartIDbc45268c4a2"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartAreaChartIDbc423665ec9"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartColumnChartIDbc466ea1eeb"></script>


<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartColumnChartIDbc417ea6415"></script>
 
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
  
<div id="TableIDbc4ae1016c" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
<tr>
<td>

<!-- divChart -->
  
<div id="LineChartIDbc4f5d6c7d" 
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
  
<div id="AreaChartIDbc45268c4a2" 
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
  
<div id="AreaChartIDbc423665ec9" 
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
  
<div id="ColumnChartIDbc466ea1eeb" 
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
  
<div id="ColumnChartIDbc417ea6415" 
  style="width: 600; height: automatic;">
</div>

</td>
</tr>
</table>
 <div><span>Data: various &#8226; Chart ID: <a href="Chart_MergedIDbc45413c95a.html">MergedIDbc45413c95a</a> &#8226; <a href="https://github.com/mages/googleVis">googleVis-0.6.4</a></span><br /> 
<!-- htmlFooter -->
<span> 
  R version 3.5.2 (2018-12-20) 
  &#8226; <a href="https://developers.google.com/terms/">Google Terms of Use</a> &#8226; Data Policy: See individual charts
</span></div>
</body>
</html>
