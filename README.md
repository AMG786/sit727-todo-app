# Spring Boot Todo Application with Kubernetes Deployment

![Screenshot 2025-03-29 083337](https://github.com/user-attachments/assets/fef1765b-39b8-4cb1-9af8-16e4874b46b4)

## 📝 Table of Contents
- [Project Overview](#-project-overview)
- [Key Features](#-key-features)
- [Technology Stack](#-technology-stack)
- [Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Local Development](#local-development)
  - [Docker Deployment](#docker-deployment)
  - [Kubernetes Deployment](#kubernetes-deployment)
- [Project Structure](#-project-structure)
- [Troubleshooting](#-troubleshooting)
- [Academic Context](#-academic-context)
- [License](#-license)




## 🌟 Project Overview
A Model-View-Controller (MVC) Todo application developed for **SIT727 Cloud Automation Technologies** demonstrating:
- Spring Boot backend with Thymeleaf frontend
- Containerization with Docker
- Kubernetes orchestration
- Cloud-native deployment patterns

📂 Project Structure
![image](https://github.com/user-attachments/assets/63a06cd2-4293-4fea-9970-010be118af50)


## 🚀 Key Features
- **Full CRUD Functionality**: Create, Read, Update, Delete tasks
- **H2 Database**: In-memory storage with automatic schema generation
- **Responsive UI**: Bootstrap-powered interface
- **Health Checks**: Kubernetes liveness/readiness probes
- **CI/CD Ready**: Docker and Kubernetes manifests included

## 🛠 Technology Stack

| Component        | Technology                          |
|------------------|-------------------------------------|
| Backend Framework | Spring Boot 3.1.5                   |
| Frontend         | Thymeleaf + Bootstrap 5             |
| Database         | H2 (Embedded)                       |
| Containerization | Docker (Multi-stage builds)         |
| Orchestration    | Kubernetes (Minikube for local)     |
| Java Version     | OpenJDK 17                          |

## 🏁 Getting Started

### Prerequisites
- Java 17 JDK
- Maven 3.8+
- Docker Desktop
- Minikube (v1.28+)
- kubectl CLI

### Local Development
```bash
# Clone repository
git clone https://github.com/AMG786/sit727-todo-app.git
cd sit727-todo-app

# Run application
mvn spring-boot:run
```
🐳 Docker Deployment
```bash
# Build image
docker build -t todo-app .

# Run container
docker run -p 8080:8080 todo-app
```
☸️ Kubernetes Deployment
```bash
# Start Minikube
minikube start

# Set Docker env
minikube docker-env
eval $(minikube docker-env)  # Linux/Mac

# Deploy
kubectl apply -f kubernetes/deployment.yaml
kubectl apply -f kubernetes/service.yaml

# Get URL
minikube service todo-service --url
```
📜 Log Inspection
```bash
# Docker logs
docker logs <container-id>

# K8s logs
kubectl logs <pod-name> -f  # Follow logs
```
