<div align="center">
  <h1 style="color: red;">🚀 Ultimate CI/CD Corporate DevOps Pipeline Project 🛠️  :globe_with_meridians::hammer_and_wrench:</h1>
</div> 

# 🚀 DevOps Project

Corporate DevOps Pipeline: Orchestrating seamless CI/CD with Jenkins, Kubernetes, Git, and SonarQube. Securely manage source code, build Docker images, and deploy to Kubernetes. Enhanced with comprehensive monitoring solutions for real-time insights. Empower your development workflow with efficient automation and robust quality checks.
##  Project Design
![devops-task](https://github.com/github/gh-copilot/assets/94086189/63039717-682c-4bc2-b129-74db4d81f449)

## :gear: Tools  :
- Docker
- Terraform
- K8S (RKE)
- Sonarqube
- Rancher
- Jenkins
- Nexus
- Trivy
- promethus
- Grafana
- mail


### Steps
### 𝗣𝗵𝗮𝘀𝗲1. Provision Infrastructure using Terraform
- start building your Infrastructure using terraform --> (VPC, Public Subnet , IGW , Route Table, Security Group,  and EC2 that used to create jenkins ,
 sonarqube  , nexus , Rancher , promethus, grafana )

### 𝗣𝗵𝗮𝘀𝗲 𝟮: 𝗦𝗲𝘁𝘂𝗽 𝗣𝗿𝗶𝘃𝗮𝘁𝗲 𝗚𝗶𝘁 𝗥𝗲𝗽𝗼
-Established a secure private Git repository.
-Implemented token-based authentication for enhanced security.
-Successfully pushed the source code into the repository, ensuring version control.

### 𝗣𝗵𝗮𝘀𝗲 𝟯: 𝗖𝗼𝗻𝗳𝗶𝗴𝘂𝗿𝗲 𝗝𝗲𝗻𝗸𝗶𝗻𝘀 & 𝗖𝗜𝗖𝗗 𝗣𝗶𝗽𝗲𝗹𝗶𝗻𝗲 🔧
- In this phase, we configured Jenkins with essential plugins to ensure smooth pipeline execution. The CI/CD pipeline was meticulously designed with various stages, including:-Source Code.
- Definition: Define source code from the repository.
- Compilation: Compile the source code.
- Testing: Execute automated tests.
- File System Scan / Dependency Check Scan: Scan the file system for vulnerabilities or dependency issues.
- SonarQube Analysis: Perform code quality analysis using SonarQube.
- Quality Gate Check: Ensure code meets predefined quality standards.
- Building/Packaging Application: Construct application artifacts.
- Publishing Application Artifacts to Nexus: Publish artifacts to Nexus repository.
- Building & Tagging Docker Images: Build Docker images and assign appropriate tags.
- Vulnerability Scanning of Docker Images: Scan Docker images for vulnerabilities.
- Docker Image Pushing to Registry: Push Docker images to a registry.
- Deployment to Kubernetes Clusters: Deploy application to Kubernetes clusters.
- Verification of Deployment using Trivy: Verify successful deployment using Trivy.
- Pushing Docker Images to Docker Hub Repository: Push Docker images to Docker Hub repository.
- Deployment of Application Artifacts to Kubernetes: Deploy application artifacts to Kubernetes.
- Verification of Deployment: Verify successful deployment.
- Deployment of Application Artifacts to Docker Hub Repository: Deploy application artifacts to Docker Hub repository.
- Verification of Deployment: Verify successful deployment.