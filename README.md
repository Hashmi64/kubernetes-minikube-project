Project Steps:

1. Started Minikube
Launched a local Kubernetes cluster to run both the frontend and backend applications.

2. Activated Minikube Docker environment
Switched Docker to Minikube’s internal Docker engine so images are built directly inside the cluster.

3. Built the Flask backend Docker image
Created a Docker image for the backend API from the backend folder.

4. Built the Node.js frontend Docker image
Created a Docker image for the frontend application that submits data to the backend.

5. Created Kubernetes YAML files
Prepared Deployment and Service YAML files for both applications.
Frontend communicates with the backend using the backend service name inside Kubernetes.

6. Applied all Kubernetes deployments
Used kubectl apply commands to deploy the backend and frontend pods into the cluster.

7. Exposed the services
Backend exposed via ClusterIP (internal service).
Frontend exposed via NodePort to access it from the browser.

8. Verified running pods and services
Checked the cluster to ensure pods and services were running correctly using Kubernetes commands.

9. Opened the frontend using Minikube
Used Minikube to get the external URL and opened the frontend application in the browser.

Author: Mosharib Ahmad Hashmi
Solutions Architect | DevOps 

11. Tested frontend-to-backend communication
Submitted the form on the frontend, confirming that data was successfully sent to the Flask backend.
