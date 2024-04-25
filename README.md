---
author:
- Joseph Womersley
bibliography: references.bib
csl: nature.csl
editor: visual
execute:
  echo: false
  error: false
  include: true
  message: false
  warning: false
title: "Defining the Future of Hematopoiesis: Mmrn1 as a Novel Marker
  for Long-Term Hematopoietic Stem Cells"
toc-title: Table of contents
---

```{=html}
<div style="text-align: left;">
  <img src="images/Haemopetic%20stem%20cell%20heirarchy..png" width="800" height="270" alt="Haemopoietic Stem Cell Hierarchy"/>
  <p style="color: gray; font-size: 0.6em;">Laurenti, E. and Göttgens, B. (2018) ‘From haematopoietic stem cells to complex differentiation landscapes’, Nature, 553(7689), pp. 418–426. Available at: https://doi.org/10.1038/nature25022.</p>
</div>
```
Documentation for the project "Defining the Future of Hematopoiesis:
Mmrn1 as a Novel Marker for Long-Term Hematopoietic Stem Cells",
detailing the exploration of the differentiation hierarchy of
hematopoietic stem cells (HSCs) through single-cell RNA-sequencing data
and confirming assumptions using quantitative PCR.

## Project Description

Hematopoietic stem cells (HSCs) are at the apex of the differentiation
hierarchy and defined by their ability to differentiate and produce the
full spectrum of mature blood cells and self-renew to sustain
haematopoiesis. Long-term hematopoietic stem cells (LT.HSCs) sit within
this HSC pool and are of much interest due to their capacity to support
long-term hematopoietic reconstitution[@gur-cohen2016; @notta2011].
Utilising surface markers for these cells has allowed for HSC purities
of more than 50%. However, none have allowed for populations of a single
homogeneous cell type[@adam2005; @kent2009; @zhang2005; @nestorowa2016].

Recently there has been the development of single-cell profiling
techniques which are able to profile transitional cells and resolve the
heterogeneity within these populations at large
numbers[@bendall2014; @jaitin2014; @mahata2014]. This should allow the
identification of novel HSC markers[@nestorowa2016].

We utilised single cell RNA-sequencing data collected by Nesterowa et
al., (2016) which analysed over 1600 single HSPC transcriptomes which
were profiled into LT-HSCs, HSPCs and Progenitor cells using FACS index
sorting and using wide gating to allow for analysis of transitional
cells. This allowed us to find a potential new marker of LT.HSCs.

## Installation

`REPORT::` can be installed using
[`devtools::`](https://devtools.r-lib.org) from GitHub with:

::: cell
``` {.r .cell-code}
usethis::use_course(url = "JoeWomersley/REPORT", destdir = ".")
```
:::

## Regenerating The Analysis

The analysis can be freely reproduced and adapted by simply:

1.  Downloading [R studio and R version](https://www.r-project.org):
    4.3.1 (2023-06-16)

2.  Following the [Installation](#installation) instructions above

3.  Installing [Packages](#packages), listed below

4.  Running the `main.qmd` file

5.  Rendering within the Quarto framework, leveraging the integrated
    **code execution engine**.

6.  This should allow interaction with the plots using the html output.

7.  If you desire to change the raw data set, simply alter the data-raw
    file and change the `Read.csv` function to the new file path. I
    would highlight that the Analysis does include some hard coding to
    alleviate some issues, where hard coding is used there should be
    comments within the code highlighting this.

## Dates

-   **Start Date**: 05/04/24
-   **Last Updated Date**: 23/04/24

## Contact Information

-   **Author**: Joseph Womersley
-   **Email**: JW3723@york.ac.uk

## Technical Description

**R Version**: 4.3.1 (2023-06-16)[@base]

## Contributions

All of the analysis was written with the assistance of Dr Emma
Rand[@rand2023], Co-pilot[@githubc2024a] and chatGPT[@chatgpt2024].

## Packages

-   **Tidyverse (1.3.0)**: A collection of R packages designed for data
    science, offering tools for data manipulation, analysis, and
    visualization. Includes **`dplyr`** for data manipulation and
    **`ggplot2`** for visualization.[@tidyverse]
-   **Patchwork (1.1.3)**: Combines multiple ggplot2 plots into a
    cohesive figure, enhancing data presentation and
    interpretation.[@patchwork]
-   **HtmlTable (2.4.2)** and **DT (0.31)**: Essential for creating
    interactive HTML and dynamic tables within Quarto.[@htmlTable; @DT]
-   **Conflicted (1.2.0)**: To manage namespace conflicts between loaded
    packages.[@conflicted]
-   **Scran (1.28.2)** and **BiomaRt (2.56.1)**: For differential
    analysis of the single-cell RNA-seq data and gene
    annotations.[@scran; @biomaRt]
-   **Bookdown (0.38)**, **Knitr (1.45)**, and **KableExtra (1.4.0)**:
    Facilitate the creation of the documents and report, enabling
    comprehensive documentation of the analysis
    process.[@bookdown; @knitr; @kableExtra]
-   **ggrepel (0.9.4)**: Improves clarity in ggplot2 visualizations by
    preventing text label overlaps.[@ggrepel]
-   **Pheatmap (1.0.12)**: For creating heatmaps with more control over
    aesthetics.[@pheatmap]
-   **Plotly (4.10.4.9000)**: Enables interactive plots that can be
    embedded in web apps or documents.[@plotly]
-   **Readxl (1.4.3)**: Simplifies the process of importing Excel data
    into R, facilitating data integration from diverse sources.[@readxl]

For more information on why specific packages were used and why please
visit: [Supplementary
Methods](./Supplementary_Data_Analysis_Methods.qmd)
