# Off-Premises AWS Lab Setup
In this lab, I am going to show you how to create an off-premises IT Lab with AWS or Amazon Web Services. I am also going to show you how to create and configure an EC2 instance which is just a Virtual Machine, configure port rules so that we can connect to our Cloud VM, and how to terminate our EC2 instances and our off-premises lab. 
## Project Walkthrough: 
1. Sign in to AWS
  - Navigate to the AWS Management Console.
  - Log in with your AWS credentials. If you don't have an account, you'll need to create one.
2. Access the EC2 Dashboard
  - In the AWS Management Console, type “EC2” in the search bar and select EC2 under Services.
  - This will take you to the EC2 Dashboard.
3. Launch a New Instance
  - Click on the Launch Instance button.
  - This will open the instance creation wizard.
4. Name Your Instance
  - Under Name and tags, enter a descriptive name for your instance.
5. Choose an Amazon Machine Image (AMI)
  - Under Application and OS Images (Amazon Machine Image), select an AMI. For beginners, the Amazon Linux 2 AMI is a good choice.
  - Ensure the AMI you select is marked as Free tier eligible if you're using the AWS Free Tier.
6. Choose an Instance Type
  - Select an instance type that suits your needs. For Free Tier users, t2.micro or t3.micro are eligible options.
  - Click Next: Configure Instance Details.
7. Configure Instance Details
  - You can leave the default settings for most options.
  - Ensure that Auto-assign Public IP is enabled if you want to connect to your instance over the internet.
  - Click Next: Add Storage.
8. Add Storage
  - The default storage configuration is typically sufficient.
  - Ensure the storage size and type meet your requirements.
  - Click Next: Add Tags.
9. Add Tags
  - Tags are key-value pairs that help you manage and identify your AWS resources.
  - Add a tag with the key Name and a value that identifies your instance.
  - Click Next: Configure Security Group.
10. Configure Security Group
  - Security groups act as virtual firewalls for your instance.
  - Create a new security group or select an existing one.
  - Add rules to allow specific types of traffic (e.g., SSH for Linux or RDP for Windows).
  - Click Review and Launch.
11. Review and Launch
  - Review all your configurations.
  - Click Launch.
  - A prompt will appear asking you to select a key pair.
12. Select or Create a Key Pair
  - If you have an existing key pair, select it.
  - To create a new key pair: Click Create a new key pair, Enter a key pair name, Download the .pem file and store it securely. This file is essential for connecting to your instance.
  - Acknowledge that you have access to the selected key pair.
  - Click Launch Instances.
13. View Your Instance
  - Click View Instances to see your running instances.
  - Wait for the instance state to show as running and the status checks to pass.
14. Connect to Your Instance
  - Select your instance and click Connect.
  - Follow the provided instructions to connect via SSH (for Linux) or RDP (for Windows), using the key pair you specified earlier.



