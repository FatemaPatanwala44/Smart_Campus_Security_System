# Smart_Campus_Security_System
A serverless AWS-based security system that automatically identifies authorized individuals using face recognition and alerts security teams in real time when unknown persons are detected.
# Smart Campus Security System (AWS)

## Overview
This project is a serverless Smart Campus Security System built using AWS services.
It automatically identifies authorized and unauthorized individuals entering a campus
using face recognition technology.

## Problem Statement
Manual security checks are time-consuming and error-prone.
This system automates entry verification and improves campus safety.

## Technologies Used
- AWS Lambda
- Amazon S3
- Amazon Rekognition
- Amazon SNS
- Amazon DynamoDB
- AWS IAM
- Amazon CloudWatch

## Working
1. Face image is captured at the campus entry point.
2. Image is uploaded to an S3 bucket.
3. S3 triggers AWS Lambda automatically.
4. Lambda sends the image to Amazon Rekognition for face matching.
5. If the face is recognized, the entry is logged.
6. If the face is unknown, an alert is sent via SNS and the image is stored separately.

## Cloud Model
- Platform as a Service (PaaS)
- Serverless Architecture

## Future Scope
- Integration with IoT-based CCTV cameras
- Real-time video processing
- Admin dashboard for monitoring and analytics

## Note
This project is implemented using AWS Free Tier for learning and demonstration purposes.
