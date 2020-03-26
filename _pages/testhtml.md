---
title: test html
layout: single
permalink: /test/
---

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
 ---
title: test html
layout: single
permalink: /test/
---

c(jsHeader = "<!-- ColumnChart generated in R 3.6.3 by googleVis 0.6.4 package -->\n<!-- Thu Mar 26 16:37:41 2020 -->\n\n\n<!-- jsHeader -->\n<script type=\"text/javascript\">\n", jsData = "\n// jsData \nfunction gvisDataColumnChartID2b146d8b12bf () {\nvar data = new google.visualization.DataTable();\nvar datajson =\n[\n [\nnew Date(2020,2,26,13,30,0),\n2.62,\n\"#5C3292\"\n],\n[\nnew Date(2020,2,26,13,40,0),\n2.64,\n\"#5C3292\"\n],\n[\nnew Date(2020,2,26,13,56,0),\n4.85,\n\"#871B47\"\n],\n[\nnew Date(2020,2,26,14,6,0),\n4.6,\n\"#871B47\"\n],\n[\nnew Date(2020,2,26,14,17,0),\n4.75,\n\"#871B47\"\n],\n[\nnew Date(2020,2,26,14,27,0),\n4.8,\n\"#871B47\"\n],\n[\nnew Date(2020,2,26,14,37,0),\n4.5,\nnull\n],\n[\nnew Date(2020,2,26,14,47,0),\n4.2,\nnull\n],\n[\nnew Date(2020,2,26,14,57,0),\n4.3,\n\"#871B47\"\n],\n[\nnew Date(2020,2,26,15,7,0),\n4.6,\n\"#871B47\"\n],\n[\nnew Date(2020,2,26,15,17,0),\n4,\nnull\n],\n[\nnew Date(2020,2,26,15,27,0),\n4.5,\nnull\n] \n];\ndata.addColumn('datetime','time');\ndata.addColumn('number','PM25');\ndata.addColumn({type: 'string', role: 'style'});\ndata.addRows(datajson);\nreturn(data);\n}\n", 
jsDrawChart = "\n// jsDrawChart\nfunction drawChartColumnChartID2b146d8b12bf() {\nvar data = gvisDataColumnChartID2b146d8b12bf();\nvar options = {};\noptions[\"allowHtml\"] = true;\n\n\n    var chart = new google.visualization.ColumnChart(\n    document.getElementById('ColumnChartID2b146d8b12bf')\n    );\n    chart.draw(data,options);\n    \n\n}\n  \n", jsDisplayChart = "\n// jsDisplayChart\n(function() {\nvar pkgs = window.__gvisPackages = window.__gvisPackages || [];\nvar callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];\nvar chartid = \"corechart\";\n  \n// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)\nvar i, newPackage = true;\nfor (i = 0; newPackage && i < pkgs.length; i++) {\nif (pkgs[i] === chartid)\nnewPackage = false;\n}\nif (newPackage)\n  pkgs.push(chartid);\n  \n// Add the drawChart function to the global list of callbacks\ncallbacks.push(drawChartColumnChartID2b146d8b12bf);\n})();\nfunction displayChartColumnChartID2b146d8b12bf() {\n  var pkgs = window.__gvisPackages = window.__gvisPackages || [];\n  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];\n  window.clearTimeout(window.__gvisLoad);\n  // The timeout is set to 100 because otherwise the container div we are\n  // targeting might not be part of the document yet\n  window.__gvisLoad = setTimeout(function() {\n  var pkgCount = pkgs.length;\n  google.load(\"visualization\", \"1\", { packages:pkgs, callback: function() {\n  if (pkgCount != pkgs.length) {\n  // Race condition where another setTimeout call snuck in after us; if\n  // that call added a package, we must not shift its callback\n  return;\n}\nwhile (callbacks.length > 0)\ncallbacks.shift()();\n} });\n}, 100);\n}\n", 
jsFooter = "\n// jsFooter\n</script>\n", jsChart = "\n<!-- jsChart -->  \n<script type=\"text/javascript\" src=\"https://www.google.com/jsapi?callback=displayChartColumnChartID2b146d8b12bf\"></script>\n", divChart = "\n<!-- divChart -->\n  \n<div id=\"ColumnChartID2b146d8b12bf\" \n  style=\"width: 500; height: automatic;\">\n</div>\n") ---
title: test html
layout: single
permalink: /test/
---

<div><span>Data: data &#8226; Chart ID: <a href="Chart_ColumnChartID2b146d8b12bf.html">ColumnChartID2b146d8b12bf</a> &#8226; <a href="https://github.com/mages/googleVis">googleVis-0.6.4</a></span><br /> ---
title: test html
layout: single
permalink: /test/
---


<!-- htmlFooter -->
<span> 
  R version 3.6.3 (2020-02-29) 
  &#8226; <a href="https://developers.google.com/terms/">Google Terms of Use</a> &#8226; <a href="https://google-developers.appspot.com/chart/interactive/docs/gallery/columnchart">Documentation and Data Policy</a>
</span></div>
</body>
</html>
