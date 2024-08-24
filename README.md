# Breast Cancer Detection Application
## What is Breast Cancer?
Cancer occurs when changes called mutations take place in genes that regulate cell growth. The mutations let the cells divide and multiply in an uncontrolled, chaotic way. The cells keep on proliferating, producing copies that get progressively more abnormal. In most cases, the cell copies eventually end up forming a tumor.

Breast cancer occurs when a malignant (cancerous) tumor originates in the breast. As breast cancer tumors mature, they may metastasize (spread) to other parts of the body. The primary route of metastasis is the lymphatic system which, ironically enough, is also the body's primary system for producing and transporting white blood cells and other cancer-fighting immune system cells throughout the body. Metastasized cancer cells that aren't destroyed by the lymphatic system's white blood cells move through the lymphatic vessels and settle in remote body locations, forming new tumors and perpetuating the disease process.

Breast cancer is not just a woman's disease. It is quite possible for men to get breast cancer, although it occurs less frequently in men than in women. Our discussion will focus primarily on breast cancer as it relates to women but it should be noted that much of the information is also applicable for men.

## Overview

This Breast Cancer Detection application uses a machine learning model to predict the presence of breast cancer based on various features of cell nuclei. The model has been trained using a dataset of cell characteristics and provides predictions of whether a patient has breast cancer or not.



## Features

- **Predict Breast Cancer**: Input cell details to receive a prediction on whether the patient has breast cancer.
- **Interactive Interface**: User-friendly form for entering cell characteristics and viewing predictions.
- **Information About the Model**: Provides detailed information about the model, features, and dataset.

## Technologies Used

- **Flask**: A lightweight WSGI web application framework in Python.
- **Bootstrap**: A front-end framework for developing responsive and mobile-first websites.
- **Python**: The programming language used to implement the Flask application and machine learning model.

## Model Selection and evaluation
Baseline algorithm checking
Analyse and build a model to predict if a given set of symptoms lead to breast cancer. This is a binary classification problem, and a few algorithms are appropriate for use.
As we do not know which one will perform the best at the point, we will do a quick test on the few appropriate algorithms with default setting to get an early indication of how each of them perform.

We will use 10 fold cross validation for each testing.

The following non-linear algorithms will be used, namely:

- Classification and Regression Trees (CART)
- Linear Support Vector Machines (SVM)
- Gaussian Naive Bayes (NB)
- k-Nearest Neighbors (KNN).
- ANN

## Hyperparameter Tuning and Cross Validation
<img width="476" alt="image" src="https://github.com/user-attachments/assets/4f8ae556-4bc5-44c7-baf5-d3899d443891">

## Based on the results:

Decision Tree (CART): With a mean accuracy of approximately 95.90%, using a max depth of 10 yielded the best performance for the CART model.

Support Vector Machine (SVM): Using a radial basis function kernel with C=1 resulted in the highest mean accuracy of approximately 97.13% for the SVM model.

Gaussian Naive Bayes (NB): The Gaussian Naive Bayes model achieved a mean accuracy of approximately 96.32% without any specific hyperparameters tuned, suggesting that the default configuration performed well.

k-Nearest Neighbors (KNN): Utilizing a Manhattan distance metric with 3 neighbors produced the highest mean accuracy of approximately 97.55% for the KNN model.

Overall, all models performed well, with SVM and KNN slightly outperforming CART and NB in terms of mean accuracy. The choice of the best model may depend on various factors such as interpretability, computational efficiency, and specific requirements of the application.

## Feature Importance

<img width="443" alt="image" src="https://github.com/user-attachments/assets/22571c47-685d-44de-a257-bb5a07ee3738">

## Installation

### Prerequisites

Ensure you have Python 3.12 installed. You will also need to have `pip` for installing Python packages.

### Setup

1. **Clone the Repository**

   ```bash
   git clone https://github.com/Sumbati10/PREDICTION_BREASTCANCER.git
   cd BREAST_CANCER

## Running the Application
Start the Flask Development Server
In your terminal, run:

python app.py

## Contributing
If you would like to contribute to this project, please fork the repository and create a pull request with your changes. For any issues or feature requests, please create an issue in the repository.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

## Contact
For any questions or feedback, please contact:

Lindah Sumbati: sumbatilinda@gmail.com   
