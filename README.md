# Deep Learning for Post-Processing Ensemble Weather Forecasts

This repository contains the code and supporting materials for the project **“Deep Learning for Bias Correction of Ensemble Weather Forecast Post-Processing”**, which explores the use of neural network models to improve the calibration and skill of ensemble-based weather forecasts.

This study uses a batch-based workflow on Google Colab to process the large datasets using GPU acceleration. Model training and inferenece are divided into sequential batch runs, chunks are executed concurrently and results aggregated across runs for evaluation. This approach allows for scaling the experiments efficiently despite compute limitations.

> **Note:** The dataset used in this project is not publicly available and cannot be shared. Please refer to the accompanying write-up for a detailed discussion of the data, methods, and results.

---

## Contents

- **`CNN_Bias_Correction.ipynb`** — Jupyter notebook containing the code implementation, model training, and evaluation procedures.
- **`Deep Learning in Post Processing.pdf`** — Full project report describing methodology, background, experiments, and findings.

## Project Overview

Ensemble weather prediction systems produce a set of forecasts to capture forecast uncertainty. However, these raw ensembles often exhibit systematic biases and dispersion errors. Statistical post-processing can help correct these issues. This project investigates a deep learning approach to post-processing, aiming to:

- Improve calibration of ensemble forecasts  
- Reduce forecast error  
- Provide a flexible, learnable mapping from raw ensemble predictions to improved probabilistic forecasts

Key features of this work include:

✅ A neural network–based post-processing framework  
✅ Comparison with traditional post-processing methods  
✅ Evaluation using standard ensemble forecast verification metrics

## How to Read This Repository

This repository is intended to accompany the write-up for transparency and documentation purposes. While the dataset cannot be shared due to licensing restrictions, the code and notebook are provided to demonstrate the modeling approach, feature engineering, and evaluation workflow.  

You can explore the following files:

- **`CNN_Bias_Correction.ipynb`** — Shows the end-to-end deep learning post-processing pipeline on ensemble weather forecasts, including architecture design, training loops, and evaluation steps.
- **`Deep Learning in Post Processing.pdf`** — Provides detailed background, methodology, results, and discussion.

If you wish to apply these methods to your own data, you can adapt the code by replacing the data-loading sections in the notebook with your own ensemble forecast data.
