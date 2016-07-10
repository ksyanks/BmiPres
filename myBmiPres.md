Body Mass Index - Shiny Web Application Pitch Presentation
========================================================
author: KS
date:  Sun Jul 10 14:07:43 2016
autosize: true

Agenda
========================================================

1. Purpose and Information
2. Embedded R Code  
3. Instructions to use

1. Purpose and Information
========================================================
This Shiny application is my submission for the assignment of the course Developing Data Products, part of the Data Science Specialization offered by the Johns Hopkins University. This is an interactive web based application, frameworked in R, for Body Mass Index (BMI) calculation.

BMI is a statistic developed by Adolphe Quetelet in the 1900's for evaluating body mass. It is not related to gender and age. It uses the same formula for men, women and children.


Embedded R Code 
========================================================
BMI is calculated with below sample code

```r
#body weight key in by user
slrBdyKg <- 60

#height key in by user
slrBdyHt <- 160

#Calculate BMI
reBdyBMI <- slrBdyKg/((slrBdyHt/100) * (slrBdyHt/100)) 
print(reBdyBMI)
```

```
[1] 23.4375
```

Instructions to use
========================================================

To reproducing this app locally on your computer, you would need to follow these steps:
  1. Install rstudio if you don't have one.
  2. Install the necessary packages to run RStudio's Shiny server locally, go to this link for more detail: <http://shiny.rstudio.com/articles/shinyapps.html>
  3. Copy server.R, ui.R and README.md files from <https://github.com/ksyanks/BMIshinyapp> to your local. These files (server.R, ui.R and README.md) you find them the above given link at GitHub.
  Please place the files into an directory example, myBMI directory, set your working 1 level above mpg directory. You can launch the app in R with the following commands:

    install.packages("shiny")     
    library(shiny)     
    runApp('myBMI')       

