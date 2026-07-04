# Data Files

This folder includes the datasets needed to run and review the project.

## Included Files

- `data.csv`: raw online retail transaction dataset used by the notebook.
- `cleaned_rfm_customer_segments.csv`: customer-level RFM output exported from the notebook after RFM scoring and customer segmentation.
- `data_source.txt`: source references for the dataset.

## Source

The dataset is based on the Online Retail transaction dataset used for RFM analysis. Source references are listed in `data_source.txt`.

## Reproducing the Cleaned File

Run the notebook:

```bash
jupyter notebook notebooks/rfm_customer_segmentation_analysis.ipynb
```

The final notebook cell exports:

```text
data/cleaned_rfm_customer_segments.csv
```

This means a cloned copy of the repository already has the data needed to run, while the notebook can still regenerate the cleaned output.
