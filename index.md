---
title       : simplePlot
subtitle    : A simple data plotting Shiny App
author      : Mark Evans
job         : XOMA
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
---

## simplePlot

<b>simplePlot is a great little application that allows users to upload a simple text data file and plot it.</b>
- Guidelines
    1. Input file may be comma or tab-seperated
    2. Input file must have three columns
    3. First column will be used for values of the x-axis
    4. Second and third columns will contain y-axis values
    5. Input file may or may not have a header row
 
- Once the file has been uploaded, click the 'Plot Data' tab to show the graph
- Add labels to the X and Y axes and provide a title

--- .class #id 

## Example of Input file
|Days|Antigen1|Antigen2|
|--- |:------:| ------:|
|1   |12      |5       |
|2   |24      |10      |
|3   |33      |15      |
|4   |45      |20      |
|5   |51      |25      |
|6   |60      |30      |
|7   |73      |35      |
|8   |80      |40      |
|9   |90      |45      |
|10  |98      |50      |

--- .class #id

## Example of the Output graph

```r
plot(a$v2~a$v1, xlab="Days", ylab="Antigen values", main="Antigen values vs. Days")
```

![plot of chunk unnamed-chunk-2](assets/fig/unnamed-chunk-2-1.png) 

--- .class #id

## Demo of simplePlot
Please feel free to follow the link below and give it a try!

http://talonsensei.shinyapps.io/simplePlot
