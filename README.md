[![CircleCI](https://circleci.com/gh/sageexplorer/Machine-Learning-Microservice-API.svg?style=svg)](https://circleci.com/gh/sageexplorer/Machine-Learning-Microservice-API)


## Setup the Environment

* Create a virtualenv and activate it
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`..Flask app will be available in port 80
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Kubernetes Steps

* run minikube create, and minikube start to create, and run the kubernetes pod
* Verify pod is running by typing `kubectl get pods`
* run ./run_kubernetes to create a deployment
* Flask app will be exposed to port 8888
* run ./make predictions to call Flask api 
