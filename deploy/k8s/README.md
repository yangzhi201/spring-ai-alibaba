# Kubernetes Deployment Guide

This directory contains the Kubernetes configuration files for deploying the `chatbot` example application.

## Prerequisites

- Kubernetes cluster (e.g., Minikube, Docker Desktop K8s, or a cloud provider)
- `kubectl` installed and configured
- Docker installed

## Build the Docker Image

Navigate to the `examples/chatbot` directory and build the application and Docker image:

```bash
cd ../../examples/chatbot
mvn clean package
docker build -t spring-ai-alibaba-chatbot:latest .
```

## Deploy to Kubernetes

Apply the configuration files:

```bash
kubectl apply -f chatbot-deployment.yaml
kubectl apply -f chatbot-service.yaml
```

## Verify Deployment

Check the status of the pods and service:

```bash
kubectl get pods
kubectl get svc
```

## Access the Application

If you are using `ClusterIP` (default), you can port-forward to access it locally:

```bash
kubectl port-forward svc/chatbot-service 8080:80
```

Then access it at `http://localhost:8080`.
