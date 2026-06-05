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

<img width="1774" height="887" alt="image" src="https://github.com/user-attachments/assets/c8401889-0363-412c-b567-640cfa0efeda" />

  <img width="1917" height="1077" alt="image" src="https://github.com/user-attachments/assets/96093e56-591e-4b58-b55b-a804b5addcc0" />
  <img width="1917" height="1077" alt="image" src="https://github.com/user-attachments/assets/d266107d-347e-41be-ad35-7ca55f1310e5" />
  <img width="1917" height="1077" alt="image" src="https://github.com/user-attachments/assets/5c7700fb-73d4-4ce6-b410-6bc385355858" />
  <img width="1917" height="1077" alt="image" src="https://github.com/user-attachments/assets/cb43a725-5860-4393-8b76-1b4312b8c458" />





## Author

Vaishnavi
