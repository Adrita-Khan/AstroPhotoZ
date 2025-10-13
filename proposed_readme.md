# Photometric Redshift Estimation Using Machine Learning Approaches

*This research project is currently under active development and subject to ongoing refinements.*

![Python Version](https://img.shields.io/badge/python-3.8%2B-blue.svg) ![License](https://img.shields.io/badge/license-MIT-blue.svg)

## Abstract

This repository presents a comprehensive framework for photometric redshift estimation, a fundamental measurement in extragalactic astronomy and cosmology. The project employs Gaussian Process Regression as a non-parametric Bayesian method to model photometric redshift–spectroscopic redshift relationships while quantifying prediction uncertainties. Through systematic comparison of multiple machine learning algorithms, this work establishes a rigorous benchmarking framework that evaluates model performance in terms of prediction accuracy, computational efficiency, and uncertainty quantification. The methodology is designed for application to wide-field X-ray surveys and deep multi-wavelength astronomical datasets.

![Galaxy Redshift](https://c02.purpledshub.com/uploads/sites/48/2020/04/Galaxy-Red-Shift-0fbfa50.jpg?webp=1&w=1200)

## Research Objectives

This investigation pursues a systematic approach to photometric redshift estimation through the following objectives:

1. **Methodology Validation**: Implement and validate Gaussian Process Regression and complementary machine learning techniques using spectroscopically confirmed samples from the Stripe 82X survey, establishing baseline performance metrics for subsequent applications.

2. **Reproducibility Assessment**: Apply the validated methodology to legacy datasets to demonstrate consistency with previously published photometric redshift catalogs, ensuring algorithmic robustness and reproducibility.

3. **Extension to Sparse Datasets**: Adapt the framework for wide-field X-ray surveys with incomplete spectroscopic coverage, including XMM-XXL, while developing strategies to address inhomogeneous spatial and wavelength coverage.

4. **Multi-Survey Performance Evaluation**: Conduct comparative analysis across surveys of varying depth and completeness to assess methodology scalability and identify optimal application domains.

5. **Application to Uncharacterized Fields**: Deploy the methodology to X-ray selected Active Galactic Nuclei samples lacking spectroscopic redshifts, enabling mass estimation and large-scale structure studies through advanced machine learning techniques.

## Methodology

### Gaussian Process Regression

This project implements Gaussian Process Regression, a Bayesian non-parametric approach that provides:

- Flexible modeling of complex, non-linear relationships between photometric colors and redshift
- Rigorous uncertainty quantification through predictive variance estimates
- Minimal assumptions regarding functional form of the underlying redshift–color relationship

### Data Processing Pipeline

The framework incorporates comprehensive data preprocessing capabilities including:

- Quality control and filtering procedures for multi-wavelength photometric catalogs
- Feature engineering from photometric measurements (colors, magnitudes, errors)
- Treatment of missing data and photometric upper limits
- Standardization protocols aligned with Sloan Digital Sky Survey (SDSS) data products

### Comparative Machine Learning Analysis

Multiple regression algorithms are implemented and benchmarked, including:

- Gaussian Process Regression (primary method)
- Random Forest Regression
- Gradient Boosting Machines
- Neural Network architectures (optional)

Performance is evaluated using standard metrics: root-mean-square error (RMSE), normalized median absolute deviation (σ<sub>NMAD</sub>), outlier fraction, and computational runtime.

### Visualization and Diagnostic Tools

The repository includes publication-quality visualization utilities for:

- Photometric versus spectroscopic redshift comparisons
- Redshift probability distribution functions
- Error analysis and outlier diagnostics
- Feature importance and model interpretability assessments

![Photometric Redshift vs True Redshift](Assets/Color-plot-for-photometric-redshift-estimation-vs-true-redshift-for-the-galaxy-catalog_W640.jpg)

![Hubble Law Animation](https://astro.wku.edu/astr106/Hubble_law_anim.gif)

## Technical Requirements

### System Requirements

- **Python**: Version 3.8 or higher
- **Operating System**: Platform-independent (Linux, macOS, Windows)

### Dependencies

#### Core Scientific Computing
- NumPy: Numerical array operations
- Pandas: Tabular data manipulation
- SciPy: Scientific computing routines

#### Machine Learning and Statistical Modeling
- Scikit-Learn: Classical machine learning algorithms
- GPflow: Gaussian Process modeling with TensorFlow backend

#### Visualization
- Matplotlib: Static plotting library
- Seaborn: Statistical data visualization

#### Astronomical Data Handling
- Astroquery: Astronomical database query interface
- Astropy: Core astronomy data structures and utilities

#### Deep Learning (Optional)
- TensorFlow: Neural network implementations

#### Utilities
- tqdm: Progress monitoring
- h5py: HDF5 data format support

## Installation and Setup

### Repository Access

```bash
git clone https://github.com/Adrita-Khan/AstroPhotoZ.git
cd AstroPhotoZ
```

### Dependency Installation

```bash
pip install -r requirements.txt
```

### Jupyter Notebook Examples

The repository includes comprehensive Jupyter notebooks demonstrating key functionality:

1. **Exploratory Data Analysis**: [`Photometric_Redshift_Dataset_Exploration.ipynb`](EDA/Photometric_Redshift_Dataset_Exploration.ipynb) — Statistical characterization and visualization of photometric redshift training datasets.

2. **Synthetic Data Validation**: [`Synthetic_Photometric_Redshift_Predictor.ipynb`](Simulated%20Data%20Analysis/Notebooks/Synthetic_Photometric_Redshift_Predictor.ipynb) — Methodology validation using simulated photometric observations with known redshift distributions.

3. **Observational Data Application**: [`Sample_Galaxy_Redshift_Prediction_py.ipynb`](Redshift_Analysis/Sample_Galaxy_Redshift_Prediction_py.ipynb) — End-to-end pipeline demonstration using real astronomical survey data.

## Usage Guidelines

The provided notebooks demonstrate the complete workflow from data ingestion through model training, validation, and uncertainty quantification. Hyperparameters, feature selections, and algorithmic choices may be modified to accommodate specific survey characteristics and scientific requirements. Users are encouraged to consult inline documentation and docstrings for detailed implementation guidance.

## Contributions

This project welcomes contributions from the astronomical and data science communities. Potential contributors are encouraged to submit issues for bug reports or feature requests, and to propose improvements through pull requests following standard collaborative development practices.

## License

This software is distributed under the MIT License, permitting unrestricted use, modification, and distribution subject to the terms specified in the LICENSE file.

## References and Resources

### Methodological Tutorials

- Scikit-Learn Astronomy Regression Tutorial: [Link](https://ogrisel.github.io/scikit-learn.org/sklearn-tutorial/tutorial/astronomy/regression.html)
- Classification and Photo-z Regression Demonstrations (Mofokeng Chaka): [Repository](https://github.com/mofokeng-chaka/Classification-Photo-z_Regression_Demo)
- Multi-Wavelength Classification and Regression: [Notebook](https://github.com/mofokeng-chaka/Classification-Photo-z_Regression_Demo/blob/master/Multi-Wavelength_Classification_and_Regression.ipynb)
- SDSS Photometric Redshift Analysis (Tasos Theodoropoulos): [Repository](https://github.com/TasosTheodoropoulos/Photoz_SDSS)
- TITAN Project PhotoZ Implementation: [Repository](https://github.com/TITAN-Project-EU/PhotoZ_SDSS_ML)
- Photometric Redshifts Analysis: [Repository](https://github.com/martiansideofthemoon/Photometric-Redshifts)

### AstroML Library Resources

- AstroML Forest Regression Example: [Documentation](https://www.astroml.org/book_figures/chapter9/fig_photoz_forest.html)
- k-Nearest Neighbors Photo-z Implementation: [Example](https://www.astroml.org/examples/learning/plot_neighbors_photoz.html)
- SDSS Principal Component Analysis: [Example](https://www.astroml.org/examples/datasets/compute_sdss_pca.html)

### Advanced Machine Learning Implementations

- Amber's Machine Learning Approaches: [Repository](https://github.com/AstronomerAmber/Machine-Learning)
- Deep Learning for Photometric Redshifts (Shreever Shith): [Repository](https://github.com/shreevershith/EstimationOfPhotometricRedshiftUsingDL)
- Photo-z Estimation Tutorial (Qbeer): [Website](https://qbeer.github.io/photometric-redshift-estimation/)
- MLZ: Machine Learning for Redshifts: [Repository](https://github.com/mgckind/MLZ)

### SDSS Data Access and Documentation

- SDSS DR16Q Quasar Catalog Tutorial (Qiaoya Wu): [Repository](https://github.com/QiaoyaWu/sdss4_dr16q_tutorial)
- SDSS Data Release 8 Data Access: [Portal](https://www.sdss3.org/dr8/data_access.php)
- SDSS DR9 Photo-z Algorithms: [Documentation](https://www.sdss3.org/dr9/algorithms/photo-z.php)
- SDSS DR17 Photo-z Algorithms: [Documentation](https://www.sdss4.org/dr17/algorithms/photo-z/)
- SDSS Python Package: [PyPI](https://pypi.org/project/sdss/)
- Astroquery SDSS Module: [Documentation](https://astroquery.readthedocs.io/en/latest/sdss/sdss.html) | [API Reference](https://astroquery.readthedocs.io/en/latest/api/astroquery.sdss.SDSSClass.html)
- SDSS SkyServer SQL Interface: [DR14](https://skyserver.sdss.org/dr14/en/tools/search/sql.aspx) | [DR18](https://skyserver.sdss.org/dr18/en/tools/search/sql.aspx)

### Survey Documentation and Theoretical Background

- SDSS DR17 Photometric Redshift Algorithms: [Technical Documentation](https://www.sdss4.org/dr17/algorithms/photo-z/)
- Dark Energy Survey Data Management System: [Publication](https://www.researchgate.net/publication/51942136_The_Dark_Energy_Survey_Data_Management_System/figures?lo=1)
- Redshift in Observational Cosmology: [Article](https://www.skyatnightmagazine.com/space-science/redshift)
- Hubble's Law Introduction: [Educational Resource](https://astro.wku.edu/astr106/Hubble_intro.html)

---

## Contact Information

**Adrita Khan**  
Email: [adrita.khan.official@gmail.com](mailto:adrita.khan.official@gmail.com)  
LinkedIn: [linkedin.com/in/adrita-khan](https://www.linkedin.com/in/adrita-khan)  
Twitter/X: [@Adrita_](https://x.com/Adrita_)

---

*For questions regarding methodology, data access, or collaboration opportunities, please contact the author via email or open an issue in the repository.*
