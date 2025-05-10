# Off-Premises AWS Lab Setup
In this lab, I am going to show you how to create an off-premises IT Lab with AWS or Amazon Web Services. I am also going to show you how to create and configure an EC2 instance which is just a Virtual Machine, configure port rules so that we can connect to our Cloud VM, and how to terminate our EC2 instances and our off-premises lab. 
## Project Walkthrough: 
1. Sign in to AWS
  - Navigate to the AWS Management Console.
  - Log in with your AWS credentials. If you don't have an account, you'll need to create one.
2. Access the EC2 Dashboard
  - In the AWS Management Console, type “EC2” in the search bar and select EC2 under Services.
  - This will take you to the EC2 Dashboard.

![Image](https://github.com/user-attachments/assets/cffc2e95-793a-4250-a39c-b0b4a32c1610)


3. Launch a New Instance
  - Click on the Launch Instance button.
  - This will open the instance creation wizard.

![Image](https://github.com/user-attachments/assets/0f68a247-ad1a-4714-a6f2-074cc0c1bbe2)

4. Name Your Instance
  - Under Name and tags, enter a descriptive name for your instance.
5. Choose an Amazon Machine Image (AMI)
  - Under Application and OS Images (Amazon Machine Image), select an AMI. I have picked Microsoft Windows Server 2022.
  - Ensure the AMI you select is marked as Free tier eligible if you're using the AWS Free Tier.

![Image](https://github.com/user-attachments/assets/1b93ceb9-e586-4eae-9ab0-bfc39bc40d5e)

6. Choose an Instance Type
  - Select an instance type that suits your needs. For Free Tier users, t2.micro or t3.micro are eligible options.
  - Click Next: Configure Instance Details.

![Image](https://github.com/user-attachments/assets/0c39008a-1fb1-4591-a54f-5dae089d12a0)

7. Configure Instance Details
  - You can leave the default settings for most options.
  - Ensure that Auto-assign Public IP is enabled if you want to connect to your instance over the internet.
  - Click Next: Add Storage.

![Image](https://github.com/user-attachments/assets/c8b885e1-8df8-418f-8f81-0a79578c4be4)

8. Add Storage
  - The default storage configuration is typically sufficient.
  - Ensure the storage size and type meet your requirements.
  - Click Next: Add Tags.

![Image](https://github.com/user-attachments/assets/1869efcd-c2ba-4010-a8f0-b74c96ef5b45)

9. Add Tags
  - Tags are key-value pairs that help you manage and identify your AWS resources.
  - Add a tag with the key Name and a value that identifies your instance.
  - Click Next: Configure Security Group.
10. Configure Security Group
  - Security groups act as virtual firewalls for your instance.
  - Create a new security group or select an existing one.
  - Add rules to allow specific types of traffic (e.g., SSH for Linux or RDP for Windows).
  - Click Review and Launch.

![Image](https://github.com/user-attachments/assets/e77ef85c-48fb-424c-ba8f-d7445beecbd3)

11. Review and Launch
  - Review all your configurations.
  - Click Launch.
  - A prompt will appear asking you to select a key pair.
12. Select or Create a Key Pair
  - If you have an existing key pair, select it.
  - To create a new key pair: Click Create a new key pair, Enter a key pair name, Download the .pem file and store it securely. This file is essential for connecting to your instance.
  - Acknowledge that you have access to the selected key pair.
  - Click Launch Instances.

![Image](https://github.com/user-attachments/assets/c5216634-0aa9-458d-a3d5-c564ea1c2938)

13. View Your Instance
  - Click View Instances to see your running instances.
  - Wait for the instance state to show as running and the status checks to pass.
14. Connect to Your Instance
  - Select your instance and click Connect.
  - Follow the provided instructions to connect via SSH (for Linux) or RDP (for Windows), using the key pair you specified earlier.
15. Terminate session
  - To terminate the session, quit the virtual machine.
  - Click on Instances in the left sidebar.
  - Select the checkbox next to the instance you want to terminate.
  - Click the Instance state dropdown at the top.
  - Choose Terminate instance.
  - Confirm when prompted.

![Image](https://github.com/user-attachments/assets/f6d98d97-65ce-4a01-aab1-8d371d6ef924)

This concludes the AWS lab setup project! 



