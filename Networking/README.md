## :zap: Launching an NGINX Web Server on an Amazon EC2 :cloud:

I will be highlighting the steps to launch an NGINX web server on an Amazon EC2 instance :cloud:, and map it to a domain purchased through Cloudflare

## 1) Purchase a domain on cloudfare, e.g "nginxhassan.com"

## 2) Launch an Amazon EC2 instance 
-AMI: Amazon Linux 2023
-Instance Type: t3.micro
-Security Group Inbound Rules:
-Port 22 (SSH) - Your IP
-Port 80 (HTTP) - 0.0.0.0/0
-Port 443 (HTTPS) - 0.0.0.0/0

## 3) Locate the Public IPV4 address on the instance summary, and note it down. 

## 4) Connect to the EC2 instance via SSH
ssh -i /path/to/key.pem ec2-user@<EC2_PUBLIC_IP>

## 5) Install NGINX
sudo yum update -y
sudo yum install -y nginx
sudo systemctl start nginx
sudo systemctl enable nginx

## 6) Login to your Cloudfare account, and create an A record for your domain. Point this to the Public IPV4 address you noted down earlier. 

<img width="345" height="56" alt="image" src="https://github.com/user-attachments/assets/78851876-e6b7-4af4-a23c-da181b57aa35" />

## 7) Go back onto the terminal, and confirm propagation.

nslookup (Your domain).
After a few minutes, the result should show the public IPV4 address, with your domain:

## 8) Customise your page with the command

sudo yum install nginx -y sudo systemctl start nginx

## 9) Finally, search your domain on your browser and you should find your website. :clap:
<img width="959" height="373" alt="image" src="https://github.com/user-attachments/assets/e1d9be67-76a2-4e2f-aa60-5b366cdd4d7c" />
