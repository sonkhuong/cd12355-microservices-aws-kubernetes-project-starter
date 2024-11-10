
# Project: Operationalizing a Co-working Space Service
## Coworking Space Service Extension
The Coworking Space Service comprises a suite of APIs that enable users to request one-time tokens and allow administrators to manage access to coworking spaces. Following a microservice architecture, each service is designed to be deployed and managed independently.

In this project, as the DevOps engineer, you will collaborate with a team responsible for developing an API that delivers key analytics on user activity within the service. Although the application runs smoothly in a local environment, your primary task is to create a pipeline for its deployment in a Kubernetes cluster.

## Getting Started
### Dependencies
#### Local Environment
1.  **Python Environment**: Required to run Python 3.8+ applications and install Python dependencies using `pip`.
2.  **Docker CLI**: Essential for building and running Docker images locally.
3.  **kubectl**: Necessary to execute commands against a Kubernetes cluster.
4.  **helm**: Needed to apply Helm Charts to a Kubernetes cluster.

#### Remote Resources
1.  **AWS CodeBuild**: Used for remote Docker image builds.
2.  **AWS ECR**: Hosts Docker images.
3.  **Kubernetes Environment with AWS EKS**: Deploys applications in Kubernetes.
4.  **AWS CloudWatch**: Monitors activity and logs in EKS.
5.  **GitHub**: Pulls and clones the code repository.

#### Project Structure
```
├── CODEOWNERS
├── LICENSE.txt
├── README.md
├── buildspec.yml
├── analytics
│ ├──  Dockerfile
│ ├──  __init__.py
│ ├──  app.py
│ ├──  config.py
│ └──  requirements.txt
├── db
│ ├──  1_create_tables.sql
│ ├──  2_seed_users.sql
│ └──  3_seed_tokens.sql
├── deployment
│ ├──  configmap.yaml
│ ├──  coworking.yaml
│ └──  secret.yaml
├── deployment-local
│ ├──  configmap.yaml
│ └──  coworking.yaml
├── evidences
│ ├──  *.png
```
-  `db`: SQL scripts for seeding data.
-  `deployment`: Kubernetes YAML files for deployment and configuration.
-  `evidences`: Program screenshot.

### Get Web API URL
The Web API:
```

```