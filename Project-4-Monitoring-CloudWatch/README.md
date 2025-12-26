# Monitoring and Alerting using Amazon CloudWatch

## Problem Statement
Production systems require monitoring to detect failures and performance issues.

## Solution
Implemented Amazon CloudWatch logging, metrics, and alarms to monitor AWS Lambda execution.

## Architecture
AWS Lambda → CloudWatch Logs → CloudWatch Alarms → SNS Notification

## AWS Services Used
- Amazon CloudWatch
- AWS Lambda
- Amazon SNS

## Deployment Steps
1. Viewed Lambda execution logs in CloudWatch
2. Configured error metrics
3. Created CloudWatch alarms
4. Set up SNS email notifications

## Outcome
- Real-time monitoring enabled
- Error detection and alerting implemented
- Production-grade observability added to serverless application

## Architecture Diagram

```mermaid
flowchart TD
    Lambda[AWS Lambda Function]
    Logs[Amazon CloudWatch Logs]
    Alarm[CloudWatch Alarm]
    SNS[Amazon SNS Email Notification]

    Lambda -->|Execution Logs| Logs
    Logs -->|Error Metrics| Alarm
    Alarm -->|Alert| SNS
```

## Screenshots

### Lambda Execution Logs
![CloudWatch Lambda Logs](screenshots/cloudwatch-lambda-logs.png)

### CloudWatch Alarm
![CloudWatch Alarm](screenshots/cloudwatch-alarm.png)
