# R course notebooks and analyses

This repository collects R coursework artifacts rather than a single package.
It contains a regression notebook at the root and a separate CS130 causal
inference assignment with its rendered figures and data.

## Contents

- [`Regression Notebook.Rmd`](Regression%20Notebook.Rmd) — source for a CS130
  regression notebook covering logistic regression, treatment-effect contrasts,
  model comparison with leave-one-out cross-validation, and prediction plots.
- [`Regression Notebook.nb.html`](Regression%20Notebook.nb.html) — rendered
  notebook output for browsing without opening RStudio.
- [`Causal Inference/`](Causal%20Inference/) — Fisher randomization inference,
  genetic matching, and synthetic-control coursework. The folder contains the
  source notebook, its rendered HTML, figures, and `greenbuildings.csv`.

## Reproduce or inspect

Open the rendered HTML files for the quickest overview. To work from source,
open the corresponding `.Rmd` file in RStudio or another R Markdown workflow
and install the packages named in its code, including `readxl`, `dplyr`,
`ggplot2`, `glmnet`, `caTools`, `corrplot`, `medicaldata`, `readr`,
`RcppAlgos`, `progress`, and `gtools` as needed by the notebook.

The root regression notebook refers to `regression_1.xlsx`, which is not
included in the current repository tree. A complete rerun therefore requires
that input file; the rendered HTML is the available record of its output.

The causal-inference notebook downloads its teaching data from the URL in the
source notebook. Its matching section also contains an absolute local path to
`greenbuildings.csv`, so that path must be adjusted before rerunning from a
different checkout.