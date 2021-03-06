---
title: "Installing the CloudConnector"
chapter: false
weight: 242
---

## Steps

To install this tool, we will be using a CloudFormation Template. Follow the steps below to install the Sysdig CloudConnector:

1. Navigate to the [[CloudFormation template for Sysdig Cloud Connector deployment](  https://console.aws.amazon.com/cloudformation/home#/stacks/create/template?stackName=CloudConnector&templateURL=https://cf-templates-cloud-connector.s3.amazonaws.com/cloud-connector.template)]( https://console.aws.amazon.com/cloudformation/home#/stacks/create/template?stackName=CloudConnector&templateURL=https://cf-templates-cloud-connector.s3.amazonaws.com/cloud-connector.template) template. The template will preview in CloudFormation. ![cf1](/images/20_workshop_setup/cf1.png)

2. On the “**Create stack**” section, click the '**Next**' button to start setting up the template. ![cf2](/images/20_workshop_setup/cf2.png)

3. The _“Specify stack details”_ section has no parameters for you to configure, so you can just press the **Next** button. ![cf3](/images/20_workshop_setup/cf3.png)

4. On _“Configure stack options_” screen, press the **Next** button. You can optionally add tag keys and values to the deployment, but no further configuration is required. Finally, you will be presented with a summary of all the parameters you previously introduced. Please note that dedicated IAM roles will be created to perform the scanning. These roles follow the "least privilege principle" to enforce maximum security. ![cf4](/images/20_workshop_setup/cf4.png)

5. Once you are happy with the plan, acknowledge it by marking the checkbox, and then press the **Create stack** button. ![cf5](/images/20_workshop_setup/cf5.png)

## All ready!

On the CloudFormation dashboard, you should see the template in _CREATE_IN_PROGRESS_ state. 

![cf6](/images/20_workshop_setup/cf6.png)

The creation process may take up to ten minutes. In the meantime you can continue with this workshop. You can later revisit the CloudFormation section in AWS to check the status of the deployment. It will show as “CREATE_COMPLETE” once the deployment has completed successfully.

![cf7](/images/20_workshop_setup/cf7.png)