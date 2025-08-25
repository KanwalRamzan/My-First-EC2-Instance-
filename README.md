# My First AWS EC2 Windows Server Instance
This repository documents the process of launching, configuring, and connecting to a Windows Server 2019 instance on Amazon Web Services (AWS) using the EC2 service. This project served as a foundational exercise to understand cloud instance management and remote access protocols.
**Objective**
The primary goal of this project was to successfully deploy a Windows-based virtual machine in the cloud and establish a secure Remote Desktop Protocol (RDP) connection to it.

**Technologies Used**
•	AWS EC2: Cloud computing service for launching and managing virtual servers.
•	Windows Server 2019: The operating system used for the EC2 instance.
•	Remote Desktop Protocol (RDP): The protocol used to remotely connect to the Windows instance.
•	AWS Management Console: The web-based interface for managing AWS services.

**Methodology and Key Steps**

1. **Instance Launch**
•	An EC2 instance was launched using a Windows Server 2019 AMI.
•	A new key pair was generated to secure the instance, and the private key (.pem) file was downloaded.
•	A new security group was created to control network traffic.

3. **Initial Access and Troubleshooting**
•	The instance entered a "Running" state, but the status checks remained "Initializing" for an extended period, preventing a connection.

  •	**Troubleshooting Steps:**
• Checked System Logs: I viewed the system log in the AWS Management Console, which showed the message "Windows is Ready to use." This confirmed the operating system had booted successfully, indicating the issue was not with the instance itself but with the connection.
• Verified Security Group Rules: I checked the inbound rules of the security group to ensure that RDP traffic (port 3389) was allowed from my IP address. The rule was correctly configured.
• Re-generated Password: I re-generated the RDP password using the private key file to ensure there were no copy-paste errors in the credentials.






