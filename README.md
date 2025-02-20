# Online Shop App Documentation

This guide provides step-by-step instructions to set up, build, and deploy the `online_shop` app using Docker and Docker Compose. The app is a Node.js-based online shopping platform designed to be easily deployable and scalable.

---

## **Table of Contents**
1. [Prerequisites](#prerequisites)
2. [Project Setup](#project-setup)
3. [Docker Setup](#docker-setup)
4. [Docker Compose Setup](#docker-compose-setup)
5. [Troubleshooting](#troubleshooting)
6. [Final Submission](#final-submission)

---

## **Prerequisites**
Before starting, ensure you have the following installed:
- **Node.js** (v18 or higher)
- **npm** (v8 or higher)
- **Docker** (v20 or higher)
- **Docker Compose** (v2 or higher)
- **Git**

---

## **Project Setup**
Command | Description
--- | ---
`git clone https://github.com/59Raaj/online_shop.git` | Clone the repository.
`cd online_shop` | Navigate to the project directory.
`npm install` | Install project dependencies.
`sudo apt install npm` | Install npm (if not already installed).

---

## **Docker Setup**
Command | Description
--- | ---
`sudo apt update` | Update the package list.
`sudo apt install docker.io` | Install Docker.
`sudo systemctl start docker` | Start the Docker service.
`sudo usermod -aG docker ubuntu && newgrp docker` | Add your user to the Docker group.
`docker build -t online_shop .` | Build the Docker image.
`docker run -d -p 3000:3000 --name online_shop_container online_shop` | Run the Docker container.
`docker ps` | Check running containers.
`docker logs online_shop_container` | View container logs.

---

## **Docker Compose Setup**
Command | Description
--- | ---
`sudo curl -L "https://github.com/docker/compose/releases/download/v2.23.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose` | Install Docker Compose.
`sudo chmod +x /usr/local/bin/docker-compose` | Make Docker Compose executable.
`docker-compose --version` | Verify Docker Compose installation.
`docker-compose up --build` | Start the app using Docker Compose.
`docker-compose down` | Stop the app.

---

## **Troubleshooting**
Command | Description
--- | ---
`docker stop <container_id>` | Stop a running container.
`docker rm <container_id>` | Remove a container.
`docker rmi <image_id>` | Remove a Docker image.
`docker history <image_id>` | View the history of a Docker image.
`docker inspect <container_id_or_image_id>` | Inspect a container or image.

---

## **Final Submission**

### **Update GitHub Repository**
Command | Description
--- | ---
`git add .` | Stage all changes.
`git commit -m "Final submission for Hackathon Phase 1"` | Commit changes.
`git push origin main` | Push changes to GitHub.

-----

## **Conclusion**
This documentation provides all the steps needed to set up, build, and deploy the `online_shop` app using Docker and Docker Compose. If you encounter any issues, refer to the troubleshooting section or check the Docker logs.

---

Enjoy building and deploying your online shop app
