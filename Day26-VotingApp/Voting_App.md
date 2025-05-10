# Serverless Voting Application

## Overview
This project creates a simple REST API for a voting application using AWS Lambda, API Gateway, and DynamoDB. Users can cast a vote (POST) or retrieve the vote counts (GET).

## Components
- **DynamoDB Table:** VotingTable with partition key `candidate`
- **Lambda Function:** VotingLambda (Python) that processes votes and retrieves results
- **API Gateway:** Exposes the Lambda function via a REST API endpoint

## Steps Followed
1. Created the DynamoDB table "VotingTable".
2. Developed and deployed the VotingLambda function with POST and GET handlers.
3. Adjusted the Lambda execution role to include DynamoDB permissions.
4. Configured API Gateway to trigger the Lambda function.
5. Tested the application using cURL/Postman:
   - **POST response:** Confirmed a vote was cast for a candidate.
   - **GET response:** Returned the latest vote counts.

## Observations
- The function correctly handles atomic updates in DynamoDB.
- API integration is smooth via API Gateway.
- Ensuring IAM and resource configurations are set up prevents unexpected issues.

## Cleanup Recommendations
- Delete the API Gateway if not needed.
- Remove the Lambda function and DynamoDB table if you do not intend to use the application further.
