# Hosting an Angular Application on Amazon S3

## Objective
Host a static Angular frontend application using Amazon S3 Static Website Hosting.

## Technologies Used
- Angular
- Amazon S3
- AWS CLI

## Steps Performed
1. Built the Angular application using:
   ```bash
   ng build
   ```
2. Created an S3 bucket.
3. Enabled Static Website Hosting.
4. Disabled Block Public Access.
5. Added a bucket policy to allow public read access.
6. Uploaded the build files from the `dist/angular-app` directory.
7. Accessed the application using the S3 Website Endpoint.

## Outcome
The Angular application was successfully deployed and is accessible through the Amazon S3 Static Website Endpoint.