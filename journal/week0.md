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


**I followed the instructions on the AWS CLI Install Documentation Page. File was downloaded and executed**

![image](https://user-images.githubusercontent.com/125925180/221438033-cb556884-fffd-4e6c-94bf-cd8cc783a96c.png)

after installation I need to configure AWS CLI

![image](https://user-images.githubusercontent.com/125925180/221438314-3a819c85-03e3-4ee0-942f-c0b1c8801044.png)

For that purpose I create Access Key in AWS for USer

![image](https://user-images.githubusercontent.com/125925180/221438874-205a1898-0d71-4249-807f-ce9506d9b147.png)

After configuration I got success 

![image](https://user-images.githubusercontent.com/125925180/221439022-554ec66e-5fcf-4ffa-92e8-3f21b125583b.png)


----------------------------------------------------------------------------
**Budget creation**

![image](https://user-images.githubusercontent.com/125925180/221439083-b1e2c032-a6bf-47a8-9241-290059283978.png)


----------------------------------------------------------------------------
**Recreate Logical Architectural Deisgn**

https://lucid.app/lucidchart/544c8c2f-b7ff-4f7c-87fb-e7283d98dd27/edit?viewport_loc=-320%2C-1698%2C3479%2C2378%2C0_0&invitationId=inv_028ef88e-2e02-44d3-abb2-bf99fdbbdbe9

![image](https://user-images.githubusercontent.com/125925180/221439152-f525a07a-011e-40a2-a43c-5cf695e934eb.png)



