# Working with Amazon ECS in Application Manager<a name="application-manager-working-ECS"></a>

With Application Manager, a capability of AWS Systems Manager, you can view and manage your Amazon Elastic Container Service \(Amazon ECS\) cluster infrastructure\. Application Manager provides a component runtime view of the compute, networking, and storage resources in a cluster\.

**Note**  
You can't manage or view operations information about your containers in Application Manager\. You can only manage and view operations information about the infrastructure hosting your Amazon ECS resources\.

**Actions you can perform on this page**  
You can perform the following actions on this page:
+ Choose **Manage cluster** to open the cluster in Amazon ECS\.
+ Choose **View all** to view a list of resources in your cluster\.
+ Choose **View in CloudWatch** to view resource alarms in Amazon CloudWatch\.
+ Choose **Manage nodes** or **Manage Fargate profiles** to view these resources in Amazon ECS\.
+ Choose a resource ID to view detailed information about it in the console where it was created\.
+ View a list of OpsItems related to your clusters\.
+ View a history of runbooks that have been run on your clusters\.

**To open an **ECS cluster****

1. Open the AWS Systems Manager console at [https://console\.aws\.amazon\.com/systems\-manager/](https://console.aws.amazon.com/systems-manager/)\.

1. In the navigation pane, choose **Application Manager**\.

1. In the **Container clusters** section, choose **ECS clusters**\.

1. Choose a cluster in the list\. Application Manager opens the **Overview** tab\.