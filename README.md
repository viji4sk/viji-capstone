# Cloud DevOps Engineer Capstone Project

## Whats used in this project
- Using Circle CI to implement Continuous Integration and Continuous Deployment
- Building pipelines
- Working with Ansible and CloudFormation to deploy clusters
- Building Kubernetes clusters
- Building Docker containers in pipelines
- Working in AWS

## Kubernetes Cluster
AWS CloudFormation to deploy the Kubernetes Cluster.
The CloudFormation Deployment can be broken down into four Parts:
- **Networking**, to ensure new nodes can communicate with the Cluster
- **Elastic Kubernetes Service (EKS)** is used to create a Kubernetes Cluster
- **NodeGroup**, each NodeGroup has a set of rules to define how instances are operated and created for the EKS-Cluster
- **Management** is needed to configure and manage the Cluster and its deployments and services. I created two management hosts for extra redundancy if one of them fails.

#### List of deployed Stacks:
![image](https://user-images.githubusercontent.com/94306530/148208354-ffee5368-86be-4731-9188-d73e23aae114.png)

#### List of deployed Instances:
![image](https://user-images.githubusercontent.com/94306530/148208823-41c3e34c-3cb9-4931-8f82-b81f153b88d5.png)

## CircleCi - CI/CD Pipelines
CircleCi to create a CI/CD Pipeline to test and deploy changes manually before they get deployed automatically to the Cluster using Ansible.
![image](https://user-images.githubusercontent.com/94306530/148208576-35e0f2a1-35c8-46ff-ac85-513fee543fbd.png)

## Linting using Pylint and Hadolint

#### Lint fails:



#### Lint passes:


## Access the Application

Public LB DNS: http:/a83672434bb60467e8ebcb3c9b3dc282-537929929.us-east-1.elb.amazonaws.com
<here>
