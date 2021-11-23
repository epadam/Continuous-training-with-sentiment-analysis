# Continuous-training-with-sentiment-analysis
entiment analysis with kubeflow, DVC, mlrun

## Infrastructure Setup

Please follow the instruction here. (credential setup)

## Model/code Development and Deployment

1. EDA and develop the experiment with different models (mlflow, microsoft reponsible widget, LIT)
2. Build the components and pipeline (preprocessing, training, deploying, retraining) kubeflow pipeline, tfx, seldon core(A/B testing, canary deployment)
3. Write CI/CD (github actions, Jenkins)

## Retraining 

a. Annotate your data using Label Studio and store in the node
b. Detect concept drift

--> It would trigger the retraining process and deploy the seldon core again
