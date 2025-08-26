# MSE AI 2025 - Probabilistic Programming and Bayesian Methods

This repository contains Jupyter notebooks for the MSE AI 2025 course, focusing on probabilistic programming languages (PPLs) and Bayesian methods.

## Notebooks

- **`BayesianLinearRegression.ipynb`** - Comprehensive tutorial on Bayesian linear regression using Pyro
- **`PPLs_Intro.ipynb`** - Introduction to Pyro probabilistic programming language

## Python Environment Setup

### Prerequisites

- Python 3.9 or higher
- pip (Python package installer)
- OR Anaconda/Miniconda (recommended)

### Quick Setup (Recommended)

#### Option 1: Using the Setup Scripts

**On macOS/Linux:**
```bash
chmod +x setup_env.sh
./setup_env.sh
```

**On Windows:**
```cmd
setup_env.bat
```

#### Option 2: Manual Setup with Conda

```bash
# Create conda environment
conda env create -f environment.yml

# Activate the environment
conda activate mse-ai-2025
```

#### Option 3: Manual Setup with pip

```bash
# Create virtual environment
python3 -m venv venv

# Activate virtual environment
source venv/bin/activate  # On macOS/Linux
# OR
venv\Scripts\activate.bat  # On Windows

# Install dependencies
pip install --upgrade pip
pip install -r requirements.txt
```

### Dependencies

The environment includes:

- **Core scientific computing**: numpy, pandas, matplotlib, seaborn
- **Deep learning**: PyTorch
- **Probabilistic programming**: Pyro-PPL
- **Visualization**: pydot, graphviz
- **Jupyter support**: jupyter, ipykernel
- **Additional libraries**: scipy, scikit-learn

### Running the Notebooks

1. **Activate your environment:**
   ```bash
   # If using conda
   conda activate mse-ai-2025
   
   # If using virtual environment
   source venv/bin/activate  # macOS/Linux
   # OR
   venv\Scripts\activate.bat  # Windows
   ```

2. **Start Jupyter:**
   ```bash
   jupyter notebook
   ```

3. **Navigate to the `notebooks/` folder and open the desired notebook**

### Environment Management

#### Updating Dependencies
```bash
# Update all packages
pip install --upgrade -r requirements.txt

# Or update specific packages
pip install --upgrade numpy pandas torch pyro-ppl
```

#### Removing the Environment
```bash
# If using conda
conda env remove -n mse-ai-2025

# If using virtual environment
rm -rf venv  # macOS/Linux
# OR
rmdir /s venv  # Windows
```

## Troubleshooting

### Common Issues

1. **PyTorch installation fails**: Try installing PyTorch separately first:
   ```bash
   pip install torch torchvision torchaudio
   ```

2. **Graphviz issues**: On some systems, you may need to install system-level graphviz:
   ```bash
   # Ubuntu/Debian
   sudo apt-get install graphviz
   
   # macOS
   brew install graphviz
   
   # Windows
   # Download from https://graphviz.org/download/
   ```

3. **SSL context warnings**: The notebooks include SSL context handling, but if you encounter issues, ensure `pyopenssl` is installed.

### Getting Help

If you encounter issues:
1. Check that your Python version is 3.9+
2. Ensure all dependencies are properly installed
3. Try recreating the environment from scratch
4. Check the PyTorch and Pyro documentation for version compatibility

## Course Content

This course covers:
- Introduction to probabilistic programming languages
- Bayesian linear regression
- Variational inference
- Model comparison and evaluation
- Practical applications in machine learning

## License

This project is part of the MSE AI 2025 course curriculum.


