# README
This README explains how to replicate the results and the order in which to run the notebooks.

## How to replicate the code
Clone the repository and change the working directory of your terminal to the folder.
With Conda installed, run these commands in the terminal:

```bash
conda env create -f environment.yml
conda activate econ230a-nei
jupyter notebook
```

Use the activated environment's Python kernel for all notebooks.

### Data cleaning
First place the data set `NEI_econ230a.csv` into the same folder as the cloned repository.

Only then run `clean_NEI_econ230a.ipynb` from top to bottom, with
`NEI_econ230a.csv` in the same folder.

### Analysis
Then run the three `analyze_*.ipynb` notebooks from top to bottom in any order.
The state and recession analyses use the generated `.parquet` files; the cement policy analysis reads the original CSV.
