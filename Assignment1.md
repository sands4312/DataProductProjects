---
title: "Interative Map"
author: "Sandesh"
date: "11/1/2019"
output: 
  html_document: 
    keep_md: yes
---

# Interatcive Maps using R Markdown and Leaflets

```r
library(leaflet)
```

```
## Warning: package 'leaflet' was built under R version 3.6.1
```

```r
library(shiny)
```

```
## Warning: package 'shiny' was built under R version 3.6.1
```

```r
my_map <- leaflet() %>% addTiles() 
my_map <- my_map %>% addMarkers(lng=103.7758052, lat=1.3283259, popup="My School")
my_map
```

<!--html_preserve--><div id="htmlwidget-3c51b4d323191d6603e8" style="width:672px;height:480px;" class="leaflet html-widget"></div>
<script type="application/json" data-for="htmlwidget-3c51b4d323191d6603e8">{"x":{"options":{"crs":{"crsClass":"L.CRS.EPSG3857","code":null,"proj4def":null,"projectedBounds":null,"options":{}}},"calls":[{"method":"addTiles","args":["//{s}.tile.openstreetmap.org/{z}/{x}/{y}.png",null,null,{"minZoom":0,"maxZoom":18,"tileSize":256,"subdomains":"abc","errorTileUrl":"","tms":false,"noWrap":false,"zoomOffset":0,"zoomReverse":false,"opacity":1,"zIndex":1,"detectRetina":false,"attribution":"&copy; <a href=\"http://openstreetmap.org\">OpenStreetMap<\/a> contributors, <a href=\"http://creativecommons.org/licenses/by-sa/2.0/\">CC-BY-SA<\/a>"}]},{"method":"addMarkers","args":[1.3283259,103.7758052,null,null,null,{"interactive":true,"draggable":false,"keyboard":true,"title":"","alt":"","zIndexOffset":0,"opacity":1,"riseOnHover":false,"riseOffset":250},"My School",null,null,null,null,{"interactive":false,"permanent":false,"direction":"auto","opacity":1,"offset":[0,0],"textsize":"10px","textOnly":false,"className":"","sticky":true},null]}],"limits":{"lat":[1.3283259,1.3283259],"lng":[103.7758052,103.7758052]}},"evals":[],"jsHooks":[]}</script><!--/html_preserve-->
