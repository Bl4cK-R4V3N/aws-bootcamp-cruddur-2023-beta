# Week 0 — Billing and Architecture

Install CLI

Instructions: https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html

**For windows:**

Download and run the AWS CLI MSI installer for Windows (64-bit):

https://awscli.amazonaws.com/AWSCLIV2.msi

Alternatively, you can run the msiexec command to run the MSI installer.

C:\> msiexec.exe /i https://awscli.amazonaws.com/AWSCLIV2.msi
For various parameters that can be used with msiexec, see msiexec on the Microsoft Docs website. For example, you can use the /qn flag for a silent installation.

C:\> msiexec.exe /i https://awscli.amazonaws.com/AWSCLIV2.msi /qn
To confirm the installation, open the Start menu, search for cmd to open a command prompt window, and at the command prompt use the aws --version command.

C:\> aws --version
aws-cli/2.10.0 Python/3.11.2 Windows/10 exe/AMD64 prompt/off

LINUX and MAC commands under website: https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html


**BILING**

https://docs.aws.amazon.com/account-billing/index.html


**Review your bills and usage**
To open the Billing console and view your usage and charges
Sign into the AWS Management Console and open the Billing console at https://console.aws.amazon.com/billing/.

Choose Bills to see details about your current charges.

Choose Payments to see your historical payment transactions.

Choose AWS Cost and Usage Reports to see reports that break down your costs.

For more information about setting up and using AWS Cost and Usage Reports, see the AWS Cost and Usage Reports User Guide.


**Check that the AWS CLI is working and you are the expected user**

aws sts get-caller-identity
You should see something like this:

{
    "UserId": "AIFBZRJIQN2ONP4ET4EK4",
    "Account": "655602346534",
    "Arn": "arn:aws:iam::655602346534:user/andrewcloudcamp"
}


**Create budget**

https://docs.aws.amazon.com/cli/latest/reference/budgets/create-budget.html

Get your AWS Account ID

aws sts get-caller-identity --query Account --output text


Supply your AWS Account ID
Update the json files
This is another case with AWS CLI its just much easier to json files due to lots of nested json

aws budgets create-budget \
    --account-id AccountID \
    --budget file://aws/json/budget.json \
    --notifications-with-subscribers file://aws/json/budget-notifications-with-subscribers.json

