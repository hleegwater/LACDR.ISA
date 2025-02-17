# Quarto templates for reproducible scientific scripting

## Overview

This repository contains Quarto templates that can be used for scripting in R. These templates can be matched with templates in an electronic lab journal like [RSpace](https://www.researchspace.com/) and uploaded to RSpace using the [rspacer](https://github.com/burgerga/rspacer) package.

## Install templates directly in RStudio

-   Open RStudio, or a specific R project with [renv](https://rstudio.github.io/renv) for which you want to use these templates.
-   Install the templates using:

``` r
remotes::install_github("LACDR/LACDR.ISA")
```

## Use the Quarto templates

1.  In RStudio, go to File \> New File \> R Markdown.
2.  On the left, click From Template.
3.  Choose either the Investigation, Study or Assay template. Make any edits and perform your analysis. Save the file as a Quarto file (.qmd).
4.  Render the files to reports for reproducible science.
5.  If you want to upload your Investigation, Study or Assay to Rspace, follow the [rspacer instructions](https://burgerga.github.io/rspacer).

## Installation when you want to edit these templates or add custom templates

This repository is meant to be very general for our research institute, the [LACDR](https://www.universiteitleiden.nl/en/science/drug-research). If you and your research group want to have more specific templates or use the same custom workflows, take a look at  [R_templates_dds](https://github.com/hleegwater/R_templates_dds) for some more examples. You can also make your own:

-   Fork or clone this repository.
-   Open the .Rproj project file to open the [R Project](https://bookdown.org/daniel_dauber_io/r4np_book/starting-your-r-projects.html).
-   Edit a template, or add your own and put this in a separate folder in inst/rmarkdown/templates.
-   In the top right panel in RStudio, click on Build, next to the Environment, History.
-   Install.
-   Restart Rstudio.

## Edit a template

-   Templates are stored in skeleton folders and skeleton files within inst/rmarkdown/templates.
-   Each template has its own folder.
-   Edit the skeleton file. Also, check if the YAML file is still matching the skeleton.

## Instructions on how to build templates after changing the skeleton

1.  Save your changes.
2.  In the top right panel in RStudio, click on Build. This is located next to Environment, History, Connections and Tutorial.
3.  Install.
4.  Restart Rstudio.
5.  Don't forget to commit the changes and push to the remote repository if needed!

# Work in progress

Currently (29-06-2024), creating Quarto documents from templates in RStudio is not possible. That is why we decided to use the R Markdown From Template buttons. If this is possible in the future, we aim to update this repository.

This repository is developed in parallel with [rspacer instructions](https://burgerga.github.io/rspacer) and [R_templates_dds](https://github.com/hleegwater/R_templates_dds). It may happen that we forget to include changes in this repository after a new rspacer release. Please let us know if there are any issues!

# References

-   We built this package using the instructions on <https://rstudio4edu.github.io/rstudio4edu-book/rmd-templates.html> part 12.
-   Instructions on <https://rstudio4edu.github.io/rstudio4edu-book/rmd-templates.html> were used to create a template that matches our ISA standards.
