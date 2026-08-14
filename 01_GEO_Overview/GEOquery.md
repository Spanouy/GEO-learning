# GEOquery and Programmatic Data Access

## What is GEOquery?

GEOquery is an R/Bioconductor package that provides programmatic access to data stored in the NCBI Gene Expression Omnibus (GEO).

It allows researchers to retrieve GEO datasets directly from R instead of downloading and importing files manually.

## Main Uses

GEOquery can be used to:

* Retrieve GEO Series (GSE)
* Access sample information (GSM)
* Access platform information (GPL)
* Retrieve expression data
* Access sample metadata
* Download supplementary files

## Basic Example

```r
library(GEOquery)

gse <- getGEO("GSE27830", GSEMatrix = TRUE)
```

The retrieved object can then be inspected to identify the expression data, sample metadata, and platform information.

## Why Use Programmatic Access?

Programmatic access makes the analysis more:

* Reproducible
* Efficient
* Automatable
* Easier to document

Instead of manually downloading and processing files through the GEO website, the same workflow can be reproduced using R code.
