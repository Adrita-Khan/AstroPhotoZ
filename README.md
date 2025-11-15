# Photometric Redshifts Estimation

*This project is ongoing and subject to continuous advancements and modifications.*

![Python Version](https://img.shields.io/badge/python-3.8%2B-blue.svg) ![License](https://img.shields.io/badge/license-MIT-blue.svg)

![Galaxy Redshift](https://c02.purpledshub.com/uploads/sites/48/2020/04/Galaxy-Red-Shift-0fbfa50.jpg?webp=1&w=1200)

## Table of Contents
- [Project Overview](#project-overview)
- [Aim](#aim)
- [Features](#features)
- [Requirements](#requirements)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Resources](#resources)
- [Contact](#contact)

## Project Overview

This project focuses on estimating photometric redshifts, which are crucial for studying the large-scale structure of the universe and the distribution of galaxies. It employs Gaussian processes as a flexible non-parametric approach to effectively model uncertainties in photometric data. The project also integrates various data analysis techniques to enhance accuracy and performance, offering a comprehensive framework for photometric redshift estimation and other ML and AI methods, benchmarking between them to observe each method's performance in terms of accuracy and computational time.

![Photometric Redshift vs True Redshift](Assets/Color-plot-for-photometric-redshift-estimation-vs-true-redshift-for-the-galaxy-catalog_W640.jpg)

## Aim

The project aims to test existing methodologies, such as Gaussian processes, to calculate photometric redshifts and mass estimates on a dataset with known redshifts, like Stripe 82X, to validate and benchmark the approach. The results will then be reproduced using the older dataset to ensure consistency and accuracy, demonstrating alignment with published data. 

Once validated, the methodology will be adapted and applied to other wide X-ray fields with incomplete redshift data, such as XMM XXL, while addressing challenges posed by inhomogeneous data coverage. The performance of the approach will be evaluated across datasets with varying depths and completeness to optimize its reliability for diverse datasets. 

Finally, the methodology will be scaled for fields with no redshifts, enabling broader application in X-ray AGN studies and mass estimation while leveraging advanced machine learning techniques.

![Hubble Law Animation](https://astro.wku.edu/astr106/Hubble_law_anim.gif)

## Features

- **Gaussian Process Regression**: Leverage Gaussian processes to estimate redshifts, allowing for a quantifiable measure of uncertainties
- **Data Handling and Preprocessing**: Tools for cleaning and preparing synthetic datasets based on the Sloan Digital Sky Survey (SDSS)
- **Advanced Data Analysis**: Combines Gaussian processes with other statistical and machine learning techniques to enhance predictive power
- **Visualization Tools**: Includes tools for visualizing redshift distributions, error margins, and overall model performance
- **Thorough Documentation**: Detailed explanations and example notebooks for easy understanding and reproducibility

## Requirements

**Python Version**: Python 3.8+

**Key Packages**:

| Category | Packages |
|----------|----------|
| **Core Scientific Libraries** | NumPy, Pandas, SciPy |
| **Machine Learning & Statistical Modeling** | Scikit-Learn, GPflow |
| **Visualization Tools** | Matplotlib, Seaborn |
| **Astronomy-Specific Tools** | Astroquery, Astropy |
| **Deep Learning (Optional)** | TensorFlow |
| **Utilities** | tqdm, h5py |

## Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/Adrita-Khan/AstroPhotoZ.git
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Run Example Notebooks

To help you get started with the project, you can run the following example notebooks:

| Notebook | Description |
|----------|-------------|
| [`Photometric_Redshift_Dataset_Exploration.ipynb`](EDA/Photometric_Redshift_Dataset_Exploration.ipynb) | An exploratory analysis of the photometric redshift dataset to understand underlying patterns and features |
| [`Synthetic_Photometric_Redshift_Predictor.ipynb`](Simulated%20Data%20Analysis/Notebooks/Synthetic_Photometric_Redshift_Predictor.ipynb) | A step-by-step guide to predicting photometric redshifts using synthetic data |
| [`Sample_Galaxy_Redshift_Prediction_py.ipynb`](Redshift_Analysis/Sample_Galaxy_Redshift_Prediction_py.ipynb) | An example notebook for predicting galaxy redshifts using real data |

## Usage

Follow the notebooks to apply Gaussian processes and other data analysis techniques to photometric data. Hyperparameters and methods can be adjusted to suit specific research requirements. Notebooks and scripts will be updated and shared as the work progresses.

## Contributing

Contributions are welcome! Please feel free to open issues, suggest improvements, or submit pull requests.

## License

This project is licensed under the MIT License.

## Resources

### Tutorials and Demonstrations

| Resource | Description |
|----------|-------------|
| [Scikit-Learn Astronomy Regression Tutorial](https://ogrisel.github.io/scikit-learn.org/sklearn-tutorial/tutorial/astronomy/regression.html) | Regression tutorial for astronomy applications |
| [Photo-z Regression Demo - Mofokeng Chaka](https://github.com/mofokeng-chaka/Classification-Photo-z_Regression_Demo) | Classification and photo-z regression demonstration |
| [Multi-Wavelength Classification and Regression](https://github.com/mofokeng-chaka/Classification-Photo-z_Regression_Demo/blob/master/Multi-Wavelength_Classification_and_Regression.ipynb) | Multi-wavelength approach to classification and regression |
| [PhotoZ_SDSS by Tasos Theodoropoulos](https://github.com/TasosTheodoropoulos/Photoz_SDSS) | SDSS photo-z estimation implementation |
| [TITAN Project - PhotoZ SDSS ML](https://github.com/TITAN-Project-EU/PhotoZ_SDSS_ML) | Machine learning approaches for SDSS photo-z |
| [Photometric Redshifts - Martian Side of the Moon](https://github.com/martiansideofthemoon/Photometric-Redshifts) | Photometric redshift estimation project |
| [Photometric Redshift Estimation - Amber](https://github.com/AstronomerAmber/Machine-Learning) | Machine learning for photometric redshifts |
| [Photometric Redshift Estimation by Qbeer](https://qbeer.github.io/photometric-redshift-estimation/) | Comprehensive photo-z estimation guide |
| [MLZ: Machine Learning Redshifts](https://github.com/mgckind/MLZ) | Machine learning framework for redshift estimation |

### AstroML Resources

| Resource | Description |
|----------|-------------|
| [AstroML - Forest Photometric Redshift Estimation](https://www.astroml.org/book_figures/chapter9/fig_photoz_forest.html) | Random forest photo-z estimation examples |
| [Photo-z using k-Nearest Neighbors](https://www.astroml.org/examples/learning/plot_neighbors_photoz.html) | KNN-based photo-z estimation |
| [Compute SDSS PCA](https://www.astroml.org/examples/datasets/compute_sdss_pca.html) | Principal component analysis on SDSS data |

### Deep Learning

| Resource | Description |
|----------|-------------|
| [Photometric Redshift Using Deep Learning - Shreever Shith](https://github.com/shreevershith/EstimationOfPhotometricRedshiftUsingDL) | Deep learning approaches for photo-z estimation |

### SDSS Data and Tools

| Resource | Description |
|----------|-------------|
| [SDSS4 DR16Q Tutorial by Qiaoya Wu](https://github.com/QiaoyaWu/sdss4_dr16q_tutorial) | Tutorial for SDSS Data Release 16 quasar catalog |
| [SDSS DR8 Data Access](https://www.sdss3.org/dr8/data_access.php) | Data access for SDSS DR8 |
| [SDSS DR9 Photo-z Algorithms](https://www.sdss3.org/dr9/algorithms/photo-z.php) | Photo-z algorithms documentation for DR9 |
| [SDSS DR17 Photo-z Algorithms](https://www.sdss4.org/dr17/algorithms/photo-z/) | Photo-z algorithms documentation for DR17 |
| [sdss Python Package](https://pypi.org/project/sdss/) | Python package for SDSS data access |
| [Astroquery SDSS Documentation](https://astroquery.readthedocs.io/en/latest/sdss/sdss.html) | Astroquery module for SDSS queries |
| [Astroquery SDSS API](https://astroquery.readthedocs.io/en/latest/api/astroquery.sdss.SDSSClass.html) | API documentation for SDSS queries |
| [SDSS DR14 SkyServer SQL Search](https://skyserver.sdss.org/dr14/en/tools/search/sql.aspx) | SQL search interface for DR14 |
| [SDSS DR18 SkyServer SQL Search](https://skyserver.sdss.org/dr18/en/tools/search/sql.aspx) | SQL search interface for DR18 |

### Additional Resources

| Resource | Description |
|----------|-------------|
| [The Dark Energy Survey Data Management System](https://www.researchgate.net/publication/51942136_The_Dark_Energy_Survey_Data_Management_System/figures?lo=1) | Data management insights from the Dark Energy Survey |
| [Understanding Redshift - Sky at Night Magazine](https://www.skyatnightmagazine.com/space-science/redshift) | Comprehensive explanation of redshift in astronomy |
| [Hubble Law Introduction](https://astro.wku.edu/astr106/Hubble_intro.html) | Introduction to Hubble's Law and cosmology |
| [Gaussian Process Regression Tutorial](https://github.com/jwangjie/Gaussian-Process-Regression-Tutorial) | Tutorial on Gaussian process regression |
| [ArXiv Paper: Photo-z Methods](https://arxiv.org/pdf/0910.4393) | Research paper on photometric redshift methods |

---

## Contact

**Adrita Khan**  
[Email](mailto:adrita.khan.official@gmail.com) | [LinkedIn](https://www.linkedin.com/in/adrita-khan) | [Twitter](https://x.com/Adrita_)
