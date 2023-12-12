# Web Deployment

## Description

This repository contains the source code for Web Deployment. The project is built with Maven and deploys a WAR file to a Tomcat server using GitHub Actions.

## Workflow

The deployment workflow is triggered on every push to the `main` branch. It builds the project with Maven and deploys the generated WAR file to a remote Tomcat server.

### Prerequisites

- JDK 11
- Maven
- Access to a Tomcat server with SSH configured

### Workflow Steps

1. **Build with Maven**: The workflow sets up the JDK, checks out the code, and builds the project using Maven.

2. **Deploy to Tomcat**: The workflow deploys the WAR file to the Tomcat server using SSH. The necessary server details are stored as GitHub secrets.

## Usage

To use this project, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/pavankumarindian/GitHubActions-WebAppDeployment.git

1. Configure your Tomcat server details as GitHub secrets:
    TOMCAT_HOST: The hostname or IP address of your Tomcat server.
    TOMCAT_USERNAME: The username for SSH access to your Tomcat server.
    TOMCAT_PASSWORD: The password for SSH access to your Tomcat server.

2. Push changes to the main branch to trigger the deployment workflow.

## License
This project is licensed under the MIT License.
