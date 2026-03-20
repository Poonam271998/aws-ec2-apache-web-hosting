# aws-ec2-apache-web-hosting

# 🚀 AWS EC2 Apache Web Server Setup

## 👩‍💻 Author

**Poonam Langote**

---

## 📌 Project Overview

This project demonstrates how to:

* Launch an AWS Free-Tier EC2 instance
* Connect to the instance using SSH (PuTTY)
* Install and configure Apache Web Server
* Deploy a custom webpage

---

## ☁️ AWS Configuration

* **Region:** ap-south-1
* **Instance Type:** t2.micro (Free Tier)
* **AMI:** Amazon Linux 2

---

## 🔐 Security Group Rules

| Type | Protocol | Port | Purpose      |
| ---- | -------- | ---- | ------------ |
| SSH  | TCP      | 22   | Remote Login |
| HTTP | TCP      | 80   | Web Access   |

---

## 🔗 Connect to EC2 (Using PuTTY)

1. Convert `.pem` file to `.ppk` using PuTTYgen
2. Open PuTTY
3. Enter Public IP
4. Load `.ppk` file
5. Click **Open** to connect

---

## ⚙️ Installation Steps

Run the following commands:

```bash
sudo yum update -y
sudo yum install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd
```

---

## 🌐 Deploy Webpage

```bash
echo "<h1>Hello from EC2 - Poonam</h1>" | sudo tee /var/www/html/index.html
```

---

## 🌍 Access Website

Open in browser:

```
http://43.205.230.222
```

---

## ✅ Output

* Apache server installed successfully
* EC2 instance accessible via browser
* Custom webpage deployed

---

## 📸 Screenshots

* output screenshots added in word file

---

## 💡 Key Learnings

* AWS EC2 instance creation
* Security group configuration
* SSH connection using PuTTY
* Apache installation and management
* Hosting a static webpage on cloud

---

## 📜 Conclusion

This project provides hands-on experience with AWS EC2 and basic web hosting using Apache. It is a foundational step toward cloud and DevOps practices.

---
