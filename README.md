# AWS-Automated-Instance-Restart

1. Verifying Prerequisites:
Open the AWS Management Console. Search for "EC2 Instances" and ensure your instance is healthy.
Check SSM Agent: SSH into your instance and run systemctl status amazon-ssm-agent (Linux) or check "Amazon EC2 SSM Agent" status in services.msc (Windows). If not running, Install Amazon EC2 SSM Agent" using AWS documentation.

2. Using the Pre-built Document:
Navigate to the AWS Systems Manager service.
In the navigation pane, select Run Command Option.
Click on the Targets tab and Enter your instance ID (i-01234567890abcdef) in the search bar.
Click on the Document name field and select AWS-RestartEC2Instance.
Review the document details (it restarts the instance) and click the orange Run button.

3. Simulating the Restart:
A confirmation popup will appear then Click on Run to initiate the restart command.
In the Run Command history pane, you'll see the status of execution . It might take a few minutes for the instance to restart.

4. Verifying the Restart (Optional):
Go back to the EC2 Instances . After a successful restart, the instance status should change to "running."

Images

Step 1 Copy Instance id.
![Copied instance id](https://github.com/Arzianghanchi/AWS-Automated-Instance-Restart/assets/118063625/a7dad7b7-c3a0-4379-ace4-963547f7d2ad)

Step 2 Go to System Manager.
![System Manager](https://github.com/Arzianghanchi/AWS-Automated-Instance-Restart/assets/118063625/f33ccb1a-d7c8-4c5c-b2c7-c81d97aa6e97)

Step 3 Select Automation Option.
![Automation Option](https://github.com/Arzianghanchi/AWS-Automated-Instance-Restart/assets/118063625/d4cb5265-90e2-4a62-b67d-7439cdfecab6)


Step 4 Click On Execute Automation.
![go on execucte automation](https://github.com/Arzianghanchi/AWS-Automated-Instance-Restart/assets/118063625/93f275b0-3a0b-4ae8-b472-8d58c329d288)

Step 5 Search AWS-Restart and Select it.
![Select AWS restart](https://github.com/Arzianghanchi/AWS-Automated-Instance-Restart/assets/118063625/2cca3679-d60f-4276-ba0b-d0305c4be2d1)

Step 6 Click on Execute Execution
![Exexute aws Automation](https://github.com/Arzianghanchi/AWS-Automated-Instance-Restart/assets/118063625/52bbfec9-e1f8-4552-99ca-ac8e209d19af)

Step 7 Configure the Runbook
![Runbook Configuration](https://github.com/Arzianghanchi/AWS-Automated-Instance-Restart/assets/118063625/ba1c6499-51f5-45b4-90da-485e18d949d9)

![Target ](https://github.com/Arzianghanchi/AWS-Automated-Instance-Restart/assets/118063625/57cf157c-5db3-462e-8089-fb925118ab05)

![Rate Control](https://github.com/Arzianghanchi/AWS-Automated-Instance-Restart/assets/118063625/1f924a12-aaa8-4e33-b7ef-88547b943f9b)

Step 8 Execute the Configured Runbook
![Runbook Execution](https://github.com/Arzianghanchi/AWS-Automated-Instance-Restart/assets/118063625/d853f1df-80d9-47d3-9b1f-f7911c8705dd)

Status of Automation
![Status runbook](https://github.com/Arzianghanchi/AWS-Automated-Instance-Restart/assets/118063625/bfbaa93f-d8b6-422a-9a37-1721d74f8cb7)

Instace Stopped After Execution of runbook
![Instance state after execution](https://github.com/Arzianghanchi/AWS-Automated-Instance-Restart/assets/118063625/8f40eb9d-a0e2-4a73-a315-75105ff79abd)


Execution Status
![Execution steps](https://github.com/Arzianghanchi/AWS-Automated-Instance-Restart/assets/118063625/627a6c9c-d1c1-47a0-8d3a-c30a1823a235)



