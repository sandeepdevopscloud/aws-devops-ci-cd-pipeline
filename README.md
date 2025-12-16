# AWS DevOps CI/CD Pipeline Project

## About the Project
This project shows how a simple CI/CD pipeline works using AWS and DevOps tools.
I built this project to understand how code is automatically built, containerized, and deployed to Kubernetes.

## Tools Used
- Git and GitHub
- Jenkins
- Maven
- Docker
- Kubernetes (AWS EKS)
- Ansible
- AWS services (EC2, IAM, VPC, EKS)

## How the CI/CD Pipeline Works
1. Code is pushed to the GitHub repository.
2. Jenkins is triggered automatically using a webhook.
3. Jenkins builds the application using Maven.
4. A Docker image is created from the application.
5. Ansible is used to automate deployment steps.
6. The application is deployed to a Kubernetes cluster on AWS (EKS).
7. Kubernetes manages the running containers.

## CI/CD Flow Explanation (Project Diagram)
In this project, the developer first commits the application code to GitHub.

Jenkins pulls the code from GitHub and starts the pipeline automatically using a webhook.
Jenkins builds the Java application using Maven and generates the build artifact.

After the build is successful, Jenkins uses a Dockerfile to create a Docker image.
The Docker image is then pushed to Docker Hub.

Ansible is used to automate the deployment process.
Kubernetes pulls the Docker image from Docker Hub and deploys the application as a container.

Kubernetes manages the running container and ensures the application is running properly.

## What I Learned
- How to create a CI/CD pipeline using Jenkins
- How Docker is used to containerize applications
- How to deploy applications on Kubernetes (EKS)
- Basics of using Ansible for automation
- Practical understanding of AWS cloud services
