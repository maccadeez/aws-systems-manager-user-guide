# Tutorials<a name="automation-tutorials"></a>

The following tutorials help you to use AWS Systems Manager Automation to address common use cases\. These tutorials demonstrate how to use your own runbooks, predefined runbooks provided by Automation, and other Systems Manager capabilities with other AWS services\.

**Contents**
+ [Updating AMIs](automation-tutorial-update-ami.md)
  + [Update a Linux AMI](automation-tutorial-update-patch-linux-ami.md)
  + [Update a Linux AMI \(AWS CLI\)](automation-tutorial-update-ami.md#update-patch-linux-ami-cli)
  + [Update a Windows Server AMI](automation-tutorial-update-patch-windows-ami.md)
  + [Update a golden AMI using Automation, AWS Lambda, and Parameter Store](automation-tutorial-update-patch-golden-ami.md)
    + [Task 1: Create a parameter in Systems Manager Parameter Store](automation-tutorial-update-patch-golden-ami.md#create-parameter-ami)
    + [Task 2: Create an IAM role for AWS Lambda](automation-tutorial-update-patch-golden-ami.md#create-lambda-role)
    + [Task 3: Create an AWS Lambda function](automation-tutorial-update-patch-golden-ami.md#create-lambda-function)
    + [Task 4: Create a runbook and patch the AMI](automation-tutorial-update-patch-golden-ami.md#create-custom-ami-update-runbook)
  + [Updating AMIs using Automation and Jenkins](automation-tutorial-update-patch-ami-jenkins-integration.md)
  + [Updating AMIs for Auto Scaling groups](automation-tutorial-update-patch-windows-ami-autoscaling.md)
    + [Create the **PatchAMIAndUpdateASG** runbook](automation-tutorial-update-patch-windows-ami-autoscaling.md#create-autoscaling-update-runbook)
+ [Using AWS Support self\-service runbooks](automation-tutorial-support-runbooks.md)
  + [Run the EC2Rescue tool on unreachable instances](automation-ec2rescue.md)
    + [How it works](automation-ec2rescue.md#automation-ec2rescue-how)
    + [Before you begin](automation-ec2rescue.md#automation-ec2rescue-begin)
      + [Granting `AWSSupport-EC2Rescue` permissions to perform actions on your instances](automation-ec2rescue.md#automation-ec2rescue-access)
        + [Granting permissions by using IAM policies](automation-ec2rescue.md#automation-ec2rescue-access-iam)
        + [Granting permissions by using an AWS CloudFormation template](automation-ec2rescue.md#automation-ec2rescue-access-cfn)
    + [Running the Automation](automation-ec2rescue.md#automation-ec2rescue-executing)
  + [Reset passwords and SSH keys on EC2 instances](automation-ec2reset.md)
    + [How it works](automation-ec2reset.md#automation-ec2reset-how)
    + [Before you begin](automation-ec2reset.md#automation-ec2reset-begin)
      + [Granting AWSSupport\-EC2Rescue permissions to perform actions on your instances](automation-ec2reset.md#automation-ec2reset-access)
        + [Granting permissions by using IAM policies](automation-ec2reset.md#automation-ec2reset-access-iam)
        + [Granting permissions by using an AWS CloudFormation template](automation-ec2reset.md#automation-ec2reset-access-cfn)
    + [Running the Automation](automation-ec2reset.md#automation-ec2reset-executing)
+ [Passing data to Automation using input transformers](automation-tutorial-eventbridge-input-transformers.md)