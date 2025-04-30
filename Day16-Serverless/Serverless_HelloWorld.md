"# Serverless Hello World!" 

# Serverless “Hello, World!” API

## Overview
Today, I built a simple serverless API using AWS Lambda and API Gateway. When someone visits my API URL, it shows "Hello, World!".

## Steps I Followed:

1. **Set Up Project Folder:**
   - Created a folder called `Day16-Serverless` inside my AWS-Projects repo.
   - Made a markdown file called `Serverless_HelloWorld.md` to note everything.

2. **Created a Lambda Function:**
   - Went to AWS Lambda, clicked "Create function."
   - Named it `HelloWorldLambda` and used Python 3.8.
   - Added simple code so it always returns "Hello, World!".

3. **Connected an API Gateway:**
   - Added an API Gateway trigger to the Lambda.
   - Chose a REST API that is Open so anyone can access it.
   - Got an API endpoint URL.

4. **Tested the API:**
   - Pasted the API URL in my web browser.
   - Saw the message "Hello, World!" — it worked!

## What I Learned:
- AWS Lambda and API Gateway let you build apps without having to worry about servers.
- Serverless means you don’t manage any physical or virtual servers.
- It’s fun and simple to test your code right in your browser!

## Observations:
- The response is instant.
- The whole process is like setting up a magic machine that talks back to you!
