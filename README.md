# Monolithic Architecture Development Lifecycle

This project aims to establish a streamlined software development lifecycle for a company following a monolithic architecture. It includes version control, continuous integration, containerization, deployment to Kubernetes, infrastructure creation using Terraform, and configuration management using Jenkins and Terraform.

## Project Overview

The project implements the following components:

1. **Git Workflow**: Version control system to manage code changes. Releases occur monthly on the 25th.
2. **Continuous Integration (CI)**: Jenkins pipeline script triggers code builds upon commits to the master branch.
3. **Containerization**: Dockerfile is used to containerize the code, and a custom Docker image is built upon each push to GitHub.
4. **Deployment to Kubernetes**: Containerized code from Docker Hub is deployed to a Kubernetes cluster with 2 replicas. A NodePort service is configured on port 30008.
5. **Infrastructure Creation with Terraform**: Infrastructure provisioning on AWS cloud provider using Terraform.
6. **Configuration Management**: Jenkins and Terraform manage software installations and configurations on worker machines.

## Architecture

The project involves the following worker machines:

- **Worker1**: Jenkins and Java are installed.
- **Worker2**: Docker and Kubernetes are installed.
- **Worker3**: Java, Docker, and Kubernetes are installed.
- **Worker4**: Docker and Kubernetes are installed.

## Getting Started

To get started with this project, follow these steps:

1. Set up Git workflow according to the established guidelines.
2. Install and configure Jenkins on Worker1.
3. Install Docker and Kubernetes on Worker2, Worker3, and Worker4.
4. Create a Dockerfile in your project repository for containerization.
5. Configure Jenkins pipeline script to trigger builds and deployments.
6. Configure Terraform for infrastructure provisioning on AWS.
7. Customize Terraform configurations for specific software installations and configurations on worker machines.

## Contribution

Contributions to this project are welcome! Please open an issue to discuss proposed changes or submit a pull request with improvements.

## License

This project is licensed under the [MIT License](LICENSE).
