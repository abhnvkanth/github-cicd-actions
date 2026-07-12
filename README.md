# 🚀 Spring Boot CI/CD Pipeline with Docker & GitHub Actions

![Java](https://img.shields.io/badge/Java-21-orange?style=for-the-badge&logo=openjdk)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-green?style=for-the-badge&logo=springboot)
![Docker](https://img.shields.io/badge/Docker-Containerized-blue?style=for-the-badge&logo=docker)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-CI%2FCD-2088FF?style=for-the-badge&logo=githubactions)

> End-to-end CI/CD pipeline for a Spring Boot application using **GitHub Actions**, **Docker**, and **Docker Hub**. Every push automatically builds the project, creates a Docker image, and publishes it to Docker Hub.

---

## 📖 Overview

This project demonstrates a complete Continuous Integration and Continuous Deployment (CI/CD) workflow for a Spring Boot application.

Whenever code is pushed to the **master** branch, GitHub Actions automatically:

- Builds the application using Maven
- Compiles and packages the project
- Creates a Docker image
- Pushes the Docker image to Docker Hub

The published image can then be pulled and run anywhere using Docker.

---

## 🏗 Architecture

```

Developer
│
│ git push
▼
GitHub Repository
│
▼
GitHub Actions
│
├── Checkout Code
├── Setup Java 21
├── Maven Build
├── Build Docker Image
└── Push Image to Docker Hub
│
▼
Docker Hub
│
▼
docker pull
│
▼
Docker Container
│
▼
Spring Boot Application

```

---

## 🛠 Tech Stack

- Java 21
- Spring Boot
- Maven
- Docker
- GitHub Actions
- Docker Hub

---

## ⚙ CI/CD Workflow

The GitHub Actions pipeline performs the following steps:

- Checkout source code
- Setup Java 21
- Build project with Maven
- Build Docker image
- Push Docker image to Docker Hub

Pipeline Location:

```

.github/workflows/maven.yml

```

---

## 📂 Project Structure

```

github-cicd-actions/
│
├── .github/
│ └── workflows/
│ └── maven.yml
│
├── src/
│ ├── main/
│ └── test/
│
├── Dockerfile
├── pom.xml
└── README.md

```

---

## 🐳 Docker Commands

### Pull Image

```bash
docker pull abhinavkanth234/springboot-images-new:latest
```

### Run Container

```bash
docker run -p 8080:8080 abhinavkanth234/springboot-images-new:latest
```

---

## 🌐 Test Application

Open:

```
http://localhost:8080/welcome
```

Response:

```
Welcome to Java
```

---

## 📸 Screenshots

### ✅ GitHub Actions Build

> *(Add your successful GitHub Actions screenshot here)*

---

### ✅ Docker Hub Image

> *(Add your Docker Hub repository screenshot here)*

---

### ✅ Running Application

> *(Add your browser screenshot showing "Welcome to Java")*

---

## 💡 Key Features

- Automated CI/CD pipeline
- Maven Build Automation
- Docker Image Creation
- Docker Hub Integration
- Spring Boot REST API
- Java 21 Support
- GitHub Actions Automation

---

## 🚀 Future Improvements

- Add Unit Testing
- Add Multi-stage Docker Build
- Deploy using Docker Compose
- Integrate Prometheus & Grafana
- Deploy to Kubernetes
- Add SonarQube Code Analysis

---

## 👨‍💻 Author

**Abhinav Kanth**

GitHub: https://github.com/abhnvkanth

Docker Hub: https://hub.docker.com/u/abhinavkanth234

---

## ⭐ If you found this project useful, consider giving it a star!
