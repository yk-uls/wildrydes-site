# wildrydes-site

## Build a Serverless Web Application ##

This Project was created using AWS Lambda, Amazon API Gateway, Amazon S3, Amazon DynamoDB, and Amazon Cognito.

![image](https://user-images.githubusercontent.com/68623425/222940777-7545cc3d-b48d-4e70-acbe-03862b0407c1.png)

Access the application: https://main.d3hz1t8ikrz344.amplifyapp.com/

Serverless web application that allows users to request rides on a unicorn from the Wild Rydes fleet. The app features an HTML-based UI to indicate where users would like to be picked up and interacts on the back end with a RESTful web service to submit the request and dispatch a nearby unicorn. The application also offers facilities for users to register for the service and log in before requesting rides.

The application architecture uses AWS Lambda, Amazon API Gateway, Amazon DynamoDB, Amazon Cognito, and the AWS Amplify console. The Amplify console provides deployment and hosting of static web resources including HTML, CSS, JavaScript and image files that are loaded in the user's browser. JavaScript running in the browser sends and receives data from a public backend API built using Lambda and API Gateway. Amazon Cognito provides authentication and user management functions to secure the backend API. Finally, Amazon DynamoDB provides a persistence layer where data can be stored by the API's Lambda function.

![image](https://user-images.githubusercontent.com/68623425/221295676-054ada90-a105-4a6b-b722-524ad90c0c0d.png)

## Overview ##
The workshop solution uses the following AWS services:
* AWS Amplify - simplify application lifecycle, including builds and deploys the web application by following a continuous integration and delivery model.
* Amazon Cognito - lets you add user sign-up, sign-in, and access control to your web and mobile apps quickly and easily.  In this solution, it's used to manage users, federate identities, and manage user pools.
* AWS Lambda - provide backend process for handling requests from your web application, i.e. function that is invoked whebver a user requests a unicorn to be sent to a location of his/er choice.  The function will select a unicorn from the fleet, record the request in a DynamoDB table and then respond to the front-end application with details about the unicorn being dispatched.
* Amazon API Gateway - makes it easy for developers to create, maintain, and secure APIs.  It's used to expose the Lambda function built as a RESTful API.
* Amazon S3 - object storage for hosting static web site content (HTML, CSS, JavaScript, images and other files).
* Amazon DynamoDB - NoSQL database service used to provide a table to record the unicorn requests in a DynamoDB table.

  
