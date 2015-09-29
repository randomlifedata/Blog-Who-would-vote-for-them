# *Who* would vote for *them*?

This R markdown file (article.Rmd) provides text, hyperlinks and R code for producing the blog at RandomLifeData.com titled: Who would vote for them?

## Requirements

The markdown file is intended to be processed by KnitR. To install type the following at your R commandline:

```
install.packages("knitr")
```

Other packages that are required are:
* plyr
* ggplot2
* devtools
* rCharts

For installation of rCharts, you are required first to install devtools and then to download rCharts from GitHub for installation. This can be performed using the following code at the R commandline (or in an R script):

```
install.packages("devtools")
library(devtools)
install_github("rCharts","ramnathv")

# you then need to load the rCharts package before using it:
library(rCharts)
```

One final requirement is the data - the code will automatically collect the CSV file from FigShare. The download location is http://files.figshare.com/2292075/election2015_BBC_Pov_Emp.csv or the DOI link to the data description page is: http://dx.doi.org/10.6084/m9.figshare.1559052

## Instructions

Having installed all the packages, it is simply a case of telling KnitR to process the Rmd file. KnitR can produce PDF, HTML or other formats. For HTML, the code is:

```
knit2html("article.Rmd")
```

When complete, the folder containing article.Rmd will now also contain article.md, article.html and a folder called 'figure' that contains html for each javascript figure and a PNG file for each static figure. 

For uploading to my WordPress site I have manually copied and pasted the text, images and javascript into the various widgets I have installed for those things. There are ways to automatically upload to WordPress but I've not experimented with those yet.

NB: if viewing the webpage on your computer, you'll need to be running a webserver to see the javascript.  

## Links

I recommend checking out the homepage for KnitR here: http://yihui.name/knitr/

Also the rCharts page here: http://rcharts.io/


