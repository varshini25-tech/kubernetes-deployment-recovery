# Local Kubernetes Application Deployment and Recovery

## Project Description
This project demonstrates how to deploy and manage a web application locally using Kubernetes and Minikube.

## Objectives
- Deploy an Nginx web application.
- Manage application Pods using Kubernetes.
- Expose the application using NodePort Service.
- Demonstrate automatic Pod recovery.
- Perform application scaling.

## Technologies Used
- Docker
- Kubernetes
- Minikube
- kubectl
- Nginx
- Ubuntu (WSL)
- Git
- GitHub

## Project Files
- deployment.yaml - Application deployment configuration.
- service.yaml - Service configuration.
- README.md - Project documentation.

## Implementation
1. Installed and configured Docker.
2. Started the Minikube cluster.
3. Deployed the Nginx application.
4. Created a NodePort Service.
5. Accessed the application through a browser.
6. Tested automatic Pod recovery.
7. Scaled the application from 1 Pod to 2 Pods.
8. Scaled down from 2 Pods to 1 Pod.
9. Uploaded the project to GitHub.

## Testing and Results

### Automatic Pod Recovery
A running Nginx Pod was deleted manually. Kubernetes automatically created a replacement Pod.

**Result:** Pod recovery was successful.

### Application Scaling
The application was scaled from 1 Pod to 2 Pods and then back to 1 Pod.

**Result:** Scaling was successful.

## Expected Outcome
A successfully deployed Nginx application with Kubernetes deployment, service management, automatic recovery and scaling.

## Conclusion
This project provides practical knowledge of Kubernetes application deployment and management. It demonstrates how Kubernetes can automatically recover Pods and manage application scaling.
