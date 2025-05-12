# Node.js CI/CD with GitHub Actions and Docker

This is a demo project for automating code deployment using a CI/CD pipeline with GitHub Actions and Docker.

## 🔧 Tools Used
- Node.js
- Docker & DockerHub
- GitHub Actions

## ⚙️ CI/CD Workflow Steps
1. Triggered on push to `main`
2. Installs dependencies and runs tests
3. Builds a Docker image
4. Pushes the image to DockerHub

## 📦 Docker Image
The image is published to:  
`docker.io/<your-docker-username>/nodejs-task1-app:latest`

## 🔐 Secrets Used
- `DOCKER_USERNAME`: Your DockerHub username
- `DOCKER_PASSWORD`: Your DockerHub password or token

## 🚀 Run Locally
```bash
docker run -p 3000:3000 <your-docker-username>/nodejs-task1-app

 Repo Structure
 
.github/workflows/main.yml: GitHub Actions CI/CD pipeline

Dockerfile: Docker image config

app.js: Node.js app

package.json: Dependencies and scripts