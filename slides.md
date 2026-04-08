---
title: Lets talk about ... SAM
---

---
build: true

## Lets talk about ...
# SAM

---

## Lets talk about
# Serverless

---

## Lets talk about
# Application

---

## Lets talk about
# Model

---

## Serverless - What?
build: true

- Cloud provider manages the allocation of machine resources
- User just provides Code
- Serverless runtimes
- &nbsp;

---

## Serverless - What?
- Cloud provider manages the allocation of machine resources
- User just provides Code/Schema
- Serverless runtimes
- Serverless databases

---

## Serverless - Why?
- No Servers to manage/update
- No idle times which need to be paid
- (Linear) scales with usage
- Load balancing, Networking, Fault tolerance build in

---

## Serverless - Where?
- Web Applications (eg. Express)
- Backends (eg. API with LoopBack)
- Data Processing (Background jobs, Tasks)
- Bots (eg. Chatbots)
- Automation (Extending AWS Services)

---

## Serverless - Where?
- Web Applications (eg. Express)
- Backends (eg. API with LoopBack)
- Data Processing (Background jobs, Tasks)
- Bots (eg. Chatbots)
- **Automation (Extending AWS Services)**

---

## AWS Services - Data
- S3
- DynamoDB
- Kinesis
- Aurora (MySQL)

---

## AWS Services - Management
- CloudFormation
- CloudTrail
- CodeCommit
- CloudWatch

---

## AWS Services - Endpoints
- API Gateway
- IoT
- Step Functions

---

## AWS Services - Messages
- SES
- SNS
- Cron

---

## Lambda - What is needed?
- Role
- Policy
- S3
- Lambda
- API Gateway

---

## Lambda - What is needed?
- Role
- Policy
- S3
- Lambda
- **API Gateway**

---

## API Gateway - What is needed?
- API
- Permission
- S3
- Stage
- Mapping

---

## CloudFormation
- Templates for AWS Infrastructure
- Parameters -> Resources -> Output
- Version Control, Change Sets
- A bit like docker compose
- json/yaml

---

## CloudFormation issues
- Lambda needs code within S3
- API Gateway needs Swagger File within S3

---

## CloudFormation solution
- Small initial Stack including S3
- Upload files
- Apply ChangeSet with Lambda and API Gateway
- **or**
- package (needs S3 again)

---
type: section

# SAM

---

## SAM - What?
- CloudFormation extension
- Adds new Resource types
- CLI

---

## SAM - New Types
- AWS::Serverless::Api
- AWS::Serverless::SimpleTable
- AWS::Serverless::Function

---

## SAM - New Types
- AWS::Serverless::Api
- AWS::Serverless::SimpleTable
- **AWS::Serverless::Function**

---

## AWS::Serverless::Function
- Role
- Permission
- S3
- Lambda
- Events

---

## AWS::Serverless::Function
- Role
- Permission
- S3
- Lambda
- **Events**

---

## Event Sources
- S3
- SNS
- Kinesis
- DynamoDB
- Schedule

---

## CLI
- init
- validate
- package
- deploy
- local

---

## CLI
- init
- validate
- package
- deploy
- **local**

---

## SAM - Local
- generate-event
- invoke
- start-api

---

# Demo

---
background: assets/images/all-the-things.jpg

# &nbsp;
# Thats it

---

## Whats next?
- [CloudFormation Resources](https://docs.aws.amazon.com/en_us/AWSCloudFormation/latest/UserGuide/aws-template-resource-type-ref.html)
- [SAM GitHub Repo](https://github.com/awslabs/serverless-application-model)
- [SAM CLI GitHub Repo](https://github.com/awslabs/aws-sam-cli)
- [Slides GitHub Repo](https://github.com/tamino-martinius/lets-talk-about--sam)

---
type: section

# Questions?
