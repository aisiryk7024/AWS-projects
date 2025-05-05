# Serverless Notification Service

## Overview
This project sets up a simple serverless service that sends an email notification when its API endpoint is called. It uses:
- **AWS Lambda** to run code that publishes a message.
- **Amazon SNS** to send an email notification.
- **API Gateway** to provide a web URL trigger.
- **CloudWatch** to monitor the Lambda errors.

## Steps Followed

### 1. SNS Topic Creation
- Created a topic named `NotificationServiceTopic`.
- Subscribed my email and confirmed the subscription.

### 2. Lambda Function Setup
- Created a function called `NotificationLambda` using Python 3.8.
- The code publishes a message to the SNS topic when triggered.
- Deployed the function.

### 3. API Gateway Trigger
- Added an API Gateway trigger to the Lambda function (REST API, Open access).
- Received an API endpoint URL.

### 4. Testing
- Tested the endpoint by opening it in a browser.
- Confirmed that an email notification was received.

### 5. CloudWatch Monitoring
- Set up a CloudWatch alarm on the Lambda function’s Error metric.
- Configured the alarm to send notifications via SNS if any errors occur.

## Observations
- The entire system is serverless and costs only what you use.
- It is a neat way to set up notifications without managing any servers.
