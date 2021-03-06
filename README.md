# Rsampling-shiny

[Rsampling] (https://github.com/lageIBUSP/Rsampling) is a free and open source package intended for 
teaching and learning about resampling in statistics. Rsampling-shiny is a web-based graphical user interface
written in [shiny] (http://shiny.rstudio.com).

To run, you need to install [R] (http://www.r-project.org/) and the [Rsampling] (https://github.com/lageIBUSP/Rsampling) library.

To install Rsampling, open R and run:
```R
install.packages("devtools")
library(devtools)
install_github(repo = 'lageIBUSP/Rsampling')
```

![ ] (www/chicken.png?raw=true)

## Web version
You can run Rsampling shiny from github! Just open R and run:
```R
install.packages(c("shiny","PerformanceAnalytics"))
library(shiny)
runGitHub(repo="lageIBUSP/Rsampling-shiny")
``` 
and wait for the browser window to open!

## Offline installation
If you need to be able to use Rsampling-shiny without Internet access, download the [latest stable version] 
(https://github.com/lageIBUSP/Rsampling-shiny/releases), 
and extract it to a folder. Then, open R (with the required packages installed, see above) and run
```R
library(shiny)
runApp("<path to Rsampling-shiny>")
```
Remember that you need to install the shiny/shinyBS packages while you have internet access!

## Languages
The app is currently available in English (default) and Portuguese.
To use the version in Portuguese, run the following command 
before running the app (runGitHub(...) or runApp(...))
```R
language <- "pt"
```
## Current features
* Access the Rsampling sample datafiles, or upload your own data in csv format
* Choose between a range of statistics, or write your own R function
* Select your randomization scheme, with or without replacement
* Optional stratified randomization
* Reactive graph showing the distribuion of the statistic of interest and estimated p-value
