# Data Directory

This directory should contain the datasets required for the notebooks.

## Required Datasets

### 1. Regularization Dataset (for `parameter_norm_penalties.ipynb`)

**Filename:** `regularization_dataset.csv`

**Description:** Dataset for demonstrating parameter norm penalties (L1, L2, Elastic Net regularization).

**Format:** CSV file with columns:
- `x0` through `x47`: Input features (48 features)
- `y`: Target output variable

**How to Obtain:**
- This dataset should be provided separately or generated
- If you have the dataset, place it in this directory as `data/regularization_dataset.csv`

**Expected Location:** `data/regularization_dataset.csv`

### 2. MNIST Dataset (for `neural_network_regularization.ipynb`)

**Description:** The MNIST handwritten digit dataset is automatically downloaded by PyTorch's `torchvision.datasets.MNIST()` when you run the notebook.

**No manual download required** - the notebook will handle this automatically and cache it in a local directory.

## Notes

- The `.gitignore` file is configured to exclude `*.csv` files from version control to avoid committing large datasets
- Always use relative paths from the project root when accessing data: `data/filename.csv`
- If you need to share datasets, consider using a data hosting service and documenting the download link here
