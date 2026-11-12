CloudCart – AWS E-Commerce Website Hosting with CI/CD

Project Overview
CloudCart is a static e-commerce website hosted on AWS using Amazon S3 and CloudFront. Jenkins automates the deployment process through a CI/CD pipeline integrated with GitHub.

 Technologies Used
- AWS S3
- AWS CloudFront
- AWS IAM
- AWS CloudWatch
- AWS SNS
- Jenkins
- Git and GitHub
- Linux (Ubuntu WSL 2)
- AWS CLI
- HTML, CSS and JavaScript

Architecture

GitHub → Jenkins → AWS S3 → CloudFront → End Users

CloudWatch monitors CloudFront traffic and errors. SNS provides email notifications through a CloudWatch alarm.

 Project Features
- Static e-commerce website with product listings.
- Private S3 bucket for website storage.
- CloudFront distribution for HTTPS content delivery.
- Automated deployment using Jenkins.
- CloudFront cache invalidation after deployment.
- IAM-based access control for Jenkins.
- CloudWatch dashboard for traffic and error monitoring.
- CloudWatch alarm with SNS email notification.

CI/CD Pipeline Stages
1. Checkout source code from GitHub.
2. Verify website files.
3. Deploy website files to S3 using AWS CLI.
4. Invalidate CloudFront cache.
5. Report pipeline success or failure.

AWS Configuration
- S3 Region: ap-south-1
- S3 Bucket: cloudcart-website-22
- CloudFront Distribution ID: E2M55RQUAVVJAG
- CloudWatch Dashboard: CloudCart-Monitoring

Learning Outcomes
- Practical experience with AWS cloud hosting.
- Configuring private S3 and CloudFront OAC.
- Creating IAM policies and Jenkins credentials.
- Implementing automated CI/CD pipelines.
- Deploying applications using AWS CLI.
- Monitoring cloud infrastructure using CloudWatch and SNS.

 Project Status
Successfully deployed and tested using Jenkins CI/CD.

Author
Tanuj