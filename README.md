# AutoML Comparison: H2O and Vertex AI Pipelines

## Overview

This project evaluates the capabilities of two AutoML platforms — **H2O AutoML** and **Vertex AI Pipelines** — using the athletes dataset. It compares model performance, feature importance, and execution speed while documenting the process and results for each platform.

---

## Objectives

1. Perform AutoML analysis using H2O and Vertex AI Pipelines.
2. Identify the top 5 features impacting model performance.
3. Compare the top 3 models for:
   - Validation score using all features and top features.
   - Execution speed using all features and top features.
4. Analyze how the best models compare to previously developed models.
5. Discuss the nature of each platform: no-code, low-code, or full-code.

---

## Dataset Details

### Source:  
`athletes.csv`

### Features:
- **Categorical Variables:** Athlete metadata such as gender, nationality, and sport.  
- **Numerical Variables:** Performance metrics like height, weight, and age.

---

## Methodology

### H2O AutoML
1. **Setup**:
   - Initialized H2O instance and uploaded dataset.
   - Ran AutoML for 30 minutes to train multiple models.
2. **Feature Insights**:
   - Identified top features: `weight`, `pullups`, `height`, `age`, `athlete ID`.
3. **Model Comparison**:
   - Validation score and execution speed for all features and top features.

### Vertex AI Pipelines
1. **Setup**:
   - Uploaded dataset to Vertex AI and configured AutoML pipeline.
   - Trained models using Vertex AI's no-code interface.
2. **Feature Insights**:
   - Identified top features: `weight`, `pullups`, `height`, `age`, `athlete ID`.
3. **Model Comparison**:
   - Validation score and execution speed for all features and top features.

---

## Results

### Top Features
- **H2O AutoML** and **Vertex AI** both identified the same top features:
  1. Weight  
  2. Pullups  
  3. Height  
  4. Age  
  5. Athlete ID  

### Top Models by Validation Score
- **All Features**:
  - H2O: RMSE = 123.42, R² = 0.80  
  - Vertex AI: RMSE = 121.86, R² = 0.787  
- **Top Features**:
  - H2O: Model 1, Model 2, Model 3  
  - Vertex AI: Model A, Model B, Model C  

### Top Models by Execution Speed
- **All Features**:
  - H2O: ~30 minutes  
  - Vertex AI: ~60 minutes  
- **Top Features**:
  - H2O: Significantly faster across all configurations.  
  - Vertex AI: Slightly slower but maintained performance.

---

## Platform Comparison

- **Validation Score**:  
  Vertex AI slightly outperformed H2O in RMSE, but H2O achieved a marginally better R² score.

- **Execution Speed**:  
  H2O executed significantly faster, especially with smaller feature subsets.

- **Nature of Platforms**:  
  - **H2O AutoML**: Full-code, offering extensive flexibility and control.  
  - **Vertex AI Pipelines**: No-code, ideal for quick setups with intuitive pipelines.

---

## How to Use This Repository
1. Clone the repository:
   ```bash
   git clone https://github.com/ArushiMakraria/cathletes-automl-comparison
   ```
2. Access the analysis scripts and dataset.
3. Follow the provided notebooks for step-by-step implementation and insights.

For questions or feedback, feel free to reach out!
