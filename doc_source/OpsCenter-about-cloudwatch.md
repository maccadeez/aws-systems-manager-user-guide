# CloudWatch<a name="OpsCenter-about-cloudwatch"></a>

 Amazon CloudWatch monitors your AWS resources and services, and displays metrics on every AWS service that you use\. CloudWatch creates an OpsItem when an alarm enters the alarm state\. For example, you can configure an alarm to automatically create an OpsItem if there is a spike in HTTP errors generated by your Application Load Balancer\.

Some alarms that you can configure in CloudWatch to create OpsItems are shown in the following list: 
+ Amazon DynamoDB: database read and write actions reach a threshold
+ Amazon EC2: CPU utilization reaches a threshold
+ AWS billing: estimated charges reach a threshold
+ Amazon EC2: an instance fails a status check
+ Amazon Elastic Block Store \(EBS\): disk space utilization reaches a threshold

You can either create an alarm or edit an existing alarm to create an OpsItem\. For more information, see [Configure CloudWatch alarms to create OpsItems](OpsCenter-create-OpsItems-from-CloudWatch-Alarms.md)\.

When you enable OpsCenter using Integrated Setup, it integrates CloudWatch with OpsCenter\. 