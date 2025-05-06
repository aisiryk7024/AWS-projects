# Serverless Image Resizer

## Overview
This project automatically resizes images using AWS Lambda and S3. When an image is uploaded to the original images bucket, a Lambda function is triggered to create a thumbnail, which is saved under the "thumbnails/" folder in the same bucket.

## Steps Followed

### 1. S3 Buckets Setup
- Created an S3 bucket for original images.
- Decided to use the same bucket with a "thumbnails/" prefix for resized images.

### 2. Lambda Function Setup
- Created a Lambda function called `ImageResizerLambda` using Python 3.8.
- Added an S3 trigger (on PUT events) for the original images bucket.
- Wrote code to download, resize (thumbnail), and then re-upload the image.
- Deployed the function.

### 3. Testing
- Uploaded an image to the S3 bucket.
- Verified that a resized image appears in the "thumbnails/" folder.
- Checked CloudWatch logs for confirmation.

### 4. CloudWatch Monitoring
- (Optional) Set up a CloudWatch Alarm to monitor for errors in the Lambda function.

## Observations
- The thumbnail is created automatically and stored in the expected location.
- The system demonstrates a simple serverless image processing pipeline.
