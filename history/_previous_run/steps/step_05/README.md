# Advanced Neural Network Regularization Techniques

**Practical implementations of modern regularization methods for neural networks**

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-red.svg)](https://pytorch.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## Overview

Neural networks are powerful but prone to overfitting, especially with limited training data. This repository provides comprehensive Jupyter notebooks demonstrating key regularization techniques that improve model generalization and prevent overfitting.

## What's Inside

This project contains two complementary notebooks:

### 1. Parameter Norm Penalties (`parameter_norm_penalties.ipynb`)
Explores classical regularization techniques for linear models using scikit-learn:
- **L1 Regularization (Lasso)**: Encourages sparsity by driving coefficients to zero, useful for feature selection
- **L2 Regularization (Ridge)**: Shrinks coefficients to prevent overfitting while keeping all features
- **Elastic Net**: Combines L1 and L2 penalties for a balanced approach

### 2. Neural Network Regularization (`neural_network_regularization.ipynb`)
Implements modern deep learning regularization using PyTorch on MNIST:
- **Dropout**: Randomly deactivates neurons during training to prevent co-adaptation
- **Weight Decay**: L2 penalty applied directly in the optimizer
- **Early Stopping**: Halts training when validation performance plateaus

## Tech Stack

- **Python 3.8+**
- **PyTorch 2.0+**: Deep learning framework
- **scikit-learn**: Machine learning utilities and linear models
- **NumPy**: Numerical computing
- **Matplotlib**: Visualization
- **Jupyter Notebook**: Interactive development

## Repository Structure

```
advanced-neural-network-notebooks/
├── parameter_norm_penalties.ipynb        # L1/L2/Elastic Net demonstrations
├── neural_network_regularization.ipynb   # Dropout/weight decay/early stopping
├── data/
│   └── README.md                         # Dataset documentation
├── requirements.txt                      # Python dependencies
└── README.md                             # This file
```

## Setup

### Prerequisites

- Python 3.8 or higher
- pip package manager

### Installation

1. Clone this repository:
```bash
git clone https://github.com/Raminyazdani/advanced-neural-network-notebooks.git
cd advanced-neural-network-notebooks
```

2. (Optional) Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## How to Run

### Starting Jupyter Notebook

```bash
jupyter notebook
```

This will open a browser window. Navigate to and open either:
- `parameter_norm_penalties.ipynb` for classical regularization techniques
- `neural_network_regularization.ipynb` for deep learning regularization

### Running the Notebooks

1. **Parameter Norm Penalties notebook:**
   - **Data required:** Place `regularization_dataset.csv` in the `data/` directory (see Data section below)
   - Run cells sequentially from top to bottom
   - Observe training/validation curves and coefficient analysis

2. **Neural Network Regularization notebook:**
   - **Data required:** MNIST dataset (automatically downloaded on first run)
   - Run cells sequentially from top to bottom
   - Compare regularized vs. unregularized model performance

## Data

### Regularization Dataset (for Parameter Norm Penalties)

**Format:** CSV file with 48 input features (`x0` through `x47`) and one target variable (`y`)

**Placement:** Save as `data/regularization_dataset.csv`

**Note:** This dataset is not included in the repository. If you don't have it, you can:
- Generate synthetic data with similar characteristics
- Use any regression dataset with multiple features (adapt the notebook accordingly)

### MNIST Dataset (for Neural Network Regularization)

The MNIST handwritten digit dataset is **automatically downloaded** by PyTorch when you first run the neural network notebook. No manual download required.

## Outputs

Running the notebooks will generate:

### Parameter Norm Penalties Notebook
- Training and validation MSE curves
- Coefficient magnitude visualizations
- Feature selection analysis (L1 sparsity)
- Model comparison metrics

### Neural Network Regularization Notebook
- Training and validation accuracy/loss curves
- Comparison of dropout rates
- Effect of weight decay on performance
- Early stopping behavior demonstration
- Confusion matrices and sample predictions

## Reproducibility

- Random seeds are set where applicable (`random_seed = 42`)
- Requirements are pinned to major versions for stability
- All paths are relative to the project root

## Troubleshooting

### Import Errors
```bash
pip install --upgrade torch numpy matplotlib jupyter scikit-learn
```

### CUDA/GPU Issues
If you encounter PyTorch CUDA errors:
- Ensure your PyTorch version matches your CUDA version
- Or run on CPU by setting `device = 'cpu'` in the notebooks

### Memory Issues
If notebooks crash due to memory:
- Reduce batch size in the neural network notebook
- Close other applications
- Consider using Google Colab for free GPU access

### Path Issues
All paths in the notebooks are relative to the project root. Run Jupyter from the project root directory:
```bash
cd advanced-neural-network-notebooks
jupyter notebook
```

## Key Concepts Demonstrated

### Overfitting Prevention
- How regularization constrains model complexity
- Bias-variance tradeoff visualization
- Validation curve analysis

### Feature Selection
- L1 regularization driving coefficients to zero
- Identifying important features automatically

### Hyperparameter Tuning
- Grid search for regularization strength
- Cross-validation strategies
- Patience parameter for early stopping

## Contributing

Contributions are welcome! Feel free to:
- Report bugs or issues
- Suggest improvements or additional regularization techniques
- Submit pull requests

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- PyTorch team for the excellent deep learning framework
- scikit-learn contributors for robust ML utilities
- MNIST dataset from Yann LeCun's website

## Contact

For questions or suggestions, please open an issue on GitHub.

---

**Topics:** `neural-networks` `machine-learning` `deep-learning` `regularization` `pytorch` `jupyter-notebook` `dropout` `weight-decay` `l1-regularization` `l2-regularization` `elastic-net` `overfitting-prevention`

