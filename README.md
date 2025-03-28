# Spring Boot Todo Application with Kubernetes Deployment

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
