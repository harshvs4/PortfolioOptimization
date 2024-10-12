# Portfolio Optimization using LASSO, Ridge, and MinVar Approaches

This repository contains a Jupyter Notebook for building and analyzing various portfolio optimization strategies, including LASSO, Ridge, and Minimum Variance (MinVar) portfolios. The project uses financial data to calculate daily returns, construct portfolios, compute cumulative returns, and evaluate portfolio performance using the Sharpe ratio.

## Table of Contents

- [Project Overview](#project-overview)
- [Installation](#installation)
- [Data](#data)
- [Usage](#usage)
- [Results](#results)
- [License](#license)

## Project Overview

The project implements a rolling-window approach to evaluate different portfolio optimization techniques. Specifically, it computes:

- **LASSO Portfolio**: A portfolio constructed using LASSO regression for regularization.
- **Ridge Portfolio**: A portfolio constructed using Ridge regression.
- **Minimum Variance (MinVar) Portfolio**: A portfolio that minimizes variance with a concentration penalty.
- **Equally-Weighted Portfolio**: A baseline portfolio where all assets are equally weighted.

The results include cumulative returns and risk-adjusted performance (Sharpe ratio) for each portfolio strategy.

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/harshvs4/portfolio-optimization.git
    cd portfolio-optimization
    ```

## Data

The project uses daily trading data from a CSV file containing returns for a set of assets. You can replace this file with your own financial dataset, provided the format is similar (with dates as rows and asset returns as columns).

Make sure your data file is available at the appropriate path when running the notebook.

## Usage

1. **Prepare the data**: 
    Ensure that the dataset is loaded and preprocessed. The notebook includes steps for replacing missing values, normalizing the data, and splitting it into training and test sets.

2. **Run the notebook**:
    The notebook `project.ipynb` walks you through loading the data, calculating portfolio weights, evaluating performance, and plotting the results.

    You can run all the cells in the notebook in sequence to reproduce the results.

## Results

### Sharpe Ratios:
- **LASSO Portfolio**: 0.116
- **Ridge Portfolio**: 0.096
- **MinVar Portfolio**: 0.086
- **Equally-Weighted Portfolio**: 0.062

### Cumulative Return Plot:
- The notebook generates a cumulative return plot comparing LASSO, Ridge, MinVar, and equally-weighted portfolios over the test period.

### Output:
```
Sharpe Ratio (LASSO): 0.11605160669585295
Sharpe Ratio (Ridge): 0.09607737309856637
Sharpe Ratio (MinVar): 0.08588457439399969
Sharpe Ratio (Equally-Weighted): 0.06176881664146324
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
