# oba-hello-webapp

Simple containerized web application for AWS ECS deployment.

## Local Development

1. Build the container:
   ```bash
   docker build -t oba-hello-webapp .
   ```

2. Run locally:
   ```bash
   docker run -d -p 8081:80 oba-hello-webapp
   ```

3. Access the website at: http://localhost:8081

## AWS Deployment

1. Make sure AWS CLI is configured with proper credentials
2. Navigate to deploy directory and run:
   ```bash
   ./deploy-ecs.sh
   ```

## Environment Support
This project supports both local development (macOS) and EC2 deployment.
