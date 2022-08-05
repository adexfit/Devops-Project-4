## Project 4: Operationalizing a Machine Learning Microservice API

[![adexfit](https://circleci.com/gh/adexfit/Devops-Project-4.svg?style=svg)](https://app.circleci.com/pipelines/github/adexfit/Devops-Project-4)

## Project Overview
In this project, I operationalize a Python flask app that serves out predictions about housing prices through API calls.

### Running instructions

+ To run the *docker* script, use the `run_docker.sh` script (`./run_docker.sh`).
+ To run the *kubernetes* script, first start your *minikube* cluster (`minikube start`) then execute the `run_kubernetes.sh` script (`./run_kubernetes.sh`). Please note that you may need to re-run the script because the port forwarding command requires the pod to be up.
+ To make a prediction about housing prices, execute the `make_predictions.sh` script (`./make_predictions.sh`).


### Files 

+ The *python* dependencies have been listed in the `requirements.txt` file.
+ The `app.py` file contains the *python* API logic.
+ The serialized machine learning model is stored under `model_data/boston_housing_prediction.joblib`.
+ The `Dockerfile` consists of instructions to build the Docker image.
+ You can find the development commands in the `Makefile`.
+ Examples of the outputs are available in the `output_txt_files` directory.
+ Other *shell* scripts contain helper commands for deployment.
