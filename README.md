# cujo-spring-app

**Java on Kubernetes. The hard way.**

[![CI/CD](https://github.com/DamianoNicotra/cujo-spring-app/actions/workflows/deploy.yml/badge.svg)](https://github.com/DamianoNicotra/cujo-spring-app/actions/workflows/deploy.yml)

A production-ready Spring Boot application fully deployed on AWS EKS (Kubernetes). Infrastructure as code, CI/CD pipeline, and cloud-native best practices — all automated.

## 🧱 Project structure

The project is split into two logical parts:

### Part 1 – Java + Spring Boot + PostgreSQL (local)
- REST API with full CRUD operations
- Hibernate ORM for database mapping
- Maven build lifecycle
- PostgreSQL database (runs locally during development)

### Part 2 – Container + Cloud + Kubernetes
- Docker image built and pushed to Amazon ECR
- Infrastructure as Code using **Terraform** (VPC, EKS, RDS, ECR)
- Kubernetes deployment with LoadBalancer service
- Full CI/CD pipeline with **GitHub Actions**

## 🚀 Live demo

> The API is live. The database is managed (RDS). The infrastructure is reproducible. The code is on GitHub.

## 🛠️ Tech stack

| Layer | Technology |
|-------|------------|
| Language | Java 17 |
| Framework | Spring Boot 3 |
| Build tool | Maven |
| Database | PostgreSQL (RDS) |
| ORM | Hibernate |
| Container | Docker |
| Container registry | Amazon ECR |
| Orchestration | Kubernetes (EKS) |
| IaC | Terraform |
| CI/CD | GitHub Actions |
| Cloud | AWS (EKS, RDS, VPC, ECR) |

## 📦 Run locally (Part 1)

```bash
git clone https://github.com/DamianoNicotra/cujo-spring-app.git
cd cujo-spring-app
./mvnw spring-boot:run
