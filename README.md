# Continuous-training-with-sentiment-analysis

0. Data Collecting & ETL: Streamlit(Product review), SQL, Airflow
1. Data labeling: label studio
2. Model and data tracking: mlflow, DVC
3. Develop Environmnet: Kubeflow
4. Retraining Pipeline: Kubeflow Pipeline
5. Deployment: Seldon Core (online and offline)
6. Monitoring: Promethius (explainer, drift, outlier detector)
7. Logging: ELK
8. Test UI for Online Inference: Streamlit(auto reply for review commands)

Collected data will be periodically process data, train the model then deploy the model.
When detect the concept drift, it would trigger the retraining pipeline

## Infrastructure Setup

Please follow the instruction here. (credential setup)

## Model Development and Deployment Process

You can follow these steps to develop your models

1. EDA and develop the experiment with different models (mlflow, microsoft reponsible widget, LIT)
2. Build the components and pipeline (preprocessing, training, deploying, retraining) kubeflow pipeline, tfx, seldon core(A/B testing, canary deployment)
3. Write CI/CD (github actions, Jenkins)

