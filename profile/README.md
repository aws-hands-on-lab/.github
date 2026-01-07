# AWS Hands-On Lab

This organization is a **hands-on, real-world AWS learning project** focused on building, deploying, and evolving applications on AWS the same way they are built in real companies.

The goal is **not to memorize AWS services**, but to learn them by solving real problems step by step.

---

## 🎯 Objective

- Learn AWS through **actual implementations**
- Start small and **grow systems incrementally**
- Understand **why** a service is used, not just **how**
- Build confidence to design real-world AWS architectures
- Create a long-term reference for production-ready patterns

---

## 🧠 Learning Philosophy

> Never introduce an AWS service unless a real problem demands it.

This lab intentionally avoids shortcuts and over-engineering.  
Each service is added only when the existing setup starts to show limitations.

---

## 🏗️ High-Level Architecture Vision

Over time, this lab will cover:

- EC2-based deployments
- Containerized workloads (ECS on EC2, ECS Fargate)
- Serverless workloads (AWS Lambda)
- Secure networking using VPC, private subnets, and endpoints
- Internal microservice communication without public exposure
- Configuration management using Parameter Store and AppConfig
- Databases using RDS and Aurora
- CI/CD using GitHub Actions (and later advanced tools)
- DNS, routing, and traffic management
- Cost-aware and security-first design

---

## 📁 Repository Structure

Each concern is separated clearly, just like in real teams.

### 1️⃣ Infrastructure

- AWS infrastructure using Terraform
- VPC, subnets, ALB/NLB
- EC2, ECS, Lambda
- IAM, Parameter Store, AppConfig
- RDS, Aurora
- VPC Endpoints
- Environment-based setup (dev → prod)

---

### 2️⃣ Backend Services
Example:
order-service/
product-service/
payment-service/

- Spring Boot microservices
- Evolve from EC2 → ECS → Lambda
- Secure internal communication
- Realistic service boundaries

---

### 3️⃣ Frontend
- React application
- Hosted on S3 + CloudFront
- Communicates only via public ALB/API endpoints

---

## 🚀 Learning Roadmap

### Phase 1: Foundations
- Single Spring Boot service
- EC2 in private subnet
- ALB (HTTP initially)
- Parameter Store for configuration
- CI/CD using GitHub Actions

### Phase 2: Containers
- Dockerize services
- ECS on EC2
- Internal service discovery
- Rolling deployments

### Phase 3: Serverless Containers
- ECS Fargate
- Auto scaling
- Blue/green deployments

### Phase 4: Serverless Functions
- Lambda for event-driven services
- API Gateway and async workflows
- Cost and performance trade-offs

### Phase 5: Advanced Topics
- VPC Endpoints with real cost/security reasons
- RDS and Aurora
- AppConfig with feature flags
- Route 53 and HTTPS with ACM
- Multi-environment setup (dev/prod)

---

## 🌍 AWS Region

All infrastructure is initially built in:
ap-south-1 (Mumbai)

This keeps latency low and aligns with real usage in India.

---

## 💡 Who This Is For

- Developers who want **real AWS experience**
- Engineers preparing for senior/architect roles
- Anyone tired of shallow tutorials without context

---

## 📌 Important Notes

- This is a **living project**
- Architecture will evolve intentionally
- Decisions are documented along the way
- Trade-offs are explained, not hidden

---

## ✅ Status

🚧 Actively evolving  
Starting with: **EC2-based Spring Boot deployment**

---

## 📄 License

MIT (or add later)
