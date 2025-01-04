# Lambda Hosting Deployment

This repository demonstrates how to deploy an ASP.NET Core application to AWS Lambda using AWS Lambda hosting. It utilizes the `Amazon.Lambda.AspNetCoreServer` package to host the application as a Lambda function, making it easily deployable in a serverless architecture.

## Overview

The goal of this project is to provide a simple yet comprehensive solution for deploying a .NET Core Web API to AWS Lambda, using GitHub Actions to automate the build and deployment process.

### Key Features:
- **AWS Lambda Hosting**: Easily deploy .NET Core applications to AWS Lambda using the `Amazon.Lambda.AspNetCoreServer.Hosting` package.
- **CI/CD integration with GitHub Actions**: Automates the build and deployment process using GitHub Actions.
- **Support for multiple Web APIs**: The project can be configured to deploy multiple Web APIs via matrix deployments.
- **Environment configuration**: AWS Lambda function configurations such as role, memory size, timeout, and environment variables are fully customizable.

## Project Setup

### Prerequisites:
- **AWS Account**: You must have an AWS account to deploy to AWS Lambda.
- **AWS CLI**: Ensure the AWS CLI is installed and configured with your AWS credentials.
- **AWS IAM Role**: Create an IAM role with the necessary permissions to allow AWS Lambda to access the services your application needs.
- **AWS Lambda Tools**: Install the AWS Lambda Tools for .NET. This can be done with the following command:
  
  ```bash
  dotnet tool install -g Amazon.Lambda.Tools
