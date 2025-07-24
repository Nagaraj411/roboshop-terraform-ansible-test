# 🛠️ Roboshop Terraform + Ansible Automation

This repository demonstrates **end-to-end automation** of the Roboshop e-commerce application using **Terraform** for AWS infrastructure provisioning and **Ansible** for application configuration and deployment. It follows DevOps best practices to deliver a scalable and modular microservices setup.

---

## 🚀 Project Highlights

- 📦 **Terraform** provisions AWS infrastructure (VPC, EC2, security groups, etc.)
- 🤖 **Ansible** configures application services like catalogue, frontend, user, cart, and databases
- 🧱 Each microservice is handled via **dedicated Ansible roles**
- 🔄 Supports **repeatable deployments** for dev/test/prod environments

---

## 📂 Services Included (Ansible Roles)

| Role       | Description                                |
|------------|--------------------------------------------|
| `catalogue`| Node.js-based product catalogue service     |
| `frontend` | Nginx frontend UI setup                     |
| `user`     | User service connected to MongoDB           |
| `cart`     | Cart service with Redis backend             |
| `shipping` | Shipping service using MySQL                |
| `payment`  | Payment service written in Python           |
| `mongodb`  | MongoDB database setup                      |
| `redis`    | Redis installation and configuration        |
| `mysql`    | MySQL setup for shipping service            |
| `rabbitmq` | RabbitMQ messaging service                  |


---

## 🧪 How to Deploy

### Step 1: Provision AWS Infrastructure (Terraform)
```bash
cd terraform
terraform init
terraform apply -auto-approve
