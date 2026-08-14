# Expression Matrix and Metadata

## Expression Matrix

An expression matrix contains quantitative measurements of gene or transcript expression across multiple biological samples.

In a typical gene expression dataset:

- Rows represent genes, transcripts, or probe sets.
- Columns represent biological samples.
- Values represent expression measurements for each gene or feature in each sample.

For microarray datasets, rows often correspond to probe IDs, which can later be mapped to gene identifiers or gene symbols.

A simplified structure is:

| Feature | Sample 1 | Sample 2 | Sample 3 |
|---------|----------|----------|----------|
| Probe 1 | 8.2 | 7.9 | 9.1 |
| Probe 2 | 5.4 | 5.8 | 5.1 |
| Probe 3 | 10.2 | 9.8 | 10.5 |

The exact meaning and scale of expression values depend on the platform and the preprocessing methods used.

---

## Metadata

Metadata provides descriptive information about the samples and the experimental design.

It helps researchers understand what each sample represents and how samples should be grouped for analysis.

Common metadata fields include:

- Sample ID (GSM)
- Organism
- Tissue or cell type
- Disease status
- Treatment
- Genotype
- Experimental group
- Batch information
- Other biological or clinical characteristics

For example, in a study comparing BRCA1-mutant and BRCA1-non-mutant samples, metadata should allow each sample to be assigned correctly to one of these groups.

---

## Relationship Between Expression Data and Metadata

The expression matrix tells us:

> **What was measured?**

Metadata tells us:

> **Which sample was measured and under what biological or experimental conditions?**

Both are essential for downstream analyses such as differential expression analysis.

The experimental groups defined from metadata are used to construct the statistical design for methods such as `LIMMA`.
