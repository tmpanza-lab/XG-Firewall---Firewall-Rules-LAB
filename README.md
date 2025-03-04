# XG Firewall | Firewall Rules LAB

## Objective

The main objective of this XG Firewall Rules Lab is to design, implement, and test firewall rules to regulate traffic between different network segments while ensuring security and proper connectivity.

### Job Skills Learned

- Basic Sophos XG Firewall Administration Skill
- Understanding Network Segmentation
- Configuring Firewall Rules
- Implementing NAT and Routing Policies
- Testing and Validating Security Policies


### Tools Used

- Sophos XG Firewall VM: A virtual appliance used in virtualized environments (VMware).
- SFOS 17.5 Web Interface (GUI)
- SFOS 17.5 Command Line Interface (CLI)
- Control Center Dashboard: Built-in monitoring tool for real-time traffic and event analysis.
- Backup and Restore Tools
- FTP/HTTP/HTTPS Servers: For uploading firmware or serving configurations during the lab.
- Traffic Generation Tools
- EVE-NG for simulating network devices (e.g., routers, PCs, or switches) to test


*Ref 1: Network Diagram*
 ![image](https://github.com/user-attachments/assets/82f27e18-7b46-4086-837c-f8fdfb107f27)


### STEPS
![image](https://github.com/user-attachments/assets/e68a87f6-e87b-44c9-b457-78ae5ce37283)
 

### LAN-WAN

1.	- Rule1: Allow internet access to IT Users (User Rule)
![image](https://github.com/user-attachments/assets/a75bf248-f521-4cff-93c1-f1cdb4516882)
![image](https://github.com/user-attachments/assets/160d5c42-8709-4806-b22f-23a879322bf9)

 
 
User rule source
![image](https://github.com/user-attachments/assets/27eac05f-ff52-4e77-a93a-24aa9db5e541)
 
Destination & Services
![image](https://github.com/user-attachments/assets/7f0369d4-3e83-4742-87aa-d8bd808dc2f6)
 
Web malware and content scanning
![image](https://github.com/user-attachments/assets/434943e8-accf-4e8c-8479-9b28bf2d70a4)

 
Advanced and Log Traffic
![image](https://github.com/user-attachments/assets/321ec454-cb7c-4dba-9c5f-f856dc75f1bb)
 
Outcome
![image](https://github.com/user-attachments/assets/e13ad361-71dc-40e5-85db-c05c9aa827ed)
 

I can ping google
![image](https://github.com/user-attachments/assets/93802a22-1c82-46a9-ba3d-329ded0ff9c9)
![image](https://github.com/user-attachments/assets/c26f1a91-635d-4360-ab7c-7c97feaae7f1)
![image](https://github.com/user-attachments/assets/7ec29851-8f06-421d-b6aa-386ff904ea0e)
![image](https://github.com/user-attachments/assets/dd72ca23-0b06-43c4-a0d7-9bee94404b30)
 

 

 
 
Log Viewer
![image](https://github.com/user-attachments/assets/63ee9f13-5777-4981-8ff2-47221dc1023c)
![image](https://github.com/user-attachments/assets/effcdd61-9a75-4bbf-8749-29c5128e8710)
 
 
2.	- Rule2: Allow internet access to Account Users (User Rule)
![image](https://github.com/user-attachments/assets/73208377-6653-484e-abe4-22a6cb0e6d31)
 ![image](https://github.com/user-attachments/assets/502a1ce1-7921-4101-a2fa-d4c84cc26bfd)

 
Rules Created
![image](https://github.com/user-attachments/assets/cba5c3f0-b169-4632-b7de-99e3db3b1ed9)
 

IT Staff can now access internet
![image](https://github.com/user-attachments/assets/9945d66e-b64a-4a59-ba11-8491bc561d03)
![image](https://github.com/user-attachments/assets/65ade60f-7769-4247-90d9-61f88c2191fd)
 
 

### LAN-Servers
![image](https://github.com/user-attachments/assets/2f3848d0-6bfa-45e4-97de-3be85b3be362)
 

1.	- Rule1: Allow Servers access to IT (Network Rule-Any Service)
![image](https://github.com/user-attachments/assets/2ce9e025-dd7d-43f3-a3f8-81493936e412)
![image](https://github.com/user-attachments/assets/4693bfc9-e6b1-45bd-bbe4-db835cc22f2d)
![image](https://github.com/user-attachments/assets/626e792f-06ea-4342-b85c-100e8d277db0)
 
 
 
LAN PC is now able to communicate with my Servers
![image](https://github.com/user-attachments/assets/438d8df4-ac55-488c-b16f-eb9c49edce76)
 


Diagnostics using packet capture
![image](https://github.com/user-attachments/assets/327900e4-881b-445c-90be-b86dab050951)
![image](https://github.com/user-attachments/assets/84c26844-3854-4922-986a-722d7181ba73)
![image](https://github.com/user-attachments/assets/9975415c-3cc9-4104-aced-75573531c645)
 
 
 

Rule Group is created
![image](https://github.com/user-attachments/assets/17fc845a-1fb1-4494-8c11-016774402f92)
 
Log Viewer
![image](https://github.com/user-attachments/assets/e891b78c-831e-41c5-b16f-3595fcf443b9)
 

2.	- Rule2: Allow DNS, DHCP Service to Accounts
 ![image](https://github.com/user-attachments/assets/5b29e25f-a24e-4928-90b6-657bd122ddde)
![image](https://github.com/user-attachments/assets/0374eece-9d22-4f7d-aece-18d86048e15c)
![image](https://github.com/user-attachments/assets/647ff3d9-1c2d-4b73-9984-2041c21fcd50)
![image](https://github.com/user-attachments/assets/99bb8d66-3c16-466d-b5c9-6ad87e004342)


 
 
 
DNS is coming from AD Server
![image](https://github.com/user-attachments/assets/6342e2fe-b16c-4ca3-bfaf-4c89196e9735)
 


### Servers-LAN

1.	- Rule1: Allow Servers access to IT (Network Rule-Any Service)
2.	- Rule2: Allow DNS, DHCP Service to Accounts
![image](https://github.com/user-attachments/assets/d051b5b3-334e-44bb-b77b-86a13e2b13c8)
![image](https://github.com/user-attachments/assets/efb5da09-c24f-4df1-a5e8-cb7548e4af10)
![image](https://github.com/user-attachments/assets/8053abf1-4a7c-47a1-8250-b5a71ba309cd)
![image](https://github.com/user-attachments/assets/2ffbcfe9-96b0-4ef7-ab61-2952b74bef7b)
 
 

 

 

### LAN-LAN

1.	- Rule1: Allow internal Service
 ![image](https://github.com/user-attachments/assets/52bf8aeb-c8d9-4394-b2ec-706e8f52b589)
![image](https://github.com/user-attachments/assets/bb382073-e22a-4f29-a8eb-29f0b5222f87)
![image](https://github.com/user-attachments/assets/2277c1e4-a3e1-4122-9f0b-752914323ffa)


 

 

### Servers-WAN
 ![image](https://github.com/user-attachments/assets/e34760c6-9717-45e7-a90e-c1b3f8109dfc)
![image](https://github.com/user-attachments/assets/7b684fef-9816-4a67-adc8-965082f4f502)
![image](https://github.com/user-attachments/assets/12a66435-62fc-4945-b06e-39ac47d172e7)
![image](https://github.com/user-attachments/assets/1ad54cb6-630a-4c51-a84d-ae4f59042cc4)

 

 

 

This is the rule order
![image](https://github.com/user-attachments/assets/35fba19e-4b6e-4481-8ce2-085ac1ff27fa)


Let us test the Internet Access from our AD Server.
 ![image](https://github.com/user-attachments/assets/36fd8512-be45-408f-b676-e1257185e2ca)
![image](https://github.com/user-attachments/assets/da85a501-7193-4ea0-a7e1-602ea0fd8a02)

My Server can access the Internet.
![image](https://github.com/user-attachments/assets/7fb5318a-3289-400a-86ad-0955d837f709)



 
 

 


