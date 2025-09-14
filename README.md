# class71sthomeworksept25
# EC2 Web Server Deployment Homework

## Setup Instructions
1. Log in to AWS Console.
2. Create a security group first by allowing inbound HTTP (port 80) traffic with Source Anywhere IPv4. Never touch outbound rules and save.
3. Launch an EC2 instance:
   - AMI: Amazon Linux 2
   - Instance type: t2.micro (Free Tier eligible)   
   - Add User Data: Copy content of `simple_startup-metadata_script_example.txt`
4. Launch and wait for instance to start.

## Verification
- Copy Public IPv4 DNS from EC2 console.
- Open in browser: `ec2-13-230-101-168.ap-northeast-1.compute.amazonaws.com`
- You should see "My EC2 Instance and Instance Details including Hostname, Private IP and Availability Zone".

## Screenshot
![screenshot])<img width="1043" height="489" alt="class71sthomeworkscreenshot" src="https://github.com/user-attachments/assets/c738fa1e-a58d-4355-91a0-9c5d5ab00ec7" />


## Teardown Instructions
1. Terminate the EC2 instance from the AWS Console.
2. Delete associated Security Group if created manually.
3. Delete Key Pair if not needed anymore.
4. Confirm no resources remain to avoid billing.
