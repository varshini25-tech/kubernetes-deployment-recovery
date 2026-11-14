# Local Kubernetes Application Deployment and Recovery

## Project Description
This project demonstrates the deployment, management, scaling, and recovery of a web application using Kubernetes and Minikube in a local environment. Nginx is used as the sample web application.

## Objectives
- Deploy a web application using Kubernetes.
- Create and manage Kubernetes Pods.
- Expose the application using a NodePort Service.
- Demonstrate automatic Pod recovery.
- Perform application scaling.
- Understand container orchestration using Kubernetes.

## Technologies Used
- Programming Language: YAML
- Containerization: Docker
- Orchestration: Kubernetes
- Local Cluster: Minikube
- Command-Line Tool: kubectl
- Web Server: Nginx
- Operating Environment: Ubuntu (WSL)
- Version Control: Git
- Repository Hosting: GitHub

## Project Architecture
1. Nginx runs inside a Docker container.
2. Kubernetes Deployment manages the application Pods.
3. Minikube provides the local Kubernetes cluster.
4. Kubernetes Service exposes the application through NodePort.
5. Kubernetes maintains the required number of replicas and replaces deleted Pods.

## Project Files
- deployment.yaml - Defines the application Deployment and replicas.
- service.yaml - Defines the NodePort Service.
- screenshots/ - Contains project implementation and testing screenshots.
- README.md - Project documentation.

## Implementation Methodology
1. Installed and configured Docker.
2. Installed and configured Minikube.
3. Started the local Kubernetes cluster.
4. Created the Nginx Deployment.
5. Configured the NodePort Service.
6. Accessed the Nginx application through a web browser.
7. Scaled the application to three replicas.
8. Deleted a running Pod to test automatic recovery.
9. Verified that Kubernetes created a replacement Pod.
10. Captured screenshots and uploaded the project to GitHub.

## Testing and Results

### Application Deployment
The Nginx application was successfully deployed using Kubernetes.

**Result:** Application Pods reached the Running state.

### Application Scaling
The Deployment was scaled to three replicas.

**Result:** All three Pods were running successfully (3/3 Ready).

### Automatic Pod Recovery
One running Pod was manually deleted to test Kubernetes recovery.

**Result:** Kubernetes automatically created a replacement Pod, and all three replicas returned to the Running state.

### Service Verification
The application was exposed using a NodePort Service on port 31818.

**Result:** The Nginx welcome page was successfully accessed through a web browser.

## Expected Outcome
A successfully deployed and accessible Nginx application with Kubernetes-based Pod management, automatic recovery, and application scaling.

## Conclusion
This project provides practical knowledge of container orchestration and Kubernetes application management. It demonstrates how Kubernetes Deployments maintain the desired number of replicas, automatically replace failed or deleted Pods, and expose applications through Services.

## Screenshots
Project implementation and testing screenshots are available in the screenshots folder.
