# README.md

## Project Overview
This project is a cloud-native,intrusion detection system built using AWS services. The system allows users to upload network logs, which are processed using machine learning models to detect anomalies and potential threats. The architecture leverages AWS Fargate for containerized workloads.
## Features
- **Next.js Frontend**: Serves the user interface and interacts with backend APIs.
- **Flask Backend**: Runs ML inference on uploaded network logs.
- **Secure AWS Deployment**: Hosted using ECS Fargate for both frontend and backend.
- **File Storage**: Uses ECS task storage (/tmp) within the container for processing files as well as S3 storage for persistent storage.
- **Scalable and Secure**: Designed with AWS best practices including IAM, WAF, and AWS Shield.
- **Infastructure as Code (IaC)**: Fully provisioned with Terraform.

## Architecture
- **Frontend**: Next.js app running on AWS Fargate behind an ALB.
- **Backend**: Flask application running on AWS fargate behind an ALB
- **Storage**: S3 for file uploads and result storage.
- **Networking**: Uses private subnets, VPC endpoints, and ALB.

## Setup & Installation
### Prerequisites
- AWS CLI configured
- Terraform installed
- Docker installed
- Node.js & Python installed

### Infrastructure deployment (Terraform)
-- Go into the terraform folder, the details steps to provision the AWS infrastructure are outlined there.


## Contribution Guidelines
- Fork the repository.
- Create a feature branch.
- Submit a pull request with clear documentation .

## License
MIT License

