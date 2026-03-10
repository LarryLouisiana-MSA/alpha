this is a prototype for POC purposes
Key Features of This Solution
Feature	Implementation
Event Triggering	S3 bucket notifications trigger Lambda on object creation
File Name Extraction	Extracts just the filename from S3 key path
Message Format	Sends structured JSON with metadata to SQS
Error Handling	Includes try-catch blocks and detailed logging
DLQ Support	Failed messages sent to Dead Letter Queue after 3 retries
IAM Security	Least privilege permissions per AWS best practices
Monitoring	CloudWatch logs, metrics, and alarms for errors
Scalability	Configurable memory, timeout, and long polling
Infrastructure as Code	Complete Terraform automation
