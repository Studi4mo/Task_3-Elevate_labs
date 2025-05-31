# 🛡️ Nessus Installation on Kali Linux

This guide provides step-by-step instructions for installing and configuring Nessus Essentials (free version) on Kali Linux.

## 📋 Prerequisites
- Running Kali Linux installation 
- Active internet connection
- Valid email address for activation code
- Sudo privileges

---

## 🚀 Installation Steps

### 1. Obtain Activation Code
![Registration Page](https://github.com/user-attachments/assets/ccb1a710-0837-4d62-9ad8-7024953325e7)

1. Visit [Nessus Essentials Registration Page](https://www.tenable.com/products/nessus/nessus-essentials)
2. Fill in your name and email to receive the activation code
3. You'll be redirected to the download page after registration

![image](https://github.com/user-attachments/assets/cdbeff25-9778-44ad-bc2c-b7b9295b4afa)

---

### 2. Download Nessus Package
1. Select "Nessus for Debian/Kali Linux (64-bit)" from download options
2. Note the download location (typically `~/Downloads`)

![Download Selection](https://github.com/user-attachments/assets/962dadf6-eee5-4272-9646-c4c3fa9e6daf)

---

### 3. Install Nessus
- Use the following command to install the downloaded package:
sudo dpkg -i nessus-10.x.x-debian10_amd64.deb
![Screenshot 2025-05-29 152937](https://github.com/user-attachments/assets/4923c940-723a-4468-b248-1aec264514ba)

- Start the Nessus Service
  - sudo systemctl start nessusd
  - sudo systemctl enable nessusd
  - Wait 1–2 minutes for the service to initialize



 **4.Launch Browser**  
   Open your preferred web browser (Firefox recommended)

**Navigate to Local Address**  
   Enter the following URL: https://localhost:8834/
 **Handle Security Warning**  
- You'll see a "Your connection is not private" warning
![image](https://github.com/user-attachments/assets/e0987644-3bbe-47f2-924c-118fbf54e7fa)

- Click "Advanced" → "Proceed to localhost (unsafe)"
*This is safe because it's a local self-signed certificate*

**Select Product Version**  
Choose 
+ Nessus Essentials (FREE) - For personal/home use
+ Create an account to start scanning. After logging in  Nessus will download and compile the necessary plugins. This process may take 
some time.


