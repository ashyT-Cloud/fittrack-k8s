# 🚀 FitTrack - Kubernetes Deployment on Amazon EKS

![AWS](https://img.shields.io/badge/AWS-EKS-orange)
![Kubernetes](https://img.shields.io/badge/Kubernetes-v1.33-blue)
![Docker](https://img.shields.io/badge/Docker-Containers-blue)
![GitHub Actions](https://img.shields.io/badge/GitHub-Actions-success)
![License](https://img.shields.io/badge/License-MIT-green)

## 📌 Project Overview

FitTrack is a cloud-native three-tier application deployed on **Amazon Elastic Kubernetes Service (EKS)**.

The project demonstrates how to deploy a containerized application using Kubernetes best practices, including persistent storage, ConfigMaps, Secrets, LoadBalancer Services, and an automated Continuous Deployment (CD) pipeline using GitHub Actions.

---

## 🏗️ Architecture

```
                    Internet
                        │
                        ▼
            AWS Load Balancer Service
                        │
                        ▼
                Amazon EKS Cluster
        ┌──────────────┼──────────────┐
        ▼              ▼              ▼
   Frontend Pod   Backend Pod   MongoDB Pod
                                         │
                                         ▼
                                  Amazon EBS Volume
```

---

## ⚙️ Technologies Used

- Amazon Web Services (AWS)
- Amazon EKS
- Kubernetes
- Docker
- GitHub Actions
- Amazon EBS CSI Driver
- ConfigMaps
- Secrets
- Persistent Volumes
- LoadBalancer Services
- Git
- GitHub

---

## 📂 Project Structure

```text
fittrack-k8s
│
├── .github/
│   └── workflows/
│       └── deploy.yml
│
├── manifests/
│   ├── namespace/
│   ├── config/
│   ├── storage/
│   ├── database/
│   ├── backend/
│   └── frontend/
│
├── diagrams/
├── docs/
├── scripts/
│
├── LICENSE
└── README.md
```

---

## 🚀 Features

- Kubernetes Deployments
- Kubernetes Services
- Amazon EKS
- ConfigMaps
- Secrets
- Persistent Storage using Amazon EBS
- Dynamic Volume Provisioning
- GitHub Actions CD Pipeline
- AWS LoadBalancer Integration
- Namespace Isolation

---

## 🔄 Deployment Workflow

```
Developer
    │
 git push
    │
    ▼
GitHub Actions
    │
Configure AWS Credentials
    │
Update kubeconfig
    │
kubectl apply
    │
Amazon EKS Cluster
```

---

## 📦 Kubernetes Resources

- Namespace
- Deployments
- Services
- ConfigMaps
- Secrets
- StorageClass
- PersistentVolumeClaim
- PersistentVolume

---

## 📸 Screenshots

> Screenshots will be added.

- Amazon EKS Cluster
- Running Pods
- LoadBalancer Service
- Persistent Volume
- GitHub Actions Workflow
- Application Running

---

## 📚 Learning Outcomes

Through this project I learned:

- Kubernetes architecture
- Amazon EKS deployment
- Container orchestration
- Persistent storage using Amazon EBS
- Kubernetes Secrets & ConfigMaps
- GitHub Actions Continuous Deployment
- IAM authentication with Amazon EKS
- Debugging Kubernetes deployments

---

## 🔮 Future Improvements

- Helm Charts
- Ingress Controller
- Monitoring using Prometheus & Grafana
- Horizontal Pod Autoscaler
- GitOps using ArgoCD

---

## 👨‍💻 Author

Ashish Thakur

GitHub:
https://github.com/ashyT-Cloud# fittrack-k8s
