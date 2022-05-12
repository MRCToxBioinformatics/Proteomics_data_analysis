
<img src="images/UoC_logo.jpg" width="400" hspace="50"/>  <img src="images/MRC_TU_Cambridge_identifier_horizontal_RGB2_a.png" width="300"/> 


- - - -
  
# Proteomics Data Analysis

The Proteomics Data Aanalysis material was prepared by the MRC
Toxicology unit
[Bioinformatics](https://www.mrc-tox.cam.ac.uk/facilities/bioinformatics)
and [mass4tox Proteomics](https://www.mrc-tox.cam.ac.uk/facilities/proteomics) facilities to
provide training in the basics of proteomics analyses.

It assume the user’s data has been processed by Proteome Discoverer, as
per standard Proteomics facility workflows

Tutorials take the form of Rmarkdown notebooks (see links below). If you would like to
contribute or suggest modifications to the material, please see the
[github page](https://github.com/MRCToxBioinformatics/Proteomics_data_analysis)

- - - -
  
### Prerequisites

- #### R
You should be comfortable using `R`. We will be using
base `R` functions like `lapply`, `gsub`, `file.path`, alongside `tidyverse` functions
like `group_by`, `mutate` and `ggplot`. If these are not familiar, we recommend 
undertaking training in `R` and the `tidyverse` beforehand. We recommend using `R>=4.1.2` since
the material has not been tested on version before this.
    
    The [Bioinformatics](https://www.mrc-tox.cam.ac.uk/facilities/bioinformatics) facility
provide separate training covering basic `R`, data carpentry (using the `tidyverse`)
and plotting (using `ggplot2`). If there is not a course scheduled, you can get
recordings by emailing bioinfo@mrc-tox.cam.ac.uk.

    The
[Cambridge Bioinformatics Training](https://bioinfotraining.bio.cam.ac.uk/) 
centre also offer a regular course on
[R for Biologists](https://bioinfotraining.bio.cam.ac.uk/postgraduate/programming/bioinfo-introRbio)

- #### RStudio
The material will be taught in live coding sessions through Rstudio 
and we recommend using this environment whenever you use R. Installation
instructions can be found [here](https://www.rstudio.com/products/rstudio/download/)

- #### Proteomics
The materials herein assume you have attended Cat Franco's
introduction to the principles of bottom-up proteomics by Mass-Spectrometry.

- - - -
  

#### Course dependencies and data
To ensure all the neccessary R packages are installed for you to run the code,
you can install the `Protoemics.data.analysis` package like so:
``` r
remotes::install_github("MRCToxBioinformatics/Proteomics_data_analysis/", build_vignettes = TRUE)
```
This will also install the `Proteomics.analysis.data` package which contains
the data we will use.

- - - -
  
## Course materials
The course is broken into sections for different 'flavours' of quantitative
bottom-up proteomics by Mass-spectrometry. Each section contains a notebook
covering data processing and QC which starts from the Proteome Discoverer (PD)
output files and performs filtering, quality control and data processing to
obtain the desired quantification data from which one can perform further
visualisation or statistical testing. Additional notebooks are included to cover
further topics for each flavour.

#### Label-Free Quantification (LFQ)
- [Data processing and QC](https://mrctoxbioinformatics.github.io/Proteomics_data_analysis/Markdowns/LFQ.html)
- [Comparing robust and maxLFQ summarisation to protein-level abundances](https://mrctoxbioinformatics.github.io/Proteomics_data_analysis/Markdowns/LFQ_maxlfq.html)
- [An alternative normalisation using a prior expectation](https://mrctoxbioinformatics.github.io/Proteomics_data_analysis/Markdowns/LFQ_alternative_normalisation.html)


#### Stable Isotope Labelling by/with Amino acids in Cell culture (SILAC)
- [Data processing and QC](https://mrctoxbioinformatics.github.io/Proteomics_data_analysis/Markdowns/SILAC.html)
- [Differential abundance](https://mrctoxbioinformatics.github.io/Proteomics_data_analysis/Markdowns/SILAC_differential_abundance.html)
- [Incorporation rate testing](https://mrctoxbioinformatics.github.io/Proteomics_data_analysis/Markdowns/SILAC_incorporation.html)

#### Tandem-Mass Tags (TMT)
- [Data processing and QC](https://mrctoxbioinformatics.github.io/Proteomics_data_analysis/Markdowns/TMT.html)






## Additional resources
