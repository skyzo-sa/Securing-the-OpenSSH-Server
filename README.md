# Securing the SSHd daemon
# Change the configuration file (/etc/ssh/sshd_config) and then restart the server
man sshd_config
 
a) Change the port
Port 2278
![image](https://github.com/user-attachments/assets/ad953dde-3d7b-418a-9705-11713fd852fd)
  
b) Disable direct root login
PermitRootLogin no
![image](https://github.com/user-attachments/assets/7438bb1d-d222-42d6-a4b6-54b565e54bf2)
  
c) Limit Users’ SSH access
AllowUsers stud u1 u2 john
![image](https://github.com/user-attachments/assets/459a17b4-3c1d-4356-a552-f9d1dfcc20b6)
  
d) Filter SSH access at the firewall level (iptables)
![image](https://github.com/user-attachments/assets/703848f9-d674-4e0e-85f3-84fd15e6fe65)
 
 
e) Activate Public Key Authentication and Disable Password Authentication

Generating SSH Key pair on Windows
![image](https://github.com/user-attachments/assets/334bb409-0093-4bdd-b0ee-d8ce83eb7b50)
![image](https://github.com/user-attachments/assets/ba48925a-19dc-4751-b60d-05b3f4f1dce0)

 
 
Generating SSH Key pair on Linux
![image](https://github.com/user-attachments/assets/c61901fb-0b94-45c1-8c9a-a4a5da4abb76)
![image](https://github.com/user-attachments/assets/c76d57f8-87ce-4776-b31e-59bb120942fd)
![image](https://github.com/user-attachments/assets/d84b4156-0006-4f97-bc69-f25bc6f28a2d)
![image](https://github.com/user-attachments/assets/191f6393-75fb-4906-b53a-631dd57daf93)
 
 
 
f) Use only SSH Protocol version 2
 
g) Other configurations:
ClientAliveInterval 300
ClientAliveCountMax 0
MaxAuthTries 2
MaxStartUps 3
LoginGraceTime 20
![image](https://github.com/user-attachments/assets/de4abac2-3caf-4f4f-be51-7229648259d3)
![image](https://github.com/user-attachments/assets/33772448-f30f-4a0d-967f-beb179eb3242)
 
 
