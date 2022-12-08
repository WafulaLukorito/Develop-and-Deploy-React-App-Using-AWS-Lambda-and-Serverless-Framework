# Develop and Deploy React App Using AWS Lambda and Serverless Framework

In this project, I developed a simple ToDo CRUD React app using AWS Lambda and Serverless Framework. The app also uses Auth0 for authentication and authorization. DynamoDB is used as the database.

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

