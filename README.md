# Project 1: Car Similarity Visualization using Multidimensional Scaling (MDS)

## Overview
This project uses **Multidimensional Scaling (MDS)** to visualize the similarities between different car models based on a pairwise distance matrix. The goal is to reduce the data into 2D space to show which cars are most similar.

## Dataset
- Input: A symmetric distance matrix of 9 car models
- Source: Excel
- Example cars: Audi A6, BMW 525i, Porsche Cayman, etc.

## Methodology
- The original pairwise distance matrix was manually entered into Excel
- MDS coordinates were calculated using a supporting tool or visualization software (if available)
- Visual insights were extracted by observing car groupings and proximity

## Tools Used
- Microsoft Excel

## Key Insights
- Similar cars like the Audi A6 and BMW 525i had low distance values and were grouped close together
- Dissimilar cars (e.g., Porsche vs. Suzuki) had high distance values

## How to Use
1. Open the Excel file
2. Review the distance matrix between vehicles
3. Optionally visualize it using any MDS plotting tool (e.g., external app, Power BI, or Excel chart)

---

# Project 2: Personal Loan Classification using k-Nearest Neighbors (k-NN)

## Overview
This Excel project applies the **k-Nearest Neighbors (k-NN)** algorithm to predict whether a customer will accept a personal loan based on demographic and financial variables.

## Dataset
- File: `UniversalBank.xlsx`
- Features include: Age, Income, Experience, Family, CCAvg, Mortgage, CreditCard, etc.
- Target variable: `PersonalLoan` (1 = Yes, 0 = No)

## Methodology
1. Standardized (Z-score) the numeric variables to make them comparable
2. Selected new customers to predict (e.g., ID 4983)
3. Calculated **Euclidean distances** from each new customer to every record in the dataset
4. Found the **5 nearest neighbors**
5. Used **majority voting** among neighbors’ `PersonalLoan` values to make the prediction

## Tools Used
- Microsoft Excel

## Prediction Logic
- If 3 or more of the 5 nearest neighbors have `PersonalLoan = 1` → predict 1
- If the majority have 0 → predict 0

## How to Use
1. Open the Excel file
2. Enter a new (standardized) customer row
3. Calculate distances to all other customers
4. Sort and identify the 5 closest neighbors
5. Use majority vote to determine predicted class

## Example
For customer ID 4983:
- 3 neighbors had `PersonalLoan = 1`
- 2 neighbors had `PersonalLoan = 0`
- → Predicted class: **1**

---

