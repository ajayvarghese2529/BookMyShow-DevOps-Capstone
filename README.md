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
✅ Phase 1 – Phase 10 Completed  
⏸️ Project paused for cost optimization  
🚀 Ready for evaluation and demo

---

## Author
Ajay Varghese

