# Spatial-CNN-LSTM-Precipitation
Python code for the paper "Regional Precipitation Forecasting Across Turkey via Spatially-Aware Deep Learning Networks"

"""
=============================================================================
PROJECT TITLE: REGIONAL PRECIPITATION FORECASTING ACROSS TURKEY VIA 
               SPATIALLY-AWARE DEEP LEARNING NETWORKS
AUTHORS:       İbrahim Şanlıalp - Berke Güngörmez
=============================================================================

DESCRIPTION:
This repository contains the Python implementation of the Spatial CNN-LSTM 
architecture proposed in our study. The primary objective of this codebase 
is to predict daily precipitation occurrences (binary classification: dry 
vs. rainy days) across the seven main geographical regions of Turkey. 

To address the "zero-inflated" nature of isolated station data, this study 
utilizes a spatially-aware deep learning framework. The algorithm operates 
on historical precipitation data and regional adjacency matrices, without 
relying on external meteorological variables.

KEY FEATURES IN THIS CODEBASE:
- Data Aggregation: Processing 5-year daily records (2020-2024) from 1803 
  meteorological stations into regional averages.
- Trigonometric Time Encoding: Converting linear calendar days into a 
  cyclical spatial projection using Sine/Cosine transformations.
- Spatial CNN-LSTM Architecture: Utilizing 1D-Convolutional layers (Conv1D) 
  to extract spatial interactions, coupled with LSTM cells to capture 
  temporal memory.
- Regularization: Implementation of Dropout layers, ReLU activation, and 
  chronological train/validation/test splitting to limit data leakage 
  and overfitting.
  
This code is provided to support the methodological transparency of the 
findings presented in the associated academic paper.
=============================================================================
"""
