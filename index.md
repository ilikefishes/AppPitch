---
title       : Player Value Calculator
subtitle    : Project for Developing Data Products
author      : Devan S.
job         : Data Scientist (In-Training!)
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---



## Introduction
Have you ever wanted to determine the player value of a member of the Edmonton 
Oilers NHL hockey team?
<br><br>
<b>NOW YOU CAN!</b>
<br><br>
Introducing the Edmonton Oilers Value Calculator for the 2016 NHL Season!  

https://ilikefishes.shinyapps.io/PlayerValue/

---

## App Functionality
This groundbreaking new app allows you to select any two Edmonton Oilers players 
and compare their player value score using a custom value calculator function!
<br><br>
Want to discover which of the Four 1st Overall picks of the last 6 years had the
best season?
<br><br>
<b>NOW YOU CAN!</b>  
<br>The app uses the following revolutionary formula to calculate a custom value
score:

```r
"((G x 3) + (A x 2) + (PM x 1) + (PIM x 0.25) + (PP x 0.5) + (S x 0.4)) / GP"
```
<br>
If you are new to hockey, a breakdown of each category can be found in the 
documentation in the app.

---

## Calculation
A pitch presentation is no fun without some R code calculated and displayed? Right?
<b>RIGHT!</b>  
<br>Let's use an example of last years #1 overall pick and prodigy Connor McDavid.


Connor's Season Stats for 2016

```
##   NUM POS         PLAYER GP  G  A  P PM PIM PP SH GW   S SPCT
## 1  97   C CONNOR MCDAVID 43 15 30 45 -1  16  2  0  4 100   15
```

Connor's Player Value Score

```r
valueCalc(connor)
```

```
## [1] 3.465116
```

---

## Future Improvements

As this is a proof of concept currently, here are the features that will be added
as the app progresses.

1. All 30 NHL Teams (not just the Oilers!)
2. Stats for the last 10 NHL seasons (not just 2016!)
3. A 3rd tab that will list and sort all players in the NHL by their PVS 
(Player Value Score)  

Thank you for your time in evaluating my app! 

<br><br><br><br>
All code for this presentation can be found at:
www.githublink.com





