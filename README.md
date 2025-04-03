# Creating-Azure-VM
![azurevm](https://github.com/user-attachments/assets/2898c346-84ae-4819-ad33-1e8d2de0f027)




Step-by-Step Guide to Create a VM on Azure for GitHub Projects
1. Sign in to Azure Portal
Go to Azure Portal.

Sign in with your Microsoft account.
# 
2. Create a New Virtual Machine
In the Azure portal, click on "Create a resource".


# ![Screenshot 2025-04-02 142613](https://github.com/user-attachments/assets/be760121-7381-4e45-9b1a-208f1cbd764b)


Select "Virtual Machine" under Compute.

# ![Screenshot 2025-04-02 142613](https://github.com/user-attachments/assets/40659d08-4852-47be-83b0-19fdf2d5067a)






Click "Create".



3. Configure Basic Settings
Subscription: Choose your Azure subscription.

Resource Group: Create a new one or select an existing one.

Virtual Machine Name: Provide a unique name (e.g., GitHub-VM).

Region: Choose the nearest Azure data center.

Availability options: Leave as default if not required.

# ![Screenshot 2025-04-02 142854](https://github.com/user-attachments/assets/d64c8fd1-430c-481a-9085-175649356728)



Image – Choose the OS (e.g., Ubuntu 22.04 LTS or Windows Server).

Size – Choose an instance size (Standard_B1s for light use, or bigger if needed).

Administrator Account:

Authentication type: Choose Password or SSH Key (recommended for security).

Username: Set a username (e.g., azureuser).

Password: Set a strong password if using password authentication.



# ![Screenshot 2025-04-03 111349](https://github.com/user-attachments/assets/7958c818-edd6-4c4f-9d9e-465eabae38ab)




4. Configure Networking
Under Networking, ensure Public IP is enabled if you need external access.

Inbound Ports – Allow ports for access:

SSH (22) for Linux or RDP (3389) for Windows.

HTTP (80) and HTTPS (443) if hosting a web project.

Custom Port (e.g., 3000 for Node.js apps).



# ![Screenshot 2025-04-03 114059](https://github.com/user-attachments/assets/a65e375e-1ed3-4083-bc10-15f3b65715f7)



5. Review and Create
Click Review + create.

Check the settings and click Create.

Wait for deployment to complete.


Step 6. Connect to the VM
For Linux (Ubuntu) VM:

Open a terminal and use SSH:



Replace your-public-ip with the actual VM public IP.

For Windows VM:

Download the RDP file from the Azure portal and connect via Remote Desktop.



# ![Screenshot 2025-04-03 115817](https://github.com/user-attachments/assets/8538cb11-5a6c-4cf3-a224-890d9b114d66)









