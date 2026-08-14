# Microarray and RNA-seq Data

GEO contains both array-based and sequence-based gene expression datasets.

## Microarray

Microarrays measure the expression of predefined genes or transcripts using probes designed to hybridize to specific sequences.

Common microarray platforms include Affymetrix and Agilent.

Typical characteristics:

* Probe-based measurements
* Processed expression values are often available
* Affymetrix raw data are commonly provided as CEL files
* Probe annotation is required to map probes to genes

## RNA-seq

RNA-seq uses high-throughput sequencing to measure RNA molecules and characterize the transcriptome.

Typical characteristics:

* Sequence-based measurements
* Reads are aligned or quantified to produce gene or transcript-level measurements
* Raw sequencing data may be available as FASTQ files
* Processed data may be provided as count matrices or other expression measurements

## Key Difference

| Feature            | Microarray             | RNA-seq                     |
| ------------------ | ---------------------- | --------------------------- |
| Technology         | Hybridization          | Sequencing                  |
| Measurement        | Probe-based            | Read-based                  |
| Raw data example   | CEL                    | FASTQ                       |
| Feature definition | Predefined probes      | Sequenced transcripts/genes |
| Dynamic range      | Generally more limited | Generally broader           |

The choice between microarray and RNA-seq depends on the research question, study design, data availability, and quality of the dataset.
