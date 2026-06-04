GitHub Actions ECR Test# End-to-End DevOps Pipeline using Flask, Docker, GitHub Actions, AWS ECR, and EC2

## Project Overview

This project demonstrates a complete DevOps CI/CD pipeline using:

* Python Flask Application
* Docker
* Git & GitHub
* GitHub Actions
* AWS Elastic Container Registry (ECR)
* AWS EC2
* AWS CloudWatch

## Architecture

```text
GitHub
   |
GitHub Actions
   |
Docker Build
   |
AWS ECR
   |
EC2
   |
CloudWatch
```

## Technologies Used

* Python 3.11
* Flask
* Docker
* Git
* GitHub
* GitHub Actions
* AWS ECR
* AWS EC2
* AWS CloudWatch

## Application

### Endpoint

```http
GET /
```

### Response

```json
{
  "status": "success",
  "message": "DevOps Pipeline Working"
}
```

## Local Setup

```bash
pip install -r requirements.txt
python app.py
```

## Docker Commands

```bash
docker build -t flask-devops .
docker run -d -p 5000:5000 --name flask-container flask-devops
```

## AWS ECR

Repository:

```text
714610887687.dkr.ecr.ap-south-1.amazonaws.com/flask-devops
```

## CI/CD Workflow

1. Push code to GitHub
2. GitHub Actions builds Docker image
3. Image pushed to AWS ECR
4. Deployment to EC2/ECS
5. Monitoring using CloudWatch

## GitHub Secrets

* AWS_ACCESS_KEY_ID
* AWS_SECRET_ACCESS_KEY
* AWS_REGION
* ECR_REPOSITORY

## Author

Vaishnavi
