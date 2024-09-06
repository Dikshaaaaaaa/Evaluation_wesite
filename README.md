# Evaluation of E-learning Websites Using Multi-Criteria Decision-Making Approaches

This project evaluates and ranks e-learning websites using various Multi-Criteria Decision-Making (MCDM) approaches, such as TOPSIS (Technique for Order Preference by Similarity to Ideal Solution), WSM (Weighted Sum Model), and WPM (Weighted Product Model). The methods are implemented using MATLAB to determine the best-performing websites based on multiple user-defined criteria.

## Project Overview

The primary objective of this project is to compare and rank e-learning websites based on a set of weighted criteria. The criteria can include factors like usability, content quality, user interface, and more. The project leverages three decision-making models to generate rankings based on different approaches:

1. **TOPSIS**: Calculates the Euclidean distance from the ideal best and worst options and generates a performance score.
2. **WSM (Weighted Sum Model)**: Aggregates the weighted sum of criteria for each website.
3. **WPM (Weighted Product Model)**: Multiplies the weighted product of the criteria to evaluate performance.

## Features

- **Normalization**: All decision matrix values are normalized to ensure consistency across criteria.
- **Weighted Normalization**: Criteria are assigned weights based on importance.
- **TOPSIS Implementation**: Uses Euclidean distance to calculate the proximity of each website to the ideal best and worst.
- **WSM & WPM Implementation**: Provides alternative ranking methods using sum and product of weighted values.
- **MATLAB Code**: The project is entirely coded in MATLAB, including the ranking algorithms for TOPSIS, WSM, and WPM.

## Prerequisites

To run this project, you will need:
- **MATLAB** (Any recent version supporting matrix operations and basic functions)

## Usage

1. Clone the repository or download the source code.
2. Open the MATLAB environment.
3. Load the dataset (criteria matrix `X` and weight vector `W`) into MATLAB.
4. Run the script `topsis.m` for TOPSIS ranking or `wsm_wpm.m` for WSM and WPM rankings.
5. The script will output the normalized matrix, weighted matrix, and the performance score for each website.

### Example Input

A decision matrix `X` containing website evaluation scores and a weight vector `W` representing the importance of each criterion:

```matlab
X = [4 3 5;
     3 4 2;
     5 4 3];
     
W = [0.5 0.3 0.2];  % Weights for each criterion
