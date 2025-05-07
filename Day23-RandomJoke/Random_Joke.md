# Serverless Random Joke API

## Overview
This project creates a simple serverless API that returns a random joke when the endpoint is accessed. It uses AWS Lambda (with Python) and API Gateway.

## Components
- **Lambda Function:**  
  - Name: RandomJokeLambda  
  - Runtime: Python 3.8  
  - Code: Stores a list of jokes and picks one randomly.

- **API Gateway:**  
  - Provides a public REST API endpoint to invoke the Lambda function.

## Testing
- **GET Request to API Endpoint:**  
  I accessed `https://abc123.execute-api.us-east-1.amazonaws.com/default/RandomJokeLambda` and received:
  ```json
  {"joke": "Why did the bicycle fall over? Because it was two-tired!"}



3. **Save** the file once documented.

---

## **Part 6: Commit and Push Your Documentation**

1. **Open Your Terminal in the `Day23-RandomJoke` Folder.**

2. Run the following commands:
   ```bash
   git add Random_Joke.md
   git commit -m "Added Serverless Random Joke API project for Day 23"
   git push origin main
