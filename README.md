
<!-- README.md is generated from README.Rmd. Please edit that file -->

# HultenRangeMaps miniCRAN, June 2025

<!-- badges: start -->
<!-- badges: end -->

This ‘mini’ repository has been set up to insure reproducability of the
package
[HultenRangeMaps](https://github.com/ArnellM/HultenRangeMaps.git). The
repository contains all packages that the functions in HultenRangeMaps
require. First, download the repository to your computer. Then, install
the packages from your local repository using the code below.

``` r
# list of packages that the functions in HultenRangeMaps require
pkgs <- c("dplyr", "gdalUtilities", "geojsonio", "gtools", "igraph", "jpeg", "raster", "sf", "terra", "tidyr")

# path to where you have downloaded the local miniCran repository
pth <- "C:/miniCran/HultenRangeMaps_miniCRAN_June2025"

# install packages from your local miniCRAN repository
install.packages(pkgs, 
                 repos = paste0("file:///", pth),
                 type = "source")

# install HultenRange maps
library(devtools)
install_github("ArnellM/HultenRangeMaps")
library(HultenRangeMaps)
```
