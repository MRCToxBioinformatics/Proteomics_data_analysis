Proteomics Data Analysis
================

<!-- badges: start -->

[![License:
MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![R-CMD-check](https://github.com/MRCToxBioinformatics/Proteomics_data_analysis/workflows/R-CMD-check/badge.svg)](https://github.com/MRCToxBioinformatics/Proteomics_data_analysis/actions)
<!-- badges: end -->

The `Proteomics.data.analysis` package was prepared by the MRC
Toxicology unit
[Bioinformatics](https://www.mrc-tox.cam.ac.uk/facilities/bioinformatics)
and [Mass4Tox
Proteomics](https://www.mrc-tox.cam.ac.uk/facilities/proteomics)
facilities to provide training in the basics of proteomics analyses.

It assume the user’s data has been processed by Proteome Discoverer, as
per standard Proteomics facility workflows

Tutorials take the form of Rmarkdown notebooks and can be viewed by
navigating to
<https://mrctoxbioinformatics.github.io/Proteomics_data_analysis/>

To ensure all the neccessary R packages are installed to run the code in
the tutorials, you can install this package

``` r
remotes::install_github("MRCToxBioinformatics/Proteomics_data_analysis", build_vignettes = TRUE, dependencies = TRUE)
```
