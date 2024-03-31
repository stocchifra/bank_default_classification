# bank_default_classification

## Project Overview
This repository contains the analysis of a highly unbalanced dataset, bankPortfolios.csv, which features asset holdings data of 7783 US commercial banks as recorded in their balance sheet for the fourth quarter of 2007. The data was sourced from the Wharton Research Data Services. Each row in the dataset corresponds to a bank, and the columns represent various asset classes and financial indicators.

## Features
The dataset comprises 16 columns of which the first 14 denote various types of investments:

Loans for construction and land development
Loans secured by farmland
Loans secured by 1-4 family residential properties
Loans secured by multi-family (> 5) residential properties
Loans secured by non-farm non-residential properties
Agricultural loans
Commercial and industrial loans
Loans to individuals
All other loans (excluding consumer loans)
Obligations (other than securities and leases) of states and political subdivisions in the U.S.
Held-to-maturity securities
Available-for-sale securities, total
Premises and fixed assets including capitalized lease
Cash
Additionally:

Column 15: Contains the banks' debt.
Column 16: Contains a binary variable indicating default status (1 for default, 0 for no default).
Objective
The primary objective of this project is to predict the binary output variable, y, which denotes whether a bank will default. The challenge lies in the unbalanced nature of the dataset, where defaults are significantly less common than non-defaults.

## Methodology
To address the challenge of the unbalanced dataset, we employed several sampling and data generating techniques to balance it and thereby enhance the predictive models' performance. The analysis involved the use of multiple models:

Decision Trees
Random Forest
Autoencoders
Neural Network
Each model was chosen for its unique capabilities in handling datasets with varying degrees of complexity and feature interactions.

## Data Balancing Techniques
Sampling Methods: We used oversampling of the minority class and undersampling of the majority class to achieve a balanced dataset.
Data Generating Techniques: Synthetic data generation methods were implemented to create plausible default cases, augmenting the minority class.
Performance Metrics
To evaluate the models, we focused on the ability to predict bankruptcies correctly. This was measured using metrics suitable for unbalanced datasets, such as precision-recall (PR) curve, F1 score, and the area under the PR curve (AUPRC).

## Results
Among the models tested, the Autoencoders model exhibited the highest performance, particularly in predicting the number of bankruptcies correctly. This success is attributed to the Autoencoder's ability to learn a compressed representation of the data, focusing on the most salient features that contribute to the default risk.
