# Sincronización Externa de Data Lake (AWS)

The integration between Event Stores and AWS allows the seamless transfer of event data to an S3 bucket, ensuring efficient data archiving, backup, and accessibility. Exporting your data to an external data lake brings you more control over your data, leading you to valuable insights.

{% hint style="warning" %}
Before starting, ensure you have AWS Management Console access with permissions to manage Virtual Private Clouds(VPC), Security Groups, Lambda functions, and IAM roles. Also, consider that this procedure may incur additional costs in your AWS account due to the creation and usage of new resources.
{% endhint %}

## Deploying Infrastructure with AWS CloudFormation

Two templates have been developed using CloudFormation to streamline the integration setup and provide the minimum required infrastructure. Depending on your technical knowledge, you can customize these templates after their initial setup to fit your business needs.

{% hint style="info" %}
To proceed you need an API Key created with read-only permissions for event stores. You can learn to create and retrieve an API Key in this [article](../product-documentation/gestion-de-acceso-e-identidad-iam/api-keys.md).
{% endhint %}

### Template with VPC

Use this template if a Virtual Private Cloud (VPC) is already configured in your AWS account. Access the template [here](https://us-east-2.console.aws.amazon.com/cloudformation/home?region=us-east-2#/stacks/quickcreate?templateUrl=https://bms--public-files.s3.us-east-1.amazonaws.com/with-vpc.yaml\&stackName=bms%E2%80%93monitoring%E2%80%93event-pipe%E2%80%93event-recorder).

<figure><img src="../.gitbook/assets/image (1037).png" alt=""><figcaption><p>Template with VPC</p></figcaption></figure>

After accessing the template, fill in the details:

* Stack Name: This field is automatically filled, but you can use it to customize the stack name.
* S3 Bucket Name: Inform or create a name for your S3 Bucket.
* Create S3 Bucket: Choose 'true' to create a new S3 Bucket, or 'false' to use an existing one.
* Account ID: Inform your BMS Account ID.
* Event Store ID: Inform the Event Store ID, you can find it by clicking on <img src="../.gitbook/assets/image (1035).png" alt="edit" data-size="line"> at the same row as the event store you wish to import.
* API Key: Inform a BMS API Key with the "MON -Event Stores - Read Only" policy of access.

After filling out all the fields, at the end of the page, you must acknowledge that AWS CloudFormation might create IAM resources for this template. Then, click on 'Create Stack' to proceed with the stack creation.

### Template without VPC

If your AWS account does not have a Virtual Private Cloud (VPC) configured, use this template, which can be accessed [here](https://us-east-2.console.aws.amazon.com/cloudformation/home?region=us-east-2#/stacks/quickcreate?templateUrl=https://bms--public-files.s3.us-east-1.amazonaws.com/without-vpc.yaml\&stackName=bms%E2%80%93monitoring%E2%80%93event-pipe%E2%80%93event-recorder).

<figure><img src="../.gitbook/assets/image (1038).png" alt=""><figcaption><p>Template without VPC</p></figcaption></figure>

After accessing the template, fill in the details:

* Stack Name: This field is automatically filled, but you can use it to customize the stack name.
* S3 Bucket Name: Inform or create a name of your S3 Bucket.
* Create S3 Bucket: Choose 'true' to create a new S3 Bucket, or 'false' to use an existing one.
* Account ID: Inform your BMS Account ID.
* Event Store ID: Inform the Event Store ID, you can find it by clicking on <img src="../.gitbook/assets/image (1035).png" alt="edit" data-size="line"> at the same row as the event store you wish to import.
* API Key: Inform a BMS API Key with the "MON -Event Stores - Read Only" policy of access.
* Subnet IDs: Select a subnet ID for the Lambda function from the drop-down list.
* Security Group IDs: Select a security group ID for the Lambda function from the drop-down list.

After filling out all the fields, at the end of the page, you must acknowledge that AWS CloudFormation might create IAM resources for this template. Then, click on 'Create Stack' to proceed with the stack creation.

## Additional Information

Now you have integrated your BMS Event Stores with AWS and your data will start to be sent as soon as the stack creation is completed, you can follow this process at your stacks dashboard. Check these articles to learn more about related BMS Features and AWS products:

* [Event Pipes](../product-documentation/monitoring/event-pipes.md)
* [Event Stores](../product-documentation/monitoring/event-stores.md)
* [API Keys](../product-documentation/gestion-de-acceso-e-identidad-iam/api-keys.md)
* [AWS CloudFormation](https://docs.aws.amazon.com/cloudformation/)
