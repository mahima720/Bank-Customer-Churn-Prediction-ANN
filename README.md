# 🏦 Bank Customer Churn Prediction (ANN)

This project features a Deep Learning application that predicts the likelihood of a bank customer leaving (churning) based on their demographic and financial profile. It uses an Artificial Neural Network (ANN) built with TensorFlow/Keras and an interactive web interface powered by Streamlit.

# 🔗 Live Demo
[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://bank-customer-churn-prediction-ann.streamlit.app/)

![UI](/images/image1.png)
![UI](/images/image2.png)

## ✨ Features

* **🧠 Deep Learning Engine:** Utilizes a multi-layer Artificial Neural Network (ANN) trained on historical bank customer data.

* **⚡ Real-time Probability:** Calculates the exact probability of churn, allowing for nuanced decision-making.

* **🛠️ Advanced Preprocessing:**

     * **Label Encoding:** For binary categorical data like Gender.

     * **One-Hot Encoding:** For multi-class categorical data like Geography.

     * **Feature Scaling:** Uses StandardScaler to optimize neural network convergence.

* **📱 Interactive Dashboard:** A clean Streamlit UI for entering customer details and viewing immediate predictions.

## Skills Developed

- **Deep Learning Workflow:** Designing, training, and saving a Keras model for binary classification.

- **Pipeline Preservation:** Managing multiple transformation objects (encoders and scalers) to ensure data consistency between training and production.

- **Probability Analysis:** Interpreting sigmoid output values as actionable risk percentages.

- **Frontend Design:** Mapping complex data structures to user-friendly UI components.

## How it Works
1) User Input: Data is collected through Streamlit's sliders and dropdowns.

2) Transformation:
    - Categorical variables are transformed using the saved Label and One-Hot encoders.
    - The complete feature set is then normalized using the StandardScaler.
    
3) Inference: The processed vector is fed into the .h5 ANN model.

4) Thresholding: If the output probability is $> 0.5$, the customer is flagged as "Likely to Churn."

## 🏁 Conclusion

The Customer Churn Prediction app demonstrates how Deep Learning can be translated into a practical business tool. By automating the analysis of customer behavior, banks can move from reactive to proactive strategies, ultimately improving customer retention and long-term profitability.