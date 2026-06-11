# Fitness Tracker – DevOps Capstone Project

## Project Overview

This project demonstrates the implementation of a complete DevOps workflow for deploying and managing the Fitness Tracker application. The objective of this project is to automate build, test, deployment, and infrastructure management using DevOps tools and practices.

## Objectives

* Implement CI/CD pipeline for automated deployment
* Containerize application using Docker
* Orchestrate deployment using Kubernetes
* Automate infrastructure and deployment workflows
* Monitor and manage application availability

## Tech Stack

* Source Code Management: Git, GitHub
* CI/CD: Jenkins
* Containerization: Docker
* Container Registry: Docker Hub
* Orchestration: Kubernetes
* Deployment: ArgoCD
* Infrastructure: Terraform
* Cloud Platform: AWS EC2
* Monitoring: Prometheus, Grafana

## Project Architecture

Developer → GitHub → Jenkins → Docker → Docker Hub → Kubernetes → ArgoCD → Deployment

## Features

* Automated build and deployment pipeline
* Containerized application deployment
* Continuous Integration and Continuous Delivery
* Infrastructure as Code
* Monitoring and visualization
* Scalable deployment architecture

## Installation & Setup

### Clone Repository

```bash
git clone <repository-url>
cd Fitness_Tracker
```

### Build Docker Image

```bash
docker build -t fitness-tracker .
```

### Run Docker Container

```bash
docker run -d -p 3000:3000 fitness-tracker
```

### Push Image to Docker Hub

```bash
docker tag fitness-tracker <dockerhub-username>/fitness-tracker
docker push <dockerhub-username>/fitness-tracker
```

### Kubernetes Deployment

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```

### Verify Deployment

```bash
kubectl get pods
kubectl get svc
```

## CI/CD Workflow

1. Developer pushes code to GitHub
2. Jenkins triggers pipeline automatically
3. Docker image is built and pushed
4. ArgoCD syncs changes to Kubernetes
5. Application gets deployed automatically

## Monitoring

* Prometheus for metrics collection
* Grafana for dashboards and visualization

## Project Outcome

Successfully implemented a complete DevOps lifecycle with automated deployment, scalability, monitoring, and reduced manual effort.

## Future Enhancements

* Auto scaling using HPA
* Blue-Green deployment
* Security scanning integration
* Automated testing


