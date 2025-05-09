# Serverless Log Analyzer and Alerting System

## Overview
This project creates a system that automatically analyzes log files uploaded to an S3 bucket. It counts the number of lines that contain "ERROR" and "WARNING" and returns a summary. (Optionally, you can extend the project to send alerts using SNS.)

## Components
- **S3 Bucket:** Used for uploading log files (bucket name: my-log-uploads-<unique-string>).
- **AWS Lambda Function:** (LogAnalyzerLambda) Downloads the log file, counts keywords, and returns a JSON summary.
- **S3 Event Trigger:** Configured to call the Lambda function on PUT events.

## Steps Followed
1. **S3 Setup:** Created an S3 bucket for log uploads.
2. **Lambda Creation:** Built and deployed a Python-based Lambda function.
3. **Trigger Configuration:** Added an S3 event trigger to invoke the function on file uploads.
4. **Testing:** Uploaded a sample log file and verified that the Lambda function outputs the expected summary.

## Observations
- The function correctly counted errors and warnings.
- Cleanup is crucial to avoid unwanted storage or function charges.

## Cleanup Recommendations
- **Delete the S3 Bucket:** Remove it (and its contents) through the S3 Console when testing is finished.
- **Delete the Lambda Function:** Delete or disable the function if it’s no longer needed.
