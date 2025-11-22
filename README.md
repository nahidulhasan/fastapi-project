Overview

This project demonstrates how to build, containerize, and deploy a FastAPI microservice on Google Kubernetes Engine (GKE) using GitHub Actions CI/CD.
It includes:

FastAPI application

Docker image pushed to Google Artifact Registry

Kubernetes Deployment + LoadBalancer Service

Automated CI/CD pipeline using GitHub Actions

Publicly accessible endpoint through GKE LoadBalancer


🔧 Prerequisites

Before deploying, ensure you have:

Google Cloud account (Free Tier or paid)

GKE cluster created

Artifact Registry repository created

Service Account with required permissions:

Artifact Registry Writer

Kubernetes Engine Developer

Service Account User

Service account key stored in GitHub Secrets:

GCP_SA_KEY

🤖 GitHub Actions CI/CD

The pipeline does:

Authenticate to Google Cloud

Build & push Docker image to Artifact Registry

Apply Kubernetes manifests

Redeploy automatically on every git push to main

📜 License

MIT License
