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
```
---

## Commands
> Docker
> - sudo docker login -u <username> : This command logs you into Docker Hub with the specified username (karthikmp15), allowing you to pull or push images to/from your account.
> - sudo docker images : Lists all the Docker images available on your local machine, showing image names, tags, and their corresponding IDs.
> - sudo docker rmi <image_id>:<tag> --force : Removes a Docker image from your local system. You need to specify the image ID and tag (e.g., flask-chat-application:2.0.0). The --force flag forces the removal even if the image is in use.
> - sudo docker build -t <docker_file>:\<tag> . : Builds a Docker image from a Dockerfile located in the current directory (.). You need to specify a name (<docker_file>) and a tag (<tag>), such as flask-chat-application:2.0.0.
> - sudo docker push <username>/<repo_name:tag> : Pushes the local Docker image (flask-chat-application:2.0.0) to Docker Hub.

> Kubernetes
> - kubectl get nodes : Lists all the nodes in your Kubernetes cluster, showing details such as node name, status, and available resources.
> - kubectl apply -f kubernetes/<name>.yaml : Applies a Kubernetes YAML file to deploy or update resources (e.g., deployments, services) in the cluster. Replace <name> with the actual file name.
> - kubectl get deployments : Displays a list of deployments in the current namespace, showing details like name, desired replicas, and the current status.
> - kubectl get services : Lists the services in the current Kubernetes namespace, showing their names, cluster IPs, and exposed ports.
> - kubectl logs <pod-name> : Fetches and displays the logs of a specific pod (replace <pod-name> with the actual pod name).
> - kubectl get pods : Lists all the pods in the current Kubernetes namespace, displaying their names, statuses, and other details.
> - kubectl get pods --all-namespaces : Lists all the pods in the Kubernetes cluster across all namespaces, not just the current one.
> - kubectl get pod -o wide : Displays more detailed information about the pods, including their IP addresses and node assignments.
> - kubectl get svc : Displays details about the services in the current namespace, including cluster IPs, external IPs, and exposed ports.
> - kubectl scale deployment <deployment_name> --replicas=0 : Scales a deployment down to zero replicas, effectively stopping the application by removing all pods associated with the deployment.
> - kubectl delete deployment <deployment-name> : Deletes a deployment, removing all associated pods and resources.
> - kubectl describe pods <pod_name> : Displays detailed information about a specific pod, including events and error logs, which can be helpful for debugging deployment issues.







