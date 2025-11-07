#**🛒 E-Commerce SPA Deployment on AWS using AWS Amplify**

** Project Overview**

This project demonstrates how to deploy a Single Page Application (SPA) for an e-commerce platform using AWS Amplify. The static web file (index.html) is first uploaded to an Amazon S3 bucket, and then the website is hosted and managed using AWS Amplify for continuous deployment and scalability.

The goal of this project is to showcase a modern, serverless hosting workflow that enables developers to easily deploy, manage, and scale front-end applications with minimal operational overhead.

**Problem Statement**

Traditional web hosting environments require manual configuration, server management, and version control integration. For fast-growing e-commerce platforms, these challenges can lead to:

Deployment inefficiencies — manual uploads, frequent downtime during updates

Poor scalability — difficulty handling traffic spikes during sales or promotions

Limited automation — lack of CI/CD pipelines for continuous improvement

Security and reliability concerns — managing SSL certificates, version rollback, and monitoring manually

To solve these challenges, this project leverages AWS Amplify, which simplifies the hosting of SPAs with built-in CI/CD, global scalability, and zero-downtime deployments.

**⚙️ Project Architecture**
<img width="578" height="359" alt="image" src="https://github.com/user-attachments/assets/c61001d7-8616-498b-8c48-b3314a37d3d2" />


Frontend Development

Built as a Single Page Application (SPA) using HTML.

The main entry file is index.html.

Storage on S3

The static assets are uploaded to an Amazon S3 bucket configured for static website hosting.

S3 ensures durable, cost-effective storage for website assets.

Hosting with AWS Amplify

The S3 bucket is connected to AWS Amplify Hosting.

Amplify manages deployment, environment versions, and SSL automatically.

Enables CI/CD pipeline integration for future updates (e.g., via GitHub repo).

** Implementation Steps**
Step 1: Prepare the SPA Files

Build your e-commerce SPA with all assets (HTML,css,images).

Ensure the entry point is index.html.

Step 2: Create and Configure an S3 Bucket

Create an S3 bucket with a globally unique name.

Upload all SPA files into the bucket.
<img width="908" height="410" alt="image" src="https://github.com/user-attachments/assets/68e618e3-8971-4555-9e81-200c1e2e1259" />


Set appropriate permissions for Amplify to access content.

Step 3: Deploy via AWS Amplify


Open AWS Amplify Console.

Choose Host a Web App → Deploy without Git provider.

Connect your S3 bucket as the source.

Configure build settings and deploy.
<img width="917" height="412" alt="Screenshot 2025-11-07 120128" src="https://github.com/user-attachments/assets/0301dba1-53eb-4afc-bcd7-98bc65324b09" />

<img width="918" height="409" alt="Screenshot 2025-11-07 120045" src="https://github.com/user-attachments/assets/b8beddfd-5f8e-4870-ab82-a166dc8a7a2c" />

Step 4: Access and Test the Application

Amplify generates a unique domain URL (e.g., https://main.app.amplifyapp.com).
<img width="923" height="477" alt="Screenshot 2025-11-07 120219" src="https://github.com/user-attachments/assets/7b882a29-1b58-42e7-b886-722fb29cc819" />


Test responsiveness, navigation, and product pages.

Verify HTTPS, caching, and version rollback options.

**Benefits of Hosting on AWS Amplify**
**Benefit	Description**
Ease of Deployment	Simple workflow — upload files and deploy instantly.
Scalability	Built on AWS infrastructure, scales automatically with demand.
Continuous Deployment	Integrates with GitHub for automatic builds and updates.
Global Performance	Uses AWS CDN (CloudFront) for faster content delivery.
Security	Provides HTTPS and managed SSL certificates by default.
Version Control	Supports rollback to previous stable versions.
Cost Efficiency	Pay only for what you use; ideal for startups and small projects.


**Key Takeaways**

Hosting SPAs on AWS Amplify streamlines the deployment process.

Serverless hosting eliminates the need for backend server management.

S3 + Amplify provides a reliable, secure, and scalable platform for modern web apps.

 **Technologies Used**

AWS Amplify

Amazon S3

HTML / CSS 
