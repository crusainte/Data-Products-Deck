---
title       : Airport Arrivals in Singapore
subtitle    : by Country of Embarkation
author      : Yuzhong Yang
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
--- 

## Overview

This data product is created using Air passenger arrival dataset obtained from _Department of Statistics Singapore_.

Using the dataset, a data product is created to allow users to view and explore the dataset.

The dataset is a .csv file that will be read in, cleaned and transform to the following format:


```r
df<-data.frame(countries="Brunei",total="100000")
df
```

```
##   countries  total
## 1    Brunei 100000
```

Lastly, a chart of Top 10 nationality of arrivals at Changi Airport, Singapore, based on a range of year between 1978-2014
will be plotted for trend analysis as well.

---

## Usage Instruction

The Data product can be accessed from the following [link](https://crusainte.shinyapps.io/ShinyApp).

After opening the webpage for the Data Product, you would be able to drag the slider to define the
range of year for which will be used in plotting the chart of top 10 nationality of arrivals. 

Pressing on the submit button after defining the year range will update and plot the chart with
the year range input.

<div style='text-align: center;'>
    <img height='300' src='./assets/img/Steps.JPG' />
</div>

---

## Trend Analysis

Between the 1980 to 1999, majority of the airport arrivals are from Japan and Australia. This has changed
tremedously between 2000 to 2014 where the majority are now made up of arrivals from Indonesia and China.

<div style='text-align: center;'>
<img height='200' src='./assets/img/1980_1999.JPG' />
</div>

<div style='text-align: center;'>
<img height='200' src='./assets/img/after_2000.JPG' />
</div>

---

## Further Improvements

I will be building on the Data Product to show more dimensions and hopefully predict
the Top country of arrival for the upcoming year.
