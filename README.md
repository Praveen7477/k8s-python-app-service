# k8s-python-app-service

# Kubernetes Service Demo

This project demonstrates how to deploy a Python application in Kubernetes and expose it using a Service.

## Technologies
- Kubernetes
- Minikube
- Docker
- Python

## Steps

### Build Docker Image

docker build -t praveen/python-sample-app-demo:v1 .

### Deploy Application

kubectl apply -f deployment.yml

### Create Service

kubectl apply -f service.yml

### Access Application

minikube service python-django-app-service --url

## Output

The application page shows:

"Kubernetes Service - Created by Praveen"
