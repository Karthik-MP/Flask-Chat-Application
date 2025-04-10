# Flask Chat Application with WebSockets and MongoDB

This project is a simple **Flask chat application** built using **WebSockets** and **MongoDB**. The application allows users to send real-time messages in a chat environment. The project is containerized using **Docker** and deployed in a **Kubernetes** cluster.

---

## Features

- **Real-Time Chat**: Uses WebSockets for real-time communication.
- **MongoDB**: Stores chat messages in a MongoDB database.
- **Kubernetes Deployment**: Scalable and containerized in a Kubernetes environment.
- **Dockerized**: Both Flask web server and MongoDB are packaged in Docker containers.
- **Multi-Replica Flask**: Deployed with 3 replicas for high availability.
  
---

## Architecture

- **Flask Web Server**: The backend for the chat application, serving WebSocket connections and handling chat logic.
- **MongoDB**: Database used for storing chat messages.
- **Kubernetes**: Orchestrates the deployment of Flask and MongoDB services in the cluster.
- **Docker**: Used to create containers for the Flask app and MongoDB.

---

## Requirements

- **Kubernetes**: A Kubernetes cluster to deploy the application (e.g., Minikube for local testing or a cloud provider like GKE, EKS, or AKS).
- **Docker**: For building and running the application in containers.
- **MongoDB**: MongoDB database to store chat messages.

---

## Project Setup

### Step 1: Clone the Repository
---

# Demo Video
- **Docker**: https://youtu.be/AQqv_t3dFpo
- **Kubernetes**: https://youtu.be/ojIXbIo4VOI
```bash
- git clone https://github.com/Karthik-MP/Flask-Chat-Application/
- Docker Flask Images: https://hub.docker.com/repository/docker/karthikmp15/flask-chat-application/
- Docker Mongodb Images: https://hub.docker.com/repository/docker/karthikmp15/mongodb/

