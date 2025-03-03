# Statistical Machine Learning: Cancer Classification & MNIST Digit Recognition

## Overview
This project applies **Statistical Machine Learning (SML)** techniques to two different tasks  
- **Part 1:** Cancer classification using **high-dimensional gene expression data (DNA Microarray)** 
- **Part 2:** Multi-class and binary classification of **handwritten digits (MNIST dataset)**

## Files
- `jeandedieu_ngirinshuti_SML2.pdf` → Full project report 
- `jeandedieu_ngirinshuti_SML2.Rmd` → R Markdown script for data analysis and modeling

## 🧬 Part 1: Cancer Classification (High-Dimensional Data)
- Dataset: **79 samples, 501 features (DNA Gene Expressions)**  
- **Key Techniques Used**
  - **Feature Selection** using Kruskal-Wallis test  
  - **Dimensionality Reduction** via PCA  
  - **Decision Trees** for classification  
  - **ANOVA Test** to validate feature importance  

- **Findings:**
  - Top 9 genes significantly differentiate cancer vs. non-cancer cases
  - Dimensionality reduction improves model interpretability
  - Decision Trees effectively classify cancer status with low misclassification error
  - 
## Part 2: MNIST Handwritten Digit Recognition
- **Dataset:** MNIST (handwritten digits 0-9)
- **Models Evaluated**  
  - **k-NN (1NN, 5NN, 7NN, 9NN, 13NN)**  
  - **Decision Trees (various complexity parameters)**  
- **Performance Analysis**  
  - ROC Curves for classification performance  
  - Test error rates and bias-variance tradeoff analysis  

- **Findings**
  - **7NN and 9NN achieved the best balance of accuracy and generalization**
  - **Decision Trees require pruning (cp = 0.05 or 0.1) to avoid overfitting**
  - **Binary classification of digits "1" and "7" achieved high accuracy**

## 🎥 Video Presentation
Watch the full project presentation here  
🔗 **[YouTube Video](https://youtu.be/5vDRaiMnfyw)**  

## 🛠 How to Run the Code
1. Install required packages in R
   ```r
   install.packages(c("ggplot2", "dplyr", "MASS", "caret", "rpart"))
