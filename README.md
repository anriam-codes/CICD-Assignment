# 🚀 Launching a Windows EC2 Instance on AWS and Accessing via Remote Desktop

## 🎯 Aim
The aim of this lab is to **launch a Windows EC2 instance on AWS** and **access it remotely** from a local Windows machine using **Remote Desktop Connection (RDP)**.  
Through this experiment, we learn how to create, configure, and connect to a virtual Windows machine hosted in the cloud — demonstrating the core concept of **Infrastructure as a Service (IaaS)** in cloud computing.

🎥 <h3>Lab Demonstration Video: <a href="https://youtu.be/5-YWgwLRsVE" target="_blank">Watch on YouTube</a></h2>

---

## ⚙️ Steps Implemented

### 1. Login to AWS Console
- Open [https://aws.amazon.com](https://aws.amazon.com)  
- Sign in to your **AWS Management Console**.

### 2. Open EC2 Service
- In the search bar, type **EC2** and open the EC2 Dashboard.  
- Click on **Launch Instance** to create a new virtual machine.

### 3. Configure Instance Details
- **Name:** `MyWindowsServer`  
- **AMI (Amazon Machine Image):** Select *Windows Server 2019 Base*  
- **Instance Type:** Choose *t2.micro* (Free tier eligible)  
- **Key Pair:** Create or select an existing key pair and download the `.pem` file  
- **Network Settings:** Enable **RDP (port 3389)** under security group rules  
- Click **Launch Instance**

### 4. Wait for the Instance to Run
- Go to **Instances** in the left panel  
- Wait until the instance status changes to **Running**

### 5. Connect to the Instance
- Select your instance → Click **Connect** → Choose **RDP Client**  
- Click **Get Password**, upload your `.pem` file, and **Decrypt Password**  
- Copy the **Public DNS/IP** and **Administrator password**

### 6. Access via Remote Desktop
- On your local Windows system, open **Remote Desktop Connection (mstsc)**  
- Enter the **Public DNS/IP** → Click **Connect**  
- Login using **Administrator** and the **decrypted password**  
- You’ll now access the **Windows EC2 instance desktop**

### 7. Verification and Shutdown
- Check system info or open files to confirm it’s working  
- After completion, **log off** and **stop the instance** to avoid extra usage charges

---

## 👩‍💻 Observation
After completing the lab, we successfully created and accessed a **Windows environment on the AWS cloud** using EC2.  
This demonstrated how AWS provides scalable, on-demand virtual machines that can be accessed securely from any location.  
We observed how key pairs and RDP connections work together to ensure authentication and secure access to cloud resources.

---

## 💡 Applications / Examples
- **Cloud-based software testing** without using physical machines  
- **Hosting Windows servers** for applications or databases  
- **Remote system management** and **IT administration**  
- Running **enterprise tools or simulations** on demand  
- **Learning and training** environments for students or developers

---

## 🧰 Tools & Technologies Used
- **Amazon Web Services (AWS) EC2**
- **Windows Server 2025 Base**
- **Remote Desktop Connection (RDP)**
- **Key Pair Authentication**

---

## ✅ Conclusion
Through this experiment, we understood how to **deploy and manage virtual Windows instances** on the AWS cloud.  
This experiment gave me a clear idea of how **cloud computing**, **virtualization**, and **remote system management** actually work in real-world IT and DevOps environments.
