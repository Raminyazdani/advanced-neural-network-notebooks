# Dataset Documentation

## Regularization Dataset

**File:** `regularization_dataset.csv`

### Format

CSV file with the following structure:
- **Features:** 48 columns (`x0` through `x47`)
- **Target:** 1 column (`y`)

### Placement

Place the CSV file in this directory:
```
advanced-neural-network-notebooks/
└── data/
    └── regularization_dataset.csv  <-- Place here
```

### Usage

The `parameter_norm_penalties.ipynb` notebook loads this dataset to demonstrate L1, L2, and Elastic Net regularization techniques.

### Note on Missing Data

This dataset is not included in the repository. You can:
1. Generate synthetic data with similar characteristics
2. Use any regression dataset with multiple features
3. Adapt the notebook to work with your own data

## MNIST Dataset

The `neural_network_regularization.ipynb` notebook uses the MNIST dataset, which is **automatically downloaded** by PyTorch's `torchvision.datasets.MNIST` on first run. No manual download required.
