# Operationalize-a-Machine-Learning-Microservice-API
In this project, the application the skills acquired in this course to operationalize a Machine Learning Microservice API at Udacity. 

[![CircleCI](https://circleci.com/gh/NomanAbdullah/Operationalize-a-Machine-Learning-Microservice-API.svg?style=svg)](https://circleci.com/gh/NomanAbdullah/Operationalize-a-Machine-Learning-Microservice-API)

## Project Overview

A pre-trained, **sklearn** model is given that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project tests your ability to operationalize a Python flask app—in a provided file, **app.py**—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

### Project Tasks

The project goal is to operationalize this working, machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. In this project you will:
* Test the project code using linting
* Complete a Dockerfile to containerize this application
* Deploy your containerized application using Docker and make a prediction
* Improve the log statements in the source code for this application
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and make a prediction
* Upload a complete Github repo with CircleCI to indicate that the code has been tested

---

## Setting up the Environment

* Create a **Makefile**
* Create a **Dockerfile**
* Run **make setup** to create a virtual environment and activate it
* Run **make install** to install the necessary dependencies

## Linting App
* Run **make lint** 

## Testing App
* Run **make test**

### Running `app.py`

1. Standalone:  **python app.py**
2. Run in Docker:  **./run_docker.sh**
3. Run in Kubernetes:  **./run_kubernetes.sh**

### Uploading to Docker Hub
* Run **upload_docker.sh**

### Kubernetes Steps
* Use **minikube** to configue kubernetes locally.
* Run **run_kubernetes.sh** to deploy and save output logs
* Run **minikube delete** to delete kubernetes cluster