
<!-- README.md is generated from README.Rmd. Please edit that file -->
MF.matR
=======

This is a repository of tools to be used for analysis of <i>C. elegans</i> behavioral and calcium imaging data. It's a work in progress intened to mate matlab and R functions.

Installation
------------

You can install the released version of MF.matR from github with:

``` r
devtools::install_github("mikeod38/MF.matR")
#> Using GitHub PAT from envvar GITHUB_PAT
#> Skipping install of 'MF.matR' from a github remote, the SHA1 (e92b1eed) has not changed since last install.
#>   Use `force = TRUE` to force installation
```

Calcium imaging analysis
------------------------

Often we want to both analyze Ca2+ imaging data from multiple worms and generate summary plots. Main function for this is plotGCaMP\_multi(). This function imports either matlab- or imageJ analyzed calcium imagaing date from single worms.

``` r
library(MF.matR)
# CaData <- plotGCaMP_multi(FileFilter = OP50,
#                           genotype = N2,
#                           cue = hexanol,
#                           nls = TRUE,
#                           center_on_pulse = 'OFF',
#                           startPulse = 29.5,
#                           endPulse = 60.5,
#                           show.plots = FALSE,
#                           matlab = TRUE,
#                           folderPath = here::here("extdata","Ca_imaging","mat_format"))

#?MF.matR::plotGCaMP_multi()
```
