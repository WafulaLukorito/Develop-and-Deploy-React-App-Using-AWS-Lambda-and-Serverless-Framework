# Develop and Deploy React App Using AWS Lambda and Serverless Framework

In this project, I developed a simple ToDo CRUD React app using AWS Lambda and Serverless Framework. The app also uses Auth0 for authentication and authorization. DynamoDB is used as the database.

## Frontend
React app is developed using `create-react-app` and `Typescript`. `Auth0` is used for authentication and authorization and allows for login using Google accounts.

Welcome page before login:

![Welcome page before login](https://github.com/WafulaLukorito/Revised-Develop-and-Deploy-Web-Application-using-AWS-Lambda-and-Serverless-Framework/blob/master/Screenshots/Welcome%20page%20before%20login.png?raw=true "Welcome page before login")

Auth0 authorisation page and prompt for login using Google account:

![Auth0 authorisation page and prompt for login using Google account](https://github.com/WafulaLukorito/Revised-Develop-and-Deploy-Web-Application-using-AWS-Lambda-and-Serverless-Framework/blob/master/Screenshots/AuthO%20login%20Authorization%20and%20prompt.png?raw=true "Auth0 authorisation page and prompt for login using Google account")

App running successfully:

![App running successfully](https://github.com/WafulaLukorito/Revised-Develop-and-Deploy-Web-Application-using-AWS-Lambda-and-Serverless-Framework/blob/master/Screenshots/App%20running%20successfully%20.png?raw=true "App running successfully")

## Backend

The backend entails:

- A custom authorizer for API gateway (`Auth0 JWT`)
- `IamRoleStatements` configured for CRUD operations on `DynamoDB`
- A presigned URL for uploading attachment files to `S3 bucket`.
- `CORS configuration` for the API gateway functions.
- `DynamoDB` table for storing `ToDo` items.

### Best Practices Included

- Validation of incoming HTTP requests using the `serverless-reqvalidator-plugin`.
- Generation of application-level `metrics` for monitoring.
- `Logging` of application-level events with a `Winston` logger for JSON-formatted logs.
- `Distributed tracing` using `AWS X-Ray`.
- A `Postman` collection for testing the API is included.
