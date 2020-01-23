[![CircleCI](https://circleci.com/gh/Myraa/OperationalizeMachineLearningAPI.svg?style=svg)](https://circleci.com/gh/Myraa/OperationalizeMachineLearningAPI)

## Project Overview

>In this project, I applied the skills which I have acquired in this course to operationalize a Machine Learning Microservice API. This project tests my ability to operationalize a Python Flask App in a provided file, app.py that serves out predictions (inference) about housing prices through API calls.

![img-1](/housingpriceimage.JPG)


>You are given a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project tests your ability to operationalize a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

### Project Tasks

This project goal is to operationalize this working, machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. In this project you will:
* Test your project code using linting
* Complete a Dockerfile to containerize this application
* Deploy your containerized application using Docker and make a prediction
* Improve the log statements in the source code for this application
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and make a prediction
* Upload a complete Github repo with CircleCI to indicate that your code has been tested

## The files included are:
```sh.
* /.circleci : CircleCI configuration file for running the tests
* /model_data : Housing model data
* /output_txt_files : Log of Output 
* Dockerfile : Dockerfile for building the image 
* Makefile : includes instructions on environment setup and lint tests
* app.py : Python flask app that serves out predictions (inference) about housing prices through API calls
* make_prediction.sh : Send a request to the Python flask app to get a prediction, for localhost 
* requirements.txt : Install any dependencies 
* run_docker.sh : file to be able to get Docker running, locally
* run_kubernetes.sh : file to run the app in kubernetes
* upload_docker.sh : file to upload the image to docker
```
## Setup the Environment

* Create a virtualenv and activate it
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl

## CircleCI Integration

This repository has been verified with CircleCI

