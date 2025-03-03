# Statistical Machine Learning: Cancer Classification & Handwritten Digit Recognition

## Project Summary

This project uses **Statistical Machine Learning (SML)** to tackle two different tasks

*   **Part 1: Cancer Classification:** We're trying to identify cancerous tissue samples using information from DNA microarrays (which measure gene activity).
*   **Part 2: Handwritten Digit Recognition:** We're building models that can recognize handwritten digits (0-9) from the MNIST dataset.

## Project Files

*   **`jeandedieu_ngirinshuti_SML2.pdf`:** This is the full project report with all the details, results, and conclusions.
*   **`jeandedieu_ngirinshuti_SML2.Rmd`:** This is the R Markdown script that contains the code used for data analysis and building the models.

## Part 1: Cancer Classification (Analyzing Gene Data)

*   **Data:** We used a dataset with 79 samples and 501 different gene measurements (DNA Gene Expressions).
*   **Key Steps**
    *   **Finding Important Genes:** We used the Kruskal-Wallis test to select the genes that best distinguish between cancer and non-cancer samples.
    *   **Simplifying the Data:** We used PCA (Principal Component Analysis) to reduce the number of variables and make the data easier to work with.
    *   **Building a Classification Model:** We used Decision Trees to classify the samples as either cancerous or non-cancerous.
    *   **Checking the Results:** We used ANOVA to make sure the genes we selected were truly important.

*   **What We Found**
    *   The top 9 genes were able to clearly separate cancer and non-cancer samples.
    *   Reducing the number of variables made the model easier to understand.
    *   Decision Trees were able to accurately classify cancer status with few errors.

## Part 2: Recognizing Handwritten Digits

*   **Data:** We used the MNIST dataset, which contains images of handwritten digits from 0 to 9.
*   **Models We Tested**
    *   **k-NN (with different settings):** We tried k-Nearest Neighbors with different numbers of neighbors (1NN, 5NN, 7NN, 9NN, 13NN).
    *   **Decision Trees (with different settings):** We built Decision Trees with different complexity levels.
*   **How We Measured Performance**
    *   **ROC Curves:** We used ROC curves to evaluate the performance of the classification models.
    *   **Error Rates:** We looked at the test error rates and analyzed the tradeoff between bias and variance.

*   **What We Found**
    *   **7NN and 9NN worked best:** k-NN with 7 or 9 neighbors provided the best balance between accuracy and being able to work with new data.
    *   **Decision Trees need to be pruned:** Decision Trees need to be simplified (cp = 0.05 or 0.1) to avoid being too specific to the training data.
    *   **Recognizing "1" and "7" is easy:** We were able to classify the digits "1" and "7" with very high accuracy.

## Watch the Video!

You can see a presentation of the project here

🔗 **[YouTube Video](https://youtu.be/5vDRaiMnfyw)**

## How to Run the Code

1.  **Install the Necessary Packages in R:**

    Open R or RStudio and run the following command:

    ```r
    install.packages(c("ggplot2", "dplyr", "MASS", "caret", "rpart"))
    ```
