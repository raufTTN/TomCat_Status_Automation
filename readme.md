EC2 Tomcat Status Checker via AWS SSM


This Python script is designed to remotely check the status of the Tomcat service (tomcat, tomcat8, or tomcat9) on AWS EC2 instances using AWS Systems Manager (SSM). It uses the Boto3 SDK to interact with EC2 and SSM services.

📌 Features :

-> Automatically discovers EC2 instances managed by SSM.

-> Checks the status of Tomcat-related services using systemctl.

-> Displays instance IDs, instance names, and service status.

-> Handles multiple instances and outputs clearly formatted results.

✅ Prerequisites

-> Before running the script, ensure the following:

-> SSM Agent is installed and running on your EC2 instances.

-> The instance is associated with an IAM role that has AmazonSSMManagedInstanceCore permissions.

-> A security group attached to your instance must allow port 22 (SSH) access.

-> Python environment with Boto3 installed.



Steps ----
We can use this script on AWS CLI on console as well as on our system as well with AWS CLI.

Step 1. Go to AWS CLI.

Step 2. Pull the GitHub repo -- git clone https://github.com/raufTTN/TomCat_Status_Automation

Step 3. cd TomCat_Status_Automation

Step 4. python3 TomCatStatus.py

Step 5. It will fetch all servers and will SSM into each servers to check tomcat status.
