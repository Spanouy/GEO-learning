# GSE, GSM, GPL and GDS

GEO records are organized into several types of entries, each representing a different level of information.

## GSE — Series

A GSE (GEO Series) represents a research study submitted to GEO. It describes the overall experimental design and contains information about the samples and experimental conditions.

## GSM — Sample

A GSM (GEO Sample) represents an individual biological or experimental sample within a study.

## GPL — Platform

A GPL (GEO Platform) describes the technology or platform used to generate the data, such as an Affymetrix microarray platform.

## GDS — DataSet

A GDS (GEO DataSet) is a curated dataset derived from GEO data and organized for analysis and exploration.

## Relationship

GSE → GSM → GPL

A Series (GSE) contains multiple Samples (GSM), and each sample is associated with a Platform (GPL).
