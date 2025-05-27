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
