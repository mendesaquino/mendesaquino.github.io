---
title       : Calculating number of days between two dates
subtitle    : 
author      : Caroline Aquino
job         : Project - Developing Data Products - Coursera
framework   : io2012  # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}


---

## Outline of Project

> 1. Introduction:
The project was performed using shiny and the application was to calculate the number
of days between any two dates given by the user.
> 2. Methods:
Two files were created in order to run the application: ui.R and server.R, available on https://github.com/mendesaquino/project_coursera, and the application can be found online on https://mendesaquino.shinyapps.io/project_course/ 
> 3. Conclusion:
You can use this app whenever you want to calculate the number of days between two dates. 
For instance, you can see how many days until your next birthday, or how many days you have lived so far, or how many days until next Spring.

---

## Application
Here is how the application is displayed:
<img src="assets/fig/unnamed-chunk-1.png" title="plot of chunk unnamed-chunk-1" alt="plot of chunk unnamed-chunk-1" style="display: block; margin: auto;" />

---
- On the left side the user selects the start and end dates. 
- On the right side we can see the dates selected and also the difference in days between those two dates.

Example: Lets see how many days we will have until New Year's Eve.
Using the application, we see that the number of days between 19 June 2014 and 31 December 2014 is 195 days. What R does is to calculate:


```r
# use as.Date( ) to convert strings to dates 
dates <- as.Date(c("2014-06-19", "2014-12-31"))
# number of days between 2014-06-19 and 2004-12-31 
days <- dates[2] - dates[1]; days
```

```
## Time difference of 195 days
```

See the picture on the next slide illustrating the aplication running.

---

<img src="assets/fig/unnamed-chunk-3.png" title="plot of chunk unnamed-chunk-3" alt="plot of chunk unnamed-chunk-3" style="display: block; margin: auto;" />

