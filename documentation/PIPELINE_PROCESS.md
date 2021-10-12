# Pipeline process diagram

---

## 1. Orbs:
The first step in the pipeline is adding the orbs, namely:
    - node: `circleci/node@4.1.0`
    - aws-cli: `circleci/aws-cli@1.3.1`

## 2. Install the docker base image:
This image can run most needed actions with orbs.

## 3. Setup CLI & Install deployment dependencies:
Setup `aws cli` and the `eb cli`. 

## 4. Install dependencies:
Install both **Front-end** & **Back-end** dependencies.

## 5. Linting:
Run the lint commands for both **Front-end** & **Back-end** applications.

## 6. Unit Testing:
Execute the unit testing scripts for both **Front-end** & **Back-end**.

## 7. Build:
Run the build scripts for **Front-end**.

## 8. Deploy to S3:
Deploy built Front-end code to S3 bucket.

## 9. Deploy to Elastic Beanstalk:
Deploy the **Back-end** to Elastic Beanstalk.

