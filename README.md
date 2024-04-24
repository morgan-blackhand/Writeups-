# Deploying a RESTful API

## Introduction
In this lab, we'll deploy a RESTful API. The initial step involves creating a Lambda function.

## Step 1: Create and Test Lambda Function
https://imgur.com/rTLDRvp.png
  - Code the Lambda function.

https://imgur.com/oeesJ6p
- Test the event to see if the script will work in a real environment.
  - Make slight adjustments to handle more events.

https://imgur.com/cy3bwX2.png

## Step 2: Setup API Gateway

https://imgur.com/a/jCCWa6I
- Start creating an API Gateway.

https://imgur.com/s6Iikc7.png
- Add resources to the API.
  - Create methods (ID and GET) for the API to interact with Lambda.

https://imgur.com/a/15JBojj            

## Deployment
Deploy the API to the environment. Note any discrepancies in expected outcomes. For example, receiving "Hello from Lambda" as a response instead of the expected animal number and name suggests a need for code debugging.

## Challenges and Learning Points

https://imgur.com/a/Ei5yoKz
- Initially received "Hello from Lambda" due to path issues in JSON and Python scripts, indicating the need for correct path configurations.

https://imgur.com/AMHN3Jm.png
- Always deploy changes to ensure the code updates are applied; failure to do so can lead to unexpected defaults and bugs.

https://imgur.com/OBVedWj.png

## Conclusion
This lab was conducted under the constraints of AWS Cloud Quest, limited to only 2 hours, which posed significant challenges in debugging and finalizing the API.

## Disclaimer
Due to time constraints in the lab environment, the full debugging process could not be completed, affecting the final outcomes. The core idea of implementing an API connected with Lambda was successfully demonstrated.

