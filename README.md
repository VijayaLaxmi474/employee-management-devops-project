# Employee Management System - End-to-End DevOps Project

## Project Overview

This project demonstrates an End-to-End DevOps CI/CD Pipeline using Flask, Docker, Jenkins, GitHub, and Kubernetes.

The application is an Employee Management System that allows users to:

* Add Employees
* View Employees
* Delete Employees
* Health Check Endpoint

The goal of this project is to showcase DevOps skills including containerization, CI/CD automation, and deployment.

---

## Tech Stack

### Application

* Python
* Flask
* SQLite

### DevOps Tools

* Git
* GitHub
* Docker
* Docker Compose
* Jenkins
* Kubernetes
* Prometheus (Planned)
* Grafana (Planned)

---

## Project Architecture

GitHub → Jenkins → Docker Build → Docker Image → Kubernetes Deployment

---

## Features

* Employee CRUD Operations
* Health Monitoring Endpoint
* Dockerized Application
* Jenkins CI/CD Pipeline
* Kubernetes Deployment
* Containerized Environment

---

## API Endpoints

### Home Page

```http
GET /
```

### Employee List

```http
GET /employees
```

### Add Employee

```http
GET /add
POST /add
```

### Delete Employee

```http
GET /delete/<id>
```

### Health Check

```http
GET /health
```

---

## Local Setup

Clone Repository

```bash
git clone https://github.com/VijayaLaxmi474/employee-management-devops-project.git
```

Move to Project Directory

```bash
cd employee-management-devops-project
```

Create Virtual Environment

```bash
python3 -m venv venv

source venv/bin/activate
```

Install Dependencies

```bash
pip install -r requirements.txt
```

Run Application

```bash
python3 app.py
```

Application URL

```text
http://localhost:5000
```

---

## Docker Commands

Build Image

```bash
docker build -t employee-app:v1 .
```

Run Container

```bash
docker run -d -p 5000:5000 employee-app:v1
```

---

## Future Enhancements

* Docker Hub Integration
* Kubernetes Deployment
* Jenkins Webhook Trigger
* Prometheus Monitoring
* Grafana Dashboard
* AWS EKS Deployment

---

## Author

Vijaya Laxmi

DevOps Engineer | AWS | Docker | Kubernetes | Jenkins | Python
