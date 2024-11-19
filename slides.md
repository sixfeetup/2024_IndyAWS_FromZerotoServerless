---
title-prefix: Six Feet Up
pagetitle: From Zero to Serverless
author: Calvin Hendryx-Parker, CTO, Six Feet Up
author-meta:
    - Calvin Hendryx-Parker
date: IndyAWS 2024
date-meta: 2024
keywords:
    - AWS
    - Cloud
    - Serverless
    - Python
---

# From Zero to Serverless: 
### Building a Real-Time Leaderboard with AWS SAM
#### Calvin Hendryx-Parker, CTO
#### Six Feet Up

---

# Why AWS SAM?
## Simplifying Serverless Development

![](images/AWS_SAM_Mascot.png){.r-stretch}

---

# What is AWS SAM?

- **S**erverless **A**pplication **M**odel
- Open-source framework for building serverless applications
- Extension of AWS CloudFormation
- Provides simplified syntax for defining serverless resources

---

# Key Benefits of AWS SAM

---

# **Developer Productivity**
   - Write less boilerplate
   - Built-in best practices
   - Local testing and debugging

---

# **Infrastructure as Code**
   - Version control your infrastructure
   - Consistent deployments
   - Easy rollbacks
 
---

# **Local Development**
   - Test Lambda functions locally
   - Simulate API Gateway endpoints
   - Debug step-by-step

---

# Real World Use Cases

- **API Development**
  - REST APIs with Lambda + API Gateway
  - Simplified API definitions

---

# Real World Use Cases (cont.)

- **Event Processing**
  - S3 event handlers
  - SQS/SNS processors
  - CloudWatch Events

---

# Real World Use Cases (cont.)

- **Web Applications**
  - Serverless backends
  - Static website hosting
  - Authentication flows

---

# SAM vs Raw CloudFormation

```yaml{.stretch}
# Traditional CloudFormation
Resources:
  MyFunction:
    Type: AWS::Lambda::Function
    Properties:
      Handler: index.handler
      Role: !GetAtt LambdaExecutionRole.Arn
      Code:
        S3Bucket: my-bucket
        S3Key: my-function.zip
      Runtime: nodejs18.x

# SAM Equivalent
Resources:
  MyFunction:
    Type: AWS::Serverless::Function
    Properties:
      Handler: index.handler
      Runtime: nodejs18.x
```

---

# Getting Started

1. **Install SAM CLI**
   ```bash
   brew install aws-sam-cli
   ```

2. **Initialize a Project**
   ```bash
   sam init
   ```

3. **Local Development**
   ```bash
   sam local start-api
   ```

4. **Deploy**
   ```bash
   sam deploy --guided
   ```
   
---

# Hello World{.r-fit-text}

---

# Why Choose SAM?

✅ **Simplified Resource Definitions**  
✅ **Local Testing Capabilities**  
✅ **AWS Best Practices Built-in**  
✅ **Free and Open Source**  
✅ **Native AWS Integration**  
✅ **Active Community**  

---

# Scaf Leaderboard Example

![](images/ScafLeaderboardDiagram.png){.r-stretch}

---

# Resources

* [SAM Docs](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/)
* [NoSQL Workbench](https://aws.amazon.com/dynamodb/nosql-workbench/)
* [Postman](https://getpostman.com)

---

# Talk To Me

📩 <calvin@sixfeetup.com>  
🤝 <https://linkedin.com/in/calvinhp>  
✖️ [@calvinhp](https://x.com/calvinhp)  
🐘 [@calvinhp@fosstodon.org](https://fosstodon.org/@calvinhp)  
🦋 [@calvinhp.com](https://bsky.app/profile/calvinhp.com)
