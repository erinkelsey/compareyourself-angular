# CompareYourself

Simple app to compare your details to others, using AngularJS and a serverless backend with AWS Lambda, API Gateway, Cognito, DynamoDB, S3, Route53 and CloudFront.

S3 Location: http://compare-yourself-angular-serverless.s3-website.ca-central-1.amazonaws.com/

CloudFront Location: https://d2jzkhwp9umnvw.cloudfront.net

Route 53 Domain: https://compare-yourself.eksdevelopment.ca

# Features

Auth:

- Sign up -> receive email confirmation from AWS Cognito
- Confirm email
- Sign in

Details:

- Add your personal details -> saved in DynamoDB
- Retrieve your personal details
- Compare your personal details with all others
- Delete your personal details

# Install

Install Dependencies:

    node install

# Setup

TODO: include Lambda code, Cognito setup instructions, API Gateway setup instructions

Create environment variables:

- Add an environments folder in src/
- Add a environment.ts (and environment.prod.ts) file
- Example file:

          export const environment = {
            production: false,
            userPoolId: "YOUR_COGNITO_USER_POOL_ID",
            clientId: "YOUR_COGNITO_CLIENT_ID",
            apiUrl:
            "YOUR_API_GATEWAY_BASE_URL",
          };
