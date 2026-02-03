cat <<EOF > README.md
# Yashas Flask Webapp (Dockerized)

A simple Python Flask web application containerized using Docker. This project demonstrates how to set up a lightweight Flask server and package it for easy deployment.

## 🚀 Features
* **Python 3.11-slim** base image for a small footprint.
* **Flask** web server running on port 8080.
* **Dockerized** for consistent environments across development and production.

## 🛠 Prerequisites
* [Docker Desktop](https://www.docker.com/products/docker-desktop/) installed on your machine.
* Git (optional, for cloning).

## 🏃 Getting Started

### 1. Build the Image
Navigate to the project directory and run:
\`\`\`bash
docker build -t yashas-flask-app .
\`\`\`

### 2. Run the Container
Map the internal port 8080 to your local machine:
\`\`\`bash
docker run -p 8080:8080 yashas-flask-app
\`\`\`

The app will be available at: **http://localhost:8080**

## 📦 Docker Hub
You can also pull the pre-built image directly:
\`\`\`bash
docker pull yashas775/yashas-simple-webapp-docker:latest
\`\`\`

## 📂 Project Structure
* \`app.py\`: The Flask application logic.
* \`Dockerfile\`: Instructions for building the Docker image.
* \`README.md\`: This documentation.
EOF
