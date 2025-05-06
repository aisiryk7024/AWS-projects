# Serverless URL Shortener API

## Overview
This project creates a serverless API that shortens long URLs. Users can send a POST request with a long URL to receive a unique short code, and later use a GET request with that short code to retrieve the original URL.

## Components
- **DynamoDB Table:** URLShortenerTable with `short_code` as the partition key.
- **Lambda Function:** URLShortenerLambda written in Python.
- **API Gateway:** Exposes the Lambda function via a REST API.

## Testing
- **POST Example:**  
  Submitted long URL "https://www.example.com/your-long-url" and received `{"short_code": "aB3dE4", "long_url": "https://www.example.com/your-long-url"}`.
- **GET Example:**  
  Retrieved the long URL using the short code.

## Observations & Learnings
- I learned how to generate random strings in Python.
- The integration of Lambda, API Gateway, and DynamoDB makes a powerful, serverless architecture.
