---
title: "Coursera_DevelopingDataProducts_Assginment2"
author: "WENCAI"
date: "15 Mai 2019"
output: 
  html_document: 
    keep_md: yes
---



## use the leaflet package to radomly plot the locations in my city


```r
library(leaflet)
set.seed(2019-05-14)
df<-data.frame(lat=runif(20,min=50.90,max=51.00),lng=runif(20,min=6.90,max=7.00))
leaflet()%>%addTiles()%>%addMarkers(lat=df$lat,lng=df$lng)
```

<!--html_preserve--><div id="htmlwidget-ead6f0e22e69baf550e9" style="width:672px;height:480px;" class="leaflet html-widget"></div>
<script type="application/json" data-for="htmlwidget-ead6f0e22e69baf550e9">{"x":{"options":{"crs":{"crsClass":"L.CRS.EPSG3857","code":null,"proj4def":null,"projectedBounds":null,"options":{}}},"calls":[{"method":"addTiles","args":["//{s}.tile.openstreetmap.org/{z}/{x}/{y}.png",null,null,{"minZoom":0,"maxZoom":18,"tileSize":256,"subdomains":"abc","errorTileUrl":"","tms":false,"noWrap":false,"zoomOffset":0,"zoomReverse":false,"opacity":1,"zIndex":1,"detectRetina":false,"attribution":"&copy; <a href=\"http://openstreetmap.org\">OpenStreetMap<\/a> contributors, <a href=\"http://creativecommons.org/licenses/by-sa/2.0/\">CC-BY-SA<\/a>"}]},{"method":"addMarkers","args":[[50.9196595927468,50.9716425996739,50.9362085677683,50.9391077467706,50.981330720149,50.9427959861467,50.9959183329949,50.9726785608102,50.9820187097182,50.9612379388651,50.9119677312905,50.914239548333,50.90262848977,50.9073113046586,50.9981886861613,50.9441976101603,50.9589195064502,50.9335095353192,50.9880257710814,50.9212985362159],[6.99707660712302,6.9909876547521,6.9798499698285,6.97182607715949,6.99113775398582,6.9578127367422,6.94236954532098,6.97906509872992,6.95765683152713,6.91469440392684,6.98605147914495,6.91709353735205,6.91214938787743,6.99149943008088,6.95756950075738,6.9629985174397,6.91214401382022,6.99710714013781,6.94181934436783,6.93286392311566],null,null,null,{"interactive":true,"draggable":false,"keyboard":true,"title":"","alt":"","zIndexOffset":0,"opacity":1,"riseOnHover":false,"riseOffset":250},null,null,null,null,null,{"interactive":false,"permanent":false,"direction":"auto","opacity":1,"offset":[0,0],"textsize":"10px","textOnly":false,"className":"","sticky":true},null]}],"limits":{"lat":[50.90262848977,50.9981886861613],"lng":[6.91214401382022,6.99710714013781]}},"evals":[],"jsHooks":[]}</script><!--/html_preserve-->

So pretty cool with leaflet!
