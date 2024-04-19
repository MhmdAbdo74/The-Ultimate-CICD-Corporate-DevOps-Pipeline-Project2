<div align="center">
  <h1 style="color: red;">🚀 Ultimate CI/CD Corporate DevOps Pipeline Project 🛠️  :globe_with_meridians::hammer_and_wrench:</h1>
</div> 

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
- Established a secure private Git repository.
- Implemented token-based authentication for enhanced security.
- Successfully pushed the source code into the repository, ensuring version control.

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

### 𝗣𝗵𝗮𝘀𝗲 4: 𝗠𝗼𝗻𝗶𝘁𝗼𝗿𝗶𝗻𝗴 🔍
- Implemented comprehensive monitoring solutions including:
-->System-level monitoring (CPU, RAM) using node_exporter
-->Website monitoring using blackbox_exporter
-->Leveraged Prometheus & Grafana for effective visualization and analysis.

### Result 
- RKE Cluster consist of 1 Master and 2 Worker
![RKE](https://github.com/github/gh-copilot/assets/94086189/9f228bf2-ba78-45e7-be6b-35b2378bc08d)

- Jenkins is configured with all the necessary plugins to ensure smooth pipeline execution.

![Jenkins](https://github.com/github/gh-copilot/assets/94086189/be8c6be8-a402-4460-97a2-862b316590b1)

- SonarQube is configured with all the necessary plugins to ensure smooth code quality analysis.

![Sonarqube](https://github.com/github/gh-copilot/assets/94086189/a1650127-7b6f-4820-a654-6c4e69c7e862)

-  sending  mail  alerts on failure or sucess in any stage of pipline  with trivy  image report file

![mail](https://github.com/github/gh-copilot/assets/94086189/60f2b5e7-ecb9-4772-b358-fae6f894de3a)



- you can acess deployed website from NodePort service
![website](https://github.com/github/gh-copilot/assets/94086189/4291ff37-67e4-480d-a1c3-bf64caede3cd)

- grafana dashboard to monitor the deployed website
![dashboard](https://github.com/github/gh-copilot/assets/94086189/cbad2ff7-843e-49e0-90bf-972cc6336bbb)


- grafana dashboard to monitor Jenkins Server
![dashboard](https://github.com/github/gh-copilot/assets/94086189/e014c240-863e-4b64-9d1e-b5ea4300a319)