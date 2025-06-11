# **End-to-End CI/CD Pipeline with Jenkins for Container Deployment to ECS via ECR**

---

## **Description**

This project demonstrates how to build a complete **CI/CD (Continuous Integration and Continuous Deployment)** pipeline using **Jenkins**, **Docker**, **Amazon ECR (Elastic Container Registry)**, and **Amazon ECS (Elastic Container Service)**.

The goal is to automate the **entire software delivery process**—from source code changes to production deployment in containers.

### How It Works:

1. Developers push code changes to a GitHub (or AWS CodeCommit) repository.  
2. Jenkins automatically triggers the pipeline:
   - Pulls the latest code  
   - Builds a Docker image  
   - Runs unit tests  
   - Pushes the Docker image to **Amazon ECR**  
   - Updates the **ECS Cluster** to deploy the new container image automatically  

This system **eliminates manual deployments**, **reduces errors**, and enables **fast, reliable, and repeatable container releases**, supporting DevOps and microservices-based application delivery.

---

## **Technologies Used**

| Technology              | Purpose                                             |
|-------------------------|-----------------------------------------------------|
| **Jenkins**             | Automation server to orchestrate the pipeline       |
| **Docker**              | Containerization platform to package applications   |
| **Amazon ECR**          | Secure container image storage                      |
| **Amazon ECS (Fargate or EC2)** | Container orchestration and deployment        |
| **GitHub / Git**        | Source code repository                              |
| **IAM Roles and Policies** | Secure access control and authentication         |

---

## **Results / Outcome**

- Every code push **triggers an automated CI/CD pipeline**  
- Docker images are **automatically built, tested, and pushed to Amazon ECR**  
- ECS service is **updated automatically** with the latest image version  
- Enables **rapid, reliable, and scalable deployments** to production or staging environments  
- **DevOps best practices** are enforced, improving release frequency and quality  
- **Manual errors and downtime** are minimized through full pipeline automation  
