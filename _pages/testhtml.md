<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
  "https://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="https://www.w3.org/1999/xhtml">
<head>
<title>ColumnChartID2b146d8b12bf</title>
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
 <!-- ColumnChart generated in R 3.6.3 by googleVis 0.6.4 package -->
<!-- Thu Mar 26 16:37:41 2020 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataColumnChartID2b146d8b12bf () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
new Date(2020,2,26,13,30,0),
2.62,
"#5C3292"
],
[
new Date(2020,2,26,13,40,0),
2.64,
"#5C3292"
],
[
new Date(2020,2,26,13,56,0),
4.85,
"#871B47"
],
[
new Date(2020,2,26,14,6,0),
4.6,
"#871B47"
],
[
new Date(2020,2,26,14,17,0),
4.75,
"#871B47"
],
[
new Date(2020,2,26,14,27,0),
4.8,
"#871B47"
],
[
new Date(2020,2,26,14,37,0),
4.5,
null
],
[
new Date(2020,2,26,14,47,0),
4.2,
null
],
[
new Date(2020,2,26,14,57,0),
4.3,
"#871B47"
],
[
new Date(2020,2,26,15,7,0),
4.6,
"#871B47"
],
[
new Date(2020,2,26,15,17,0),
4,
null
],
[
new Date(2020,2,26,15,27,0),
4.5,
null
] 
];
data.addColumn('datetime','time');
data.addColumn('number','PM25');
data.addColumn({type: 'string', role: 'style'});
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartColumnChartID2b146d8b12bf() {
var data = gvisDataColumnChartID2b146d8b12bf();
var options = {};
options["allowHtml"] = true;


    var chart = new google.visualization.ColumnChart(
    document.getElementById('ColumnChartID2b146d8b12bf')
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
callbacks.push(drawChartColumnChartID2b146d8b12bf);
})();
function displayChartColumnChartID2b146d8b12bf() {
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
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartColumnChartID2b146d8b12bf"></script>
 
<!-- divChart -->
  
<div id="ColumnChartID2b146d8b12bf" 
  style="width: 500; height: automatic;">
</div>
 <div><span>Data: data &#8226; Chart ID: <a href="Chart_ColumnChartID2b146d8b12bf.html">ColumnChartID2b146d8b12bf</a> &#8226; <a href="https://github.com/mages/googleVis">googleVis-0.6.4</a></span><br /> 
<!-- htmlFooter -->
<span> 
  R version 3.6.3 (2020-02-29) 
  &#8226; <a href="https://developers.google.com/terms/">Google Terms of Use</a> &#8226; <a href="https://google-developers.appspot.com/chart/interactive/docs/gallery/columnchart">Documentation and Data Policy</a>
</span></div>
</body>
</html>
