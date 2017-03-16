# Metabox
This package is for West Coast Metabolomics Center 2017 Summer Course Statistics Part.


cite:
Wanichthanarak K, Fan S, Grapov D, Barupal DK, Fiehn O. Metabox: A Toolbox for Metabolomic Data Analysis, Interpretation and Integrative Exploration. PloS one. 2017 Jan 31;12(1):e0171046.

Software requirement: [R](https://www.r-project.org/about.html) and [RTools](https://github.com/stan-dev/rstan/wiki/Install-Rtools-for-Windows).
## To Install:
```
#Install dependency packages.
install.packages('devtools', repos="http://cran.rstudio.com/")
library(devtools)
install.packages('opencpu')
library(opencpu)
install.packages("pacman")

#Install WCMC_DA
devtools::install_github("slfan2013/WCMC_DA/WCMC.MasterController")
WCMC.MasterController::update_master()
WCMC.Course2017.STAT::update_childs()
```

## To Launch:
```
library(opencpu);
opencpu$browse("library/WCMC.Course2017.STAT/www");
```

## To update to the newest version (automatically skip the non-updated files): 
```
WCMC.MasterController::update_master()
WCMC.Course2017.STAT::update_childs()
```

#### please note that the first time running will be slow depending on the internet because it needs to download all the dependency packages. 
#### If reporting any bug or requirement, please contact the maintainer through email, slfan at ucdavis dot edu.

This package is built as a wrapper of [metabox](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0171046) [code](https://github.com/kwanjeeraw/metabox).
