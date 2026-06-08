# From Real to Synthetic: Socio-Spatial Population Modeling Using CTGAN for AI and Policy Applications
## Overview

This repository presents a synthetic population generation framework using Conditional Tabular Generative Adversarial Networks (CTGAN) to model socio-spatial demographic structures while preserving privacy.

The model generates realistic synthetic datasets that replicate the statistical properties, dependencies, and spatial patterns of real population data across demographic, socioeconomic, household, and provincial attributes. The resulting synthetic population supports downstream applications in AI modeling, spatial analysis, and policy evaluation without exposing sensitive individual-level data.

## Research Motivation

High-quality population data is essential for:

Urban and regional planning
Socioeconomic modeling
Policy simulation
Machine learning applications
Mobility and spatial analysis

However, real-world microdata often comes with:

Privacy restrictions
Limited accessibility
Ethical and legal constraints
Data sparsity in sensitive attributes

This study addresses these limitations by generating privacy-preserving synthetic populations that maintain realistic statistical behavior.

## Research Objectives

The main objectives of this project are to:

Generate realistic synthetic population data using CTGAN.
Preserve marginal distributions and inter-variable relationships.
Maintain socio-spatial structure across administrative regions.
Evaluate synthetic data fidelity using statistical distance metrics.
Enable privacy-preserving data sharing for AI and policy use cases.

## Methodology
### 🤖 Conditional Tabular GAN (CTGAN)

CTGAN is a generative deep learning model designed for tabular data with mixed variable types.

It learns:

Conditional distributions of categorical variables
Complex nonlinear dependencies
Multivariate relationships across features
Input Data Structure

The model is trained on eight categorical variables, representing:

#### 👨‍👩‍👧 Demographic Attributes
Age group
Gender
Household composition

#### 💼 Socioeconomic Attributes
Income class
Employment status
Education level

#### 🏠 Household Characteristics
Household type
Housing classification

#### 🗺 Spatial / Provincial Attribute
Province-level location

## Evaluation Metrics

The quality of synthetic data was assessed using multiple statistical measures:

### 📊 Distribution Similarity
Total Variation Distance (TVD)
Jensen-Shannon Divergence (JSD)

### 🔗 Dependency Preservation
Cramér’s V (categorical association strength)

### 📈 Category-Level Comparison
Marginal distribution alignment
Frequency-based validation

## Key Results
🏆 High-Fidelity Synthetic Data Generation

The CTGAN model successfully reproduced:

Realistic marginal distributions
Strong inter-variable dependencies
Spatial demographic structure
Provincial-level population patterns

📉 Minor Deviations Observed In:

High-cardinality categorical variables
Complex joint distributions
Rare population subgroups

Despite these limitations, overall fidelity remained high.

## Key Findings
✔ Strong Statistical Fidelity

Synthetic data closely matches real population distributions across all evaluated metrics, including TVD and JSD.

✔ Dependency Preservation

Cramér’s V analysis confirms that CTGAN preserves:

Socioeconomic relationships
Household structure dependencies
Demographic interactions
✔ Spatial Consistency

Province-level distributions are maintained, ensuring:

Regional representativeness
Spatial realism for policy simulations
Usability in geographic modeling tasks
✔ Privacy Preservation

The generated dataset:

Does not replicate individual records
Preserves statistical realism without exposure risk
Enables safe data sharing for research and policy use

## Applications
### 🧠 Artificial Intelligence
Training machine learning models
Data augmentation
Bias reduction in datasets

### 🏙 Urban & Regional Planning
Synthetic population modeling
Scenario simulation
Infrastructure planning

### 📊 Policy Analysis
Policy impact simulation
Socioeconomic forecasting
Decision-support systems

### 🔒 Privacy-Preserving Data Sharing
Secure data release
Open-data alternatives
Ethical research data generation

## Key Contributions
Development of a CTGAN-based synthetic population generator for socio-spatial data.
Preservation of demographic, socioeconomic, and spatial dependencies.
Comprehensive evaluation using TVD, JSD, and Cramér’s V metrics.
Demonstration of privacy-preserving synthetic data generation.
Support for AI-driven policy modeling and spatial simulations.
Scalable framework for generating realistic tabular populations.

## Limitations
Reduced accuracy in high-cardinality categorical variables.
Slight divergence in rare population segments.
Sensitivity to training data representativeness.
