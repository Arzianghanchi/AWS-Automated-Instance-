# AWS-Automated-Instance-

1. Verifying Prerequisites:
Open the AWS Management Console. Search for "EC2 Instances" and ensure your instance is healthy.
Check SSM Agent: SSH into your instance and run systemctl status amazon-ssm-agent (Linux) or check "Amazon EC2 SSM Agent" status in services.msc (Windows). If not running, follow AWS documentation to install it.

2. Using the Pre-built Document:
Navigate to the AWS Systems Manager service.
In the navigation pane, select Run Command.
Click on the Targets tab. Enter your instance ID (i-01234567890abcdef) in the search bar.
Click on the Document name field and select AWS-RestartEC2Instance.
Review the document details (it restarts the instance) and click the orange Run button.

3.Simulating the Restart:
A confirmation popup appears. Click Run to initiate the restart command.
In the Run Command history pane, you'll see the execution status. It might take a few minutes for the instance to restart.
3. Verifying the Restart (Optional):

Go back to the EC2 Instances service. After a successful restart, the instance status should change to "running."
