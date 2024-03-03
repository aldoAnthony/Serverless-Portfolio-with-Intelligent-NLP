<h1>Serverless Portfolio with Intelligent NLP Project</h1>

<h2>Description</h2>
For this project, I implemented a serverless data science portfolio website using AWS services and Python.

The website, hosted on AWS Amplify, was made to showcase various data science, machine learning, and AI projects.

The project also includes the development of an intelligent Natural Language Processing (NLP) service for automatic email responses based on visitor inquiries
<br />


<h2>Language and Libraries Used</h2>

- <b>CSS</b> 
- <b>Bootstrap</b>
- <b>JavaScript</b>
- <b>Python</b> 


<h2>Environments/Cloud Services Used </h2>

- <b>AWS IAM</b>
- <b>AWS Amplify</b>
- <b>Amazon DynamoDB</b>
- <b>Amazon API Gateway</b>
- <b>Amazon Comprehend</b>
- <b>Amazon Lambda</b>


<h2>Project Workflow:</h2>

- **Modify the Portfolio Webpage Template:** Customized a Bootstrap template to create a static website for personal data science and machine learning projects.

- **Serve Static Web Page on AWS Amplify:** Used AWS Amplify to serve the modified website in a serverless manner.
- **Create DynamoDB Database:** Set up an AWS DynamoDB NoSQL database to store visitor data, including name, email, phone number, and message.
- **Create IAM Role:**
  - Created an IAM role with policies for AWS Lambda, API Gateway, Comprehend, SES, and DynamoDB.
  - Ensured proper access and permissions for the Lambda function.
- **Set-up the Initial AWS Lambda Function and the AWS API Gateway Trigger:**
  - Created an AWS Lambda function with Python
  - Added a NumPy ARN layer to the Lambda function
  - Configured an AWS API Gateway trigger for the Lambda function to handle HTTP POST requests
- **AWS Lambda Function for Writing to DynamoDB:**
  - Set up Lambda function to write data received from the website form to DynamoDB
  - Used Python to decode and handle incoming data
- **AWS Lambda Function for Sending an Email with AWS SES:**
  - Configured AWS SES for email verification and sending automated responses
  - Integrated SES with Lambda to send emails based on specific triggers
- **AWS Lambda Function for Using Amazon Comprehend:**
  - Implemented NLP functionality using AWS Comprehend to extract sentiment and key phrases from messages
  - Was provided with helper functions for processing sentiment, key phrases, and generating intelligent email responses
