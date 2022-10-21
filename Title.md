Google Data Analytics Capstone: New car sales 2019-2021. How COVID
impacted the industry?
================
Boris Kosarenkov
2022-10-17

## Ask

In this capstone project, I will explore the new car sales and its COVID
impact. My target is to understand when the industry will be able to
come back to the pre-COVID level of 2019. Stakeholders are Global Supply
Chain Management of one of the major automotive parts manufacturers. The
business task is to analyze the automotive market and help stakeholders
perform demand arbitration and inventory strategy for 2023.

## Prepare

I will use data from “Organisation Internationale des Constructeurs
d’Automobiles” (OICA), The European Automobile Manufacturers’
Association, or ACEA, and The World Bank. This paper is created for
educational, research purposes, which falls under exceptions to French
copyright law, described in Art. L122-5. The World Bank strives to
enhance public access to and use of data that it collects and publishes
([detailed terms of
use](https://www.worldbank.org/en/about/legal/terms-of-use-for-datasets))

- Data-sets & citations:

  - Global Sales - All Vehicles from OICA, [OICA web-site](www.oica.net)

  - Vehicle sales mirror economic growth (2008-2021 trend), [ACEA
    web-site](www.acea.auto)

  - The Wrold Bank: GDP growth (annual %),[The World Bank
    web-site](data.worldbank.org)

## Process

For Data processing, cleaning and analyze I will use Excel and R studio
cloud. Excel is chosen as it fits very well for initial review of the
data and making assumptions. I have significant experience with Excel,
so it is faster and easier for me to make a quick initial data review. R
programming language and R studio IDE is chosen because it has great
capabilities in both data processing, transformation, and visualization.
R markdown format allows to output professional reports in HTML. Same
analyze and visualization could have been performed fully in Excel, or
in Google Big Query (using SQL) and Google data studio or Tableu for
visualization.

Technical documentation logging cleaning and manipulation of data is
available on
[Kaggle](https://www.kaggle.com/code/boriskosarenkov/google-data-analytics-car-sales-and-covid-impact)

## Analyze

I have prepared two data-sets. I used excel to delete and or modify
column names, delete unnecessary visual formatting, and to save data
sets as CSV files. In the next step I’m using R to load those CSV files
into IDE. I use tidyverse package to manipulate data in R, I had to
pivot longer one of the data sets in order to be able to build the
required visualization. I use DT package to make the advanced visual
output of the resulting tables. For charts, I use ggplot2 with a style
package created by [BBC bbplot package](https://github.com/bbc/bbplot).

First data set: Global Sales - All Vehicles

- It contains new vehicle sales per country and region for the period
  2019 - 2021

<div id="htmlwidget-82a8c4d5f22a3d6c8296" style="width:100%;height:auto;" class="datatables html-widget"></div>
<script type="application/json" data-for="htmlwidget-82a8c4d5f22a3d6c8296">{"x":{"filter":"top","vertical":false,"filterHTML":"<tr>\n  <td><\/td>\n  <td data-type=\"character\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"character\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"number\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n    <div style=\"display: none;position: absolute;width: 200px;opacity: 1\">\n      <div data-min=\"44977\" data-max=\"25796931\"><\/div>\n      <span style=\"float: left;\"><\/span>\n      <span style=\"float: right;\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"number\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n    <div style=\"display: none;position: absolute;width: 200px;opacity: 1\">\n      <div data-min=\"29663\" data-max=\"25311069\"><\/div>\n      <span style=\"float: left;\"><\/span>\n      <span style=\"float: right;\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"number\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n    <div style=\"display: none;position: absolute;width: 200px;opacity: 1\">\n      <div data-min=\"34472\" data-max=\"26274820\"><\/div>\n      <span style=\"float: left;\"><\/span>\n      <span style=\"float: right;\"><\/span>\n    <\/div>\n  <\/td>\n<\/tr>","data":[["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","31","32","33","34","35","36","37","38","39","40","41","42","43","44","45","46","47","48","49","50","51","52","53","54","55","56","57","58","59","60","61","62","63"],["europe","europe","europe","europe","europe","europe","europe","europe","europe","europe","europe","europe","europe","europe","europe","europe","europe","europe","europe","europe","europe","europe","europe","europe","europe","europe","europe","europe","america","america","america","america","america","america","america","america","america","america","america","asia-oceania","asia-oceania","asia-oceania","asia-oceania","asia-oceania","asia-oceania","asia-oceania","asia-oceania","asia-oceania","asia-oceania","asia-oceania","asia-oceania","asia-oceania","asia-oceania","asia-oceania","asia-oceania","asia-oceania","asia-oceania","asia-oceania","asia-oceania","africa","africa","africa","africa"],["austria","belgium","bulgaria","croatia","czech republic","denmark","finland","france","germany","greece","hungary","ireland","italy","netherlands","norway","poland","portugal","romania","slovakia","spain","sweden","switzerland","united kingdom","other countries","russia","turkey","ukraine","other countries/regions","canada","mexico","united states of america","argentina","brazil","chile","colombia","ecuador","peru","puerto rico","other countries/regions","australia","china","india","indonesia","israel","japan","kazakhstan*","kuwait","malaysia","new zealand","pakistan","philippines","saudi arabia","south korea","taiwan","thailand","united arab emirates","uzbekistan","vietnam","other countries/regions","egypt","morocco","south africa","other countries/regions"],[371934,642000,44977,73862,281423,264073,133505,2755728,4017059,122990,190090,145104,2132630,538739,189824,656258,265827,189504,113863,1501244,418478,352968,2736559,285560,1778841,491947,102542,133187,1976440,1360008,17488154,452200,2787850,348575,248689,119197,155507,101928,346376,1062867,25796931,3816858,1030486,268220,5195216,71818,112633,604287,149293,187714,410406,533904,1795134,425000,1007552,232305,197103,281262,534707,170568,165916,532898,328464],[301617,509994,29663,43800,228834,233271,112988,2100030,3266759,88710,153978,112122,1564756,427162,180592,510153,173989,145507,84909,1030746,330215,269391,1964660,215910,1631163,796150,98986,106843,1586474,977650,14881356,334316,2058437,258835,173121,78187,108999,103487,253970,916968,25311069,2938575,532077,226338,4598615,89202,85287,529434,115435,124429,244178,452544,1905972,444161,792146,158711,195000,262823,399580,219732,133308,372633,198373],[306176,462536,34472,54330,236221,221937,115291,2142284,2973319,112364,150387,136126,1664483,405061,217572,554613,183390,144222,87349,1034063,343880,272249,2044091,237203,1741965,772722,121772,96819,1704850,1046705,15408565,370283,2119851,415582,229493,109707,152856,105349,337911,1049831,26274820,3759398,887205,306012,4448340,113600,100157,508911,159636,237424,286734,556559,1734581,422000,748580,188844,184500,260850,435754,277805,175435,464493,227274]],"container":"<table class=\"display\">\n  <thead>\n    <tr>\n      <th> <\/th>\n      <th>regions<\/th>\n      <th>countries<\/th>\n      <th>ytd_2019<\/th>\n      <th>ytd_2020<\/th>\n      <th>ytd_2021<\/th>\n    <\/tr>\n  <\/thead>\n<\/table>","options":{"columnDefs":[{"className":"dt-right","targets":[3,4,5]},{"orderable":false,"targets":0}],"order":[],"autoWidth":false,"orderClasses":false,"orderCellsTop":true}},"evals":[],"jsHooks":[]}</script>

- It allows me (after some pivoting) to build a column chart
  representing the drop in sales in 2020

<!-- -->

    ## Warning in grid.Call(C_stringMetric, as.graphicsAnnot(x$label)): семейство
    ## шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_stringMetric, as.graphicsAnnot(x$label)): семейство
    ## шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_stringMetric, as.graphicsAnnot(x$label)): семейство
    ## шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

![](Title_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->

Second data set: GDP growth correlation with new vehicle sales

- It was made using data from The World Bank for GDP annual growth and
  data from OICA for vehicle sales. An article from ACEA provided the
  insight that correlation exists

<div id="htmlwidget-a2c1a1a8572342231044" style="width:100%;height:auto;" class="datatables html-widget"></div>
<script type="application/json" data-for="htmlwidget-a2c1a1a8572342231044">{"x":{"filter":"top","vertical":false,"filterHTML":"<tr>\n  <td><\/td>\n  <td data-type=\"number\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n    <div style=\"display: none;position: absolute;width: 200px;opacity: 1\">\n      <div data-min=\"2011\" data-max=\"2023\"><\/div>\n      <span style=\"float: left;\"><\/span>\n      <span style=\"float: right;\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"number\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n    <div style=\"display: none;position: absolute;width: 200px;opacity: 1\">\n      <div data-min=\"-23.7\" data-max=\"11.5\" data-scale=\"1\"><\/div>\n      <span style=\"float: left;\"><\/span>\n      <span style=\"float: right;\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"number\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n    <div style=\"display: none;position: absolute;width: 200px;opacity: 1\">\n      <div data-min=\"-6\" data-max=\"5.4\" data-scale=\"1\"><\/div>\n      <span style=\"float: left;\"><\/span>\n      <span style=\"float: right;\"><\/span>\n    <\/div>\n  <\/td>\n<\/tr>","data":[["1","2","3","4","5","6","7","8","9","10","11","12","13"],[2011,2012,2013,2014,2015,2016,2017,2018,2019,2020,2021,2022,2023],[-1.1,-10.5,-3.9,4.8,10,7.8,5.4,1.6,1.9,-23.7,-2.4,-0.6,11.5],[1.9,-0.7,0,1.6,2.3,2,2.8,2.1,1.8,-6,5.4,2.9,3]],"container":"<table class=\"display\">\n  <thead>\n    <tr>\n      <th> <\/th>\n      <th>Period<\/th>\n      <th>Sales<\/th>\n      <th>GDP_annual_growth<\/th>\n    <\/tr>\n  <\/thead>\n<\/table>","options":{"columnDefs":[{"className":"dt-right","targets":[1,2,3]},{"orderable":false,"targets":0}],"order":[],"autoWidth":false,"orderClasses":false,"orderCellsTop":true}},"evals":[],"jsHooks":[]}</script>

- Line chart helps to demonstrate the assumed correlation

<!-- -->

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call.graphics(C_text, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

    ## Warning in grid.Call(C_textBounds, as.graphicsAnnot(x$label), x$x, x$y, :
    ## семейство шрифтов не найдено в базе данных шрифтов Windows

![](Title_files/figure-gfm/unnamed-chunk-5-1.png)<!-- -->

## Act

- Data shows almost 24% drop in new car sales in 2020 comparing to 2019.
  The reduction is related to COVID pandemic impact on customer demand
  and on the whole automotive supply chain. Car manufacturers and
  component suppliers suffered production shutdowns due to quarantines.
- Data shows that there is an above average correlation between car
  sales and GDP growth. See chart.  
- On the same chart we can see that in 2020 car sales “overreact” - drop
  significantly lower in comparison to the decline in actual economic
  emissions (GDP). “Overreaction” can be caused by:  
  - Panic of consumers  

  - Showrooms closed  

  - Manufacturer’s production output reduced due to crisis in supply
    chain  
- World Bank estimates only 3.5% annual growth of GDP in 2023 and
  in 2024. With such pace market will comeback top the 2019 (pre-COVID)
  levels on in 2024

If stakeholders get a demand forecast from car makers (their customers)
which contradicts above described insights, and for example shows sales
growth above 3-4% next year it should raise questions for further
analysis:

- Is this carmaker or vehicle model outpacing the market? Did it ever
  before?

- Is the region model is targeted for outpacing the market? For example,
  China is and it is estimated that it will in 2023 as well.

If none of the above is true I suggest stakeholders to be conservative
in their demand arbitration process for 2023, so they could avoid
overstocking.
