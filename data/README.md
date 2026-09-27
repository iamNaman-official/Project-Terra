# Data

Local datasets used by Project Terra.

## Structure

- `raw/` — Original downloaded datasets
- `processed/` — Cleaned or transformed datasets
- `samples/` — Small datasets that can be safely shared for reproducible experiments

## Data Flow

Raw Data → Processing → Validation → Processed Data → Analysis

## Important

Large NASA datasets should not be committed to Git.

Keep large or downloaded datasets locally and add appropriate paths to `.gitignore`.

Small sample datasets may be committed when they are useful for reproducing experiments.

Every important dataset should have documentation in:

`docs/datasets/`