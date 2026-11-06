# AWS Project 1: Secure Static Website Hosting

## Project Overview

This project demonstrates how to deploy a static portfolio website using Amazon S3 and Amazon CloudFront, following AWS security best practices.

The website is delivered securely over HTTPS, while the S3 bucket remains private.

## Architecture

Visitor → HTTPS → Amazon CloudFront → Origin Access Control (OAC) → Private Amazon S3 Bucket

## AWS Services Used

- **Amazon S3:** Stores the HTML, CSS and JavaScript files.
- **Amazon CloudFront:** Delivers website content through a content delivery network.
- **Origin Access Control (OAC):** Restricts access to the S3 origin through CloudFront.
- **AWS IAM:** Controls permissions for managing AWS resources.
- **AWS CloudShell:** Provides a command-line environment for deployment and management.

## Security Implementation

- Enabled S3 Block Public Access.
- Configured a private S3 bucket.
- Used CloudFront Origin Access Control.
- Restricted S3 access through a CloudFront-specific bucket policy.
- Enabled HTTPS access through CloudFront.
- Verified that direct public access to S3 objects was blocked.

## Deployment Process

1. Created the portfolio website using HTML, CSS and JavaScript.
2. Created a private Amazon S3 bucket.
3. Uploaded website files using AWS CLI.
4. Created an Amazon CloudFront distribution.
5. Configured Origin Access Control.
6. Applied a restrictive S3 bucket policy.
7. Tested website accessibility and security.
8. Documented the project using Git and GitHub.

## Skills Demonstrated

- AWS cloud storage
- Content delivery networks
- AWS CLI
- Cloud security
- IAM permissions
- Git and GitHub
- Linux command-line operations

## Lessons Learned

This project strengthened my understanding of secure cloud hosting, access management, troubleshooting AWS CLI commands and deploying websites through CloudFront.

## Future Improvements

- Introduce Infrastructure as Code using Terraform.
- Automate deployments through GitHub Actions.
- Configure custom domain support.
- Add monitoring and alerting.

## Project Verification

The deployment was tested against the following security requirements:

- The website loads successfully through its CloudFront distribution.
- HTTPS is used to deliver website content.
- The S3 bucket is not publicly accessible.
- S3 Block Public Access is enabled.
- CloudFront Origin Access Control (OAC) is configured.
- The S3 bucket policy restricts object access to the authorised CloudFront distribution.

## Project Outcome

Successfully deployed a secure static portfolio website using Amazon S3 and CloudFront. This project provided practical experience with AWS CLI, cloud storage, content delivery, IAM, access control, Linux and Git version control.

## Cost Management

The project uses a lightweight static website architecture. AWS usage and billing should be monitored regularly, including S3 storage and requests, CloudFront requests and data transfer.

## Repository Structure

- `index.html` — Website content
- `style.css` — Website styling
- `script.js` — JavaScript functionality
- `README.md` — Project documentation
- `PROJECT_NOTES.md` — Additional project notes
- `.gitignore` — Files excluded from version control
