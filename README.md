# Advanced Neural Network Notebooks

A collection of Jupyter notebooks exploring neural network techniques and regularization methods.

## Contents

### 1. Parameter Norm Penalties (`parameter_norm_penalties.ipynb`)
Demonstrates L1, L2, and Elastic Net regularization using scikit-learn.

**Topics covered:**
- L1 Regularization (Lasso) - feature selection through sparsity
- L2 Regularization (Ridge) - coefficient shrinkage
- Elastic Net - combination of L1 and L2

### 2. Neural Network Regularization (`neural_network_regularization.ipynb`)
Implements modern deep learning regularization using PyTorch on MNIST.

**Topics covered:**
- Dropout - random neuron deactivation
- Weight Decay - L2 penalty in optimizer
- Early Stopping - halt training at validation peak

## Tech Stack

- Python 3.8+
- PyTorch 2.0+
- scikit-learn
- pandas
- NumPy
- Matplotlib
- Jupyter Notebook

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

### Data Requirements

**Parameter Norm Penalties notebook:**
- Place `regularization_dataset.csv` in the `data/` directory
- See `data/README.md` for format details

**Neural Network Regularization notebook:**
- MNIST dataset is automatically downloaded on first run
- No manual setup required

More documentation coming soon...
