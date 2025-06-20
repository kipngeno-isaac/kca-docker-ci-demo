# Containerization & CI/CD Demo Project

![Greeting App Screenshot](screenshot.png)

This project demonstrates containerization with Docker and CI/CD implementation using GitHub Actions. It features a simple web application that prompts users for their name and displays a personalized greeting message.

**Key Technologies Demonstrated:**
- Docker containerization
- GitHub Actions CI/CD pipeline
- Docker Hub image registry
- Nginx web server
- Client-side JavaScript

## Project Purpose

This sample project showcases:
1. Containerizing a static web application with Docker
2. Setting up automated CI/CD pipelines with GitHub Actions
3. Managing Docker image builds and deployments
4. Implementing industry best practices for container management
5. Creating a complete DevOps workflow from code to deployment

## Features

- **Containerization**:
  - Dockerized application using Alpine Linux
  - Multi-stage builds
  - Production-grade Nginx server
- **CI/CD Pipeline**:
  - Automated builds on code changes
  - Docker image versioning
  - Push to Docker Hub registry
- **Web Application**:
  - Personalized greeting functionality
  - Responsive design
  - Client-side name processing (no data storage)

## Getting Started

### Run the Application
```bash
# Run from Docker Hub
docker run -d -p 8080:80 kipngenoisaac/kca-docker-ci-demo

# Or build locally
docker build -t greeting-app .
docker run -d -p 8080:80 greeting-app
