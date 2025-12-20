# BookMyShow DevOps Capstone Project

## Project Overview
This project demonstrates an end-to-end DevOps implementation for an online movie ticketing platform (BookMyShow).
The objective is to design, build, deploy, and monitor a scalable application using modern DevOps tools and AWS cloud services.

---

## Architecture Flow
GitHub → Jenkins → Docker → AWS EKS → Prometheus → Grafana

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
- GitHub push triggers Jenkins pipeline
- Application dependencies installed
- Static code analysis using SonarQube
- Docker image built and pushed to Docker Hub
- Application validated on EC2
- Deployed to AWS EKS
- Monitored using Prometheus and Grafana

---

## Kubernetes Deployment
- Deployment with multiple replicas
- NodePort service exposure
- Namespace isolation (`bms`)
- Verified application accessibility via worker nodes

---

## Monitoring & Observability
- Prometheus collects cluster, node, and pod metrics
- Grafana visualizes CPU, memory, and pod usage
- Dashboards filtered to application namespace

---

## Project Status
✅ End-to-end CI/CD pipeline successfully implemented  
✅ Containerized application deployed and validated on AWS EKS  
✅ Observability enabled with Prometheus and Grafana  

This repository represents a complete, production-aligned DevOps implementation
demonstrating CI/CD automation, container orchestration, and monitoring best practices.
---

## Author
Ajay Varghese

