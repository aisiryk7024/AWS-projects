# Serverless To-Do List API

## Overview
I built a serverless API that can add and retrieve to-do tasks. 
It uses AWS DynamoDB to store tasks, AWS Lambda to process requests, and API Gateway to expose the functionality to the internet.

## Steps I Followed

### 1. Set Up the Project Folder
- Created a new folder `Day17-DynamoServerless` in my AWS-Projects repository.
- Added a `ToDo_API.md` file for documentation.

### 2. Created a DynamoDB Table
- Table Name: `ToDoTable`
- Partition Key: `taskId` (String)

### 3. Created the Lambda Function (`ToDoLambda`)
- Wrote code in Python to:
  - **POST:** Add a new task to DynamoDB.
  - **GET:** Retrieve all tasks from DynamoDB.
- Deployed the Lambda function.

### 4. Configured API Gateway
- Added an API Gateway trigger to Lambda.
- API Endpoint: `[Your API endpoint URL]`

### 5. Testing the API
- **GET Request:** Verified by browsing to the endpoint.
- **POST Request:** Tested using cURL/Postman to add a new task.
- Confirmed that the new task appears in DynamoDB.

## What I Learned
- How to use **DynamoDB** to store data.
- How **Lambda** can process different HTTP methods.
- How **API Gateway** makes my function available over the web.

