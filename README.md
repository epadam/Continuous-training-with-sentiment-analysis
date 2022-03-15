# Continuous-training-with-sentiment-analysis

0. Data Collecting: Streamlit, SQL
1. Data labeling: label studio
2. Model and data tracking: mlflow, DVC
3. Develop Environmnet: Kubeflow
4. Retraining Pipeline: Kubeflow Pipeline
5. Deployment: Seldon Core (online and offline)
6. Monitoring: Promethius
7. Logging: ELK

## Infrastructure Setup

Please follow the instruction here. (credential setup)

## Model Development and Deployment Process

You can follow these steps to develop your models

1. EDA and develop the experiment with different models (mlflow, microsoft reponsible widget, LIT)
2. Build the components and pipeline (preprocessing, training, deploying, retraining) kubeflow pipeline, tfx, seldon core(A/B testing, canary deployment)
3. Write CI/CD (github actions, Jenkins)

## Retraining 

a. Annotate your data using Label Studio and store in the node
b. Detect concept drift

--> It would trigger the retraining process and deploy the seldon core again
