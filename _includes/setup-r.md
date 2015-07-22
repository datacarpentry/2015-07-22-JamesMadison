**Note:** R and RStudio are separate downloads and installations. **R** is the underlying statistical computing environment, but using R alone is no fun. **RStudio** is a graphical integrated development environment that makes using R much easier. You need R installed before you install RStudio.

1. **Download the gapminder data.** [Click here to download the data](http://bioconnector.org/data/gapminder.csv) that we will use for this section. Save it somewhere you'll remember.
1. **Install R.** You'll need R version 3.2.0 or higher. Download and install R for [Windows](http://cran.r-project.org/bin/windows/base/) or [Mac OS X](http://cran.r-project.org/bin/macosx/) (download the latest R-3.x.x.pkg file for your appropriate version of OS X).
1. **Install RStudio.** Download and install the latest stable version of [RStudio Desktop](http://www.rstudio.com/products/rstudio/download/).
1. **Install R packages.** Launch RStudio (RStudio, *not R itself*). Ensure that you have internet access, then enter the following commands into the **Console** panel (usually the lower-left panel, by default). Note that these commands are case-sensitive. At any point (especially if you've used R/Bioconductor in the past), R may ask you if you want to update any old packages by asking `Update all/some/none? [a/s/n]:`. If you see this, type `a` at the propt and hit `Enter` to update any old packages. If you're using a Windows machine you might get some errors about not having permission to modify the existing libraries -- don't worry about this message. You can avoid this error altogether by running RStudio as an administrator.
1. **Download the data.** [Click here to download the data](etc/gapminder.csv) that we will use for the R lesson. Save it somewhere easy to remember and fine e.g., your Desktop. _(Alternative data source: <http://bioconnector.org/data/gapminder.csv>)_.

```
# Install packages from CRAN
install.packages("dplyr")
install.packages("ggplot2")
install.packages("tidyr")

# Install Bioconductor base
source("http://bioconductor.org/biocLite.R")
biocLite()
```

You can check that you've installed everything correctly by closing and reopening RStudio and entering the following commands at the console window:

```
library(dplyr)
library(ggplot2)
library(tidyr)
library(Biobase)
```

These commands may produce some notes or other output, but as long as they work without an error message, you're good to go. If you get a message that says something like: `Error in library(packageName) : there is no package called 'packageName'`, then the required packages did not install correctly.

