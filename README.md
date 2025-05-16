# ci-cd-jenkins

## 🛠️ Jenkins CI/CD Pipeline Design

This repository is integrated with Jenkins and follows a 7-stage CI/CD pipeline. Below are the pipeline stages, their tasks, and the tools used.

| Stage | Task Description | Tool Used |
|-------|------------------|-----------|
| **1. Build** | Compile the source code and package the application. | Maven |
| **2. Unit and Integration Tests** | Execute unit tests and integration tests to verify application logic and component interaction. | JUnit and TestNG |
| **3. Code Analysis** | Analyze the code for quality, maintainability, and standard compliance. | SonarQube |
| **4. Security Scan** | Scan for security vulnerabilities in the source code and dependencies. | OWASP Dependency-Check |
| **5. Deploy to Staging** | Deploy the application to a staging environment for testing. | AWS EC2 instance (via Ansible or SSH) |
| **6. Integration Tests on Staging** | Perform end-to-end and integration testing in a production-like environment. | Selenium |
| **7. Deploy to Production** | Deploy the verified application to the production environment. | AWS EC2 instance (via Ansible or SSH) |
