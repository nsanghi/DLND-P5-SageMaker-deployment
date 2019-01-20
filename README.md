# Machine Learning Deployment using AWS SageMaker

## Implementation of an RNN based Sentiment Analysis model using SageMaker. 

### This project involves following steps:

1. Developing a model using RNN on IMBD reviews data set
2. Training the model using SageMaker
3. Deploying the model as an end point in SageMaker
4. Use of Lambda function to provide an api to the deployed model
5. Gateway API to expose the Lambda function (and underlying RNN model) as a public end point api

The original repository with code and associated files for deploying ML models using AWS SageMaker can be found [here](https://github.com/udacity/sagemaker-deployment)


This repository contains implementation of starter code at [Sentiment Analysis Web App](https://github.com/udacity/sagemaker-deployment/tree/master/Project). The result is a deployed RNN performing sentiment analysis on movie reviews complete with publicly accessible API and a simple web page which interacts with the deployed endpoint. This project assumes that you have some familiarity with SageMaker. Completing the XGBoost Sentiment Analysis notebook from [this](https://github.com/udacity/sagemaker-deployment) repository should suffice.


## Setup Instructions

The notebooks provided in this repository are intended to be executed using Amazon's SageMaker platform. The following is a brief set of instructions on setting up a managed notebook instance using SageMaker, from which the notebooks can be completed and run.

### Log in to the AWS console and create a notebook instance

Log in to the AWS console and go to the SageMaker dashboard. Click on 'Create notebook instance'. The notebook name can be anything and using ml.t2.medium is a good idea as it is covered under the free tier. For the role, creating a new role works fine. Using the default options is also okay. Important to note that you need the notebook instance to have access to S3 resources, which it does by default. In particular, any S3 bucket or object with sagemaker in the name is available to the notebook.

A more detailed instructions can be found in `README.md` at [udacity repository](https://github.com/udacity/sagemaker-deployment)
