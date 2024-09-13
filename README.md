# Explainable Artificial Intelligence for Patient Safety A Review of Application in Pharmacovigilance
Welcome to the XAI patient safety project! This repository presents a comprehensive review of the application of Explainable AI (XAI) in the field of pharmacovigilance. While AI is increasingly being utilized in drug surveillance, patient safety, and predicting adverse drug reactions, the integration of XAI remains limited. From an initial pool of 781 studies, only 25 met the selection criteria for this research, focusing on the use of clinical, registry, and knowledge data to explore drug treatment, side effects, and drug interactions. Utilizing models such as tree models, neural networks, and graph models, this review identifies key challenges in employing XAI for pharmacovigilance, with an emphasis on the future potential and need for explainability in AI-driven medical research.
> ## Table of Contents
* [Overview](#Overview)
* [Technologies Used](#Technologies-Used)
* [How it Works](#How-it-Works)
* [Deployment](#Deployment)
* [Benefits](#Benefits)
* [Usage](#Usage)
* [Contact](#Contact)
### Overview
The system automates drug prediction, enabling healthcare professionals to make informed decisions based on key patient factors. It includes model performance comparisons, SHAP visualizations, and ensures both accuracy and interpretability, enhancing clinical decision-making in drug safety and treatment.
### Technologies Used
**1.Backend**

- **Python (Core Backend)** :Python acts as the backend programming environment, managing all the logic for data preprocessing, model building, training, and evaluation.
Machine Learning & Deep Learning Libraries
Keras (with TensorFlow backend): For building, training, and evaluating deep learning models like CNN and GraphCNN.
SHAP: For explainability, providing insights into the decision-making process of models.
File Handling
Pandas for loading CSV datasets (drug200.csv, testData.csv), and Pickle for saving/loading model history and weights.

**2.Frontend**

**Matplotlib & Seaborn Visualizations**
- **Graphs and Plots:** Various charts, confusion matrices, bar graphs, and SHAP visualizations serve as the "frontend" where users see the output and results from model training and evaluation.
- **SHAP Plots:** Force plots, summary plots, and violin plots generated by SHAP offer an interactive, explainable AI perspective for understanding model predictions.
### How it Works
**1.Data Preprocessing:**
-Load and preprocess the drug dataset, converting categorical data to numerical values and normalizing features for model training.

**2.Model Training:**
- Train different machine learning models such as XGBoost, Neural Networks, and Graph Convolutional Neural Networks (GraphCNN) using the processed dataset.
  
**3.Model Evaluation:**
- After training, the models are evaluated using performance metrics such as accuracy, precision, recall, and F1-score. Confusion matrices and other visualizations help understand the model's performance.
  
**4.Explainability with SHAP:**
- Use SHAP (SHapley Additive exPlanations) to explain the decision-making of the trained models, showing which features contributed most to the predictions with interactive plots.

**5.Drug Prediction:**
- The system can predict drug types based on patient information. Users can input test data, and the models will provide predictions for the most appropriate drug.
  
**6.Performance Comparison:**
- Compare the performance of different models (XGBoost, Neural Network, GraphCNN, CNN2D) using visual comparison charts to identify the most effective model for drug prediction.
### Deployment
**1.Environment Setup:**

- Install necessary Python libraries such as scikit-learn, xgboost, Keras, SHAP, and others used in the project.
Ensure that the machine learning models, datasets, and necessary code files are ready for deployment.

**2.Server Configuration:**

- Configure a Python-based server using Flask or Django to handle model inference and serve predictions via an API.
Alternatively, use FastAPI for more efficient, asynchronous handling of requests if required.
### Benefits

- **Efficiency:**
Automates the process of drug prediction and analysis, reducing manual effort in pharmacovigilance and clinical decision-making.
- **Explainability:**
Utilizes SHAP to provide transparent, explainable AI, allowing healthcare professionals to understand the reasoning behind model predictions.
- **Data Management:**
Centralizes patient and drug data, allowing for efficient storage, retrieval, and analysis of drug interactions and side effects.
- **Customization:**
The system can be easily customized to accommodate different types of data and models, allowing it to be tailored for specific healthcare needs.
- **Accuracy:**
Provides high accuracy in drug predictions through advanced algorithms such as XGBoost, Neural Networks, and GraphCNN, improving patient safety.
### Contact
If you have any questions or suggestions, feel free to contact us:

Email: yarukalaalekhya@gmail.com

Thank you for exploring our AI-based Drug Prediction System! We hope it enhances your understanding of pharmacovigilance and AI-driven healthcare solutions.
