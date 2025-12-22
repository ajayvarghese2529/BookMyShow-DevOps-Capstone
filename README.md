# BookMyShow DevOps Capstone Project

## Project Overview
This project demonstrates an end-to-end DevOps implementation for an online movie ticketing platform inspired by BookMyShow.  
The objective is to design, build, deploy, and monitor a scalable application using modern DevOps tools and AWS cloud services, with a strong focus on automation, reliability, and observability.


---

## Technology Stack
- AWS (EC2, IAM, EKS)
- Jenkins
- Docker
- Kubernetes
- SonarQube
- Trivy
- Prometheus
- Grafana
- Helm
- GitHub

---

## Key Highlights
- Designed and implemented a complete CI/CD pipeline using Jenkins
- Integrated static code analysis and security scanning into the pipeline
- Built production-ready Docker images using multi-stage builds
- Deployed and validated the application on AWS EKS
- Implemented real-time monitoring using Prometheus and Grafana
- Applied DevOps best practices for automation, observability, and scalability

---

## CI/CD Pipeline Summary
- A GitHub push automatically triggers the Jenkins pipeline
- Application dependencies are installed
- Static code analysis is performed using SonarQube
- Docker image is built and pushed to Docker Hub
- Application container is validated
- Container image is deployed to AWS EKS
- Application and infrastructure are monitored using Prometheus and Grafana

---

## Kubernetes Deployment
- Kubernetes Deployment configured with multiple replicas
- NodePort service used for external access
- Namespace isolation applied using `bms`
- Application accessibility verified via EKS worker node public IPs

---

## Monitoring & Observability
- Prometheus collects cluster-level, node-level, and pod-level metrics
- Grafana visualizes CPU, memory, and pod resource usage
- Dashboards filtered to focus on the `bms` namespace for clarity

---

## Challenges & Learnings

### Challenges Encountered
- Jenkins builds initially failed due to the application residing in a subdirectory
- Application UI did not load when containerized using a development runtime
- SonarQube scanner execution failed during early pipeline runs
- GitHub authentication failed due to deprecated password-based access
- Kubernetes services were inaccessible externally due to missing NodePort rules

### Resolutions Implemented
- Corrected Jenkins execution context using `dir()` for the application path
- Implemented multi-stage Docker builds and served the application via NGINX
- Configured and explicitly invoked SonarQube Scanner as a Jenkins tool
- Used GitHub Personal Access Token (PAT) for secure authentication
- Updated AWS security group rules to allow required NodePort access

### Key Learnings
- Importance of correct execution context in CI/CD pipelines
- Difference between development and production container strategies
- Secure credential handling in Jenkins and GitHub
- Kubernetes networking and service exposure concepts
- Practical cloud resource management and observability practices

---

## Project Status
✅ End-to-end CI/CD pipeline successfully implemented  
✅ Containerized application deployed and validated on AWS EKS  
✅ Observability enabled using Prometheus and Grafana  

This repository represents a complete, production-aligned DevOps implementation demonstrating CI/CD automation, container orchestration, and monitoring best practices.

---

## Author
Ajay Varghese
 
