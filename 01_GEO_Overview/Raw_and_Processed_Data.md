# Raw and Processed Data

## Raw Data

Raw data are the measurements generated directly from an experimental platform before the main preprocessing steps.

For example, in Affymetrix microarray experiments, raw data are commonly provided as **CEL files**.

Raw data can be used to perform preprocessing and quality control independently.

Typical preprocessing steps may include:

* Background correction
* Quality control
* Normalization
* Probe summarization
* Probe annotation

---

## Processed Data

Processed data are data that have already undergone one or more preprocessing steps.

In GEO, processed expression data may be provided as a **Series Matrix** or other processed data files.

The exact preprocessing steps depend on the study and platform. Therefore, the GEO record and the original study should be checked to determine how the data were processed.

---

## Raw vs Processed Data

| Feature         | Raw Data                         | Processed Data                    |
| --------------- | -------------------------------- | --------------------------------- |
| Processing      | Minimal or none                  | One or more preprocessing steps   |
| Example         | Affymetrix CEL files             | Series Matrix / expression matrix |
| Quality control | Can be performed independently   | May already have been performed   |
| Normalization   | Usually performed by the analyst | May already be performed          |
| Flexibility     | Higher                           | Depends on available information  |

### Important Consideration

Processed data should not automatically be considered equivalent to normalized data. Before using a processed dataset, researchers should determine which preprocessing and normalization methods were applied.
