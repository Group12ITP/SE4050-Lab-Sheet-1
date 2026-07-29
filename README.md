# SE4050 – Deep Learning Lab 1
## Introduction to Python Libraries for Deep Learning

This repository contains the complete solutions for Lab Sheet 1 of the SE4050 Deep Learning course.
The objective of the lab is to familiarize students with essential Python libraries used in deep learning, including NumPy, Matplotlib, Pandas, and Seaborn.

## 📚 Table of Contents
- [Overview](#overview)
- [Requirements](#requirements)
- [Dataset Information](#dataset-information)
- [Tasks & Solutions](#tasks--solutions)
  - [Task 1 – Basic NumPy & Matplotlib](#task-1--basic-numpy--matplotlib)
  - [Task 2 – Au Nanoparticle Data Analysis](#task-2--au-nanoparticle-data-analysis)
- [Running the Notebook](#running-the-notebook)
- [Results Summary](#results-summary)
- [Submission](#submission)
- [Acknowledgements](#acknowledgements)

## Overview
The lab is split into two main parts:

**Task 1** – Exercises with NumPy and Matplotlib:
- Generate random arrays from exponential distribution.
- Visualise histograms of exponential, uniform, and normal distributions.
- Create a 3D surface plot of \( Z = X^2 + Y^2 \).
- Compute Pearson and Spearman correlations on Pokémon stats and visualise with heatmaps.

**Task 2** – Data analysis with Pandas and Seaborn using the Au nanoparticle dataset:
- Filter the dataset to keep only four features: `N_total`, `N_bulk`, `N_surface`, `R_avg`.
- Display first 20 samples.
- Calculate descriptive statistics (mean, std, quartiles).
- Plot histograms in a 1×4 layout.
- Generate pairplots and custom PairGrid visualisations.

All code is written in a single Jupyter Notebook (`.ipynb`) and can be run in Google Colab or locally.

## Requirements
The code requires the following Python libraries:
- `numpy`
- `matplotlib`
- `pandas`
- `seaborn`
- `scipy` (for correlation)
- `mpl_toolkits.mplot3d` (built‑in with matplotlib)

## Dataset Information
- **Pokémon dataset** – loaded directly from a public GitHub repository:  
  [https://raw.githubusercontent.com/omkarsawant30/Pokemon---Gotta-catch-Em-all-/master/Pokemon.csv](https://raw.githubusercontent.com/omkarsawant30/Pokemon---Gotta-catch-Em-all-/master/Pokemon.csv)
- **Au nanoparticle dataset** – must be downloaded from the provided Google Drive link and uploaded to Colab (or placed in the local directory).  
  [Google Drive folder](https://drive.google.com/drive/folders/1 6- GpmILQB4- 8rMf5oW604pP1Nx54dYx?usp=sharing)

## Tasks & Solutions

### Task 1 – Basic NumPy & Matplotlib
1. **Random 4×4 array**: created using `np.random.exponential()`.
2. **Distribution histograms**: plotted together with adjusted bins and axis limits for clarity.
3. **3D surface plot**: generated using `plot_surface` with a colour map.
4. **Correlation heatmaps**: computed both Pearson and Spearman correlations and displayed with annotated heatmaps.

### Task 2 – Au Nanoparticle Data Analysis
1. **Filtering**: kept only the four specified columns.
2. **First 20 samples**: displayed using `head(20)`.
3. **Descriptive statistics**: calculated mean, standard deviation, and quartiles via `describe()` and custom additions.
4. **1×4 histograms**: plotted each feature in a separate subplot.
5. **Pairplot**: used `sns.pairplot()` with histograms on the diagonal.
6. **Custom PairGrid**:  
   - Diagonal: histogram + KDE.  
   - Upper triangle: bivariate histogram.  
   - Lower triangle: bivariate KDE.
