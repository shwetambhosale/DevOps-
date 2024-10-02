# Customer Churn Prediction using Artificial Neural Network (ANN)

## Overview
This project aims to predict customer churn using an Artificial Neural Network (ANN). Customer churn refers to when customers stop using a company's product or service. Accurately predicting which customers are likely to churn allows companies to implement strategies to retain them.

The project utilizes a dataset containing customer features and labels, where the label indicates whether a customer has churned or not. The ANN model is built to predict this label using key features. This project is deployed using **Streamlit**, providing an interactive web interface where users can input customer data and view predictions.

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [License](#license)

## Dataset
The dataset used contains customer details such as:
- **Customer ID**
- **Gender**
- **Age**
- **Geography**
- **Credit Score**
- **Balance**
- **Tenure**
- **Number of Products**
- **Has Credit Card**
- **Is Active Member**
- **Estimated Salary**
- **Exited (Label)**: 1 if the customer churned, 0 otherwise.

The dataset is preprocessed to handle missing values, scale numerical features, and encode categorical variables.

## Model Architecture
The ANN architecture consists of:
- **Input Layer**: The number of neurons corresponds to the number of features in the dataset.
- **Hidden Layers**: Multiple hidden layers with a specified number of neurons and activation functions such as ReLU.
- **Output Layer**: A single neuron with a sigmoid activation function to output the probability of churn.

The model is trained using **binary cross-entropy** loss and optimized with the **Adam optimizer**.

## Requirements
To run this project, you need the following dependencies:
- Python 3.x
- TensorFlow/Keras
- NumPy
- Pandas
- Scikit-learn
- Matplotlib (optional, for visualization)
- Streamlit (for deployment)

Install the dependencies using:
```bash
pip install tensorflow numpy pandas scikit-learn matplotlib streamlit
```

## Installation
To set up the project locally, follow these steps:
1. **Clone the repository**:
2. **Install the required packages**:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
To run the Streamlit application, execute the following command in your terminal:
```bash
streamlit run app.py
```

## Results
The application displays predictions based on user input and provides visualizations that help analyze the factors contributing to customer churn.

## License
This project is licensed under the Apache 2.0 License. See the LICENSE file for more details.
