# Team Sigma: Accident Fatality Predictor (Toronto Police)

# Live Application
Experience our model in action at the live application: [Accident Fatality Predictor](https://accident-fatality-predictor.streamlit.app/).

## Overview
This project is an accident fatality predictor, which can predict if the Accident is going to be fatal or not based on many factors of the accident such as The location, the type of road, if the person was a pedestrian or a driver or cyclist etc etc. This is made for city of toronto as the dataset is based on the Toronto city Data.

## Data Description
- **Source:** Toronto Police Service
- **Features:** The dataset includes both numerical and categorical data, representing various aspects of each collision, such as road conditions, vehicle type, and weather conditions.
- **Challenges:** The primary challenges with the dataset included a significant class imbalance and handling numerous object-type features with substantial null values.

## Features and Preprocessing
- **Feature Engineering:** New features were generated to better capture the complexities of the data. Techniques like one-hot encoding were applied to transform categorical data into a machine-readable format.
- **Handling Missing Data:** Various imputation methods were used depending on the nature of the data in each column.

## Model Development
- **Model Evaluation:** Several models were tested, including Logistic Regression, Decision Trees, Random Forest, and Neural Networks.
- **Selection Criteria:** The Random Forest model was chosen for its robustness in handling imbalanced data and its ability to model complex interactions between features.

## Technology Stack
- **Frontend:** Streamlit for dynamic and interactive data visualization.
- **Machine Learning:** Python, Pandas for data manipulation, Scikit-Learn for model building for more complex model architectures.
- **Containerization:** Docker to ensure consistent environments across different stages of development and deployment.

## Installation and Running
Ensure Docker is installed on your machine for a smoother setup and execution process.

### Clone the Repository
```bash
git clone https://github.com/ItsJainam28/Accident_Fatality_Predictor.git
cd Accident_Fatality_Predictor

docker build -t accident_fatality_predictor .

docker run -p 8501:8501 accident_fatality_predictor

```

### Acknowledgements
Thanks to Prof. Ashish Gupta for his continuous support and guidance.
Gratitude towards the Toronto Police for providing the dataset essential for this analysis.
