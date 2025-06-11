# GMM vs KDE: Learning 2D Distributions from Samples

This project demonstrates how to learn the underlying distribution of a 2D non-Gaussian dataset using two different techniques:

- **Kernel Density Estimation (KDE)** with Seaborn
- **Gaussian Mixture Models (GMM)** with scikit-learn

We use the `make_moons` dataset as an example of a complex, non-Gaussian distribution.

## Features

- Visual comparison of KDE and GMM estimates
- Demonstrates where KDE struggles and GMM adapts better
- Uses `seaborn`, `sklearn`, and `matplotlib` for plotting and modeling

## Dataset

We generate a synthetic 2D dataset using:

```python
from sklearn.datasets import make_moons
X, _ = make_moons(n_samples=1000, noise=0.05)
