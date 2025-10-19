# DevOps Server Setup on AWS EC2 (Amazon Linux)

## Overview
This project sets up three servers on a single EC2 instance:
1. **Web Server** - Apache (httpd)
2. **Mail Server** - Postfix
3. **DNS Server** - BIND9

## EC2 Instance
- OS: Amazon Linux 2023
- Public IP: 54.160.134.186
- User: ec2-user

## Commands Summary

### Web Server (Apache)
```bash
sudo dnf install httpd -y
sudo systemctl enable httpd
sudo systemctl start httpd
sudo dnf install postfix mailx -y
sudo systemctl enable postfix
sudo systemctl start postfix
sudo dnf install bind bind-utils -y
sudo systemctl enable named
sudo systemctl start named
NAME : EZEOGU CHUKWUEMEKA DANIEL
