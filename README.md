⚖️ AWS Network Load Balancer (NLB) Project
🏗️ Architecture

<img width="1693" height="929" alt="ChatGPT Image Jun 21, 2026, 01_17_44 PM" src="https://github.com/user-attachments/assets/b4502a32-9431-4b98-9305-9d4e39833ebe" />


📌 Description:
High availability setup using AWS NLB distributing traffic across EC2 instances in multiple AZs.

📸 Step-by-Step Flow (Screenshots)
1️⃣ VPC Setup

<img width="1533" height="756" alt="vpc (1)" src="https://github.com/user-attachments/assets/4d3d1de6-d21f-48a3-8b6e-d0511f190bfa" />


📌 Create VPC with 2 public subnets in different Availability Zones.

<img width="1373" height="605" alt="subnets (1)" src="https://github.com/user-attachments/assets/f6fbb8c8-a848-4d7b-bd6f-32c188328b12" />


2️⃣ EC2 Instances (Apache Setup)

📌 Launch two EC2 instances and install Apache web server.

<img width="1643" height="100" alt="two instance running (1)" src="https://github.com/user-attachments/assets/e377e803-995a-4ab8-982e-2bba835457fd" />


3️⃣ Target Group

📌 Register EC2 instances into target group for load balancing.

<img width="1350" height="647" alt="nlb (1)" src="https://github.com/user-attachments/assets/b8e08323-b661-4c08-a34e-cdcad8cc8c8b" />


4️⃣ Network Load Balancer

📌 Create NLB and attach target group for traffic distribution.

<img width="1597" height="382" alt="Screenshot 2026-06-21 132913" src="https://github.com/user-attachments/assets/0aa05bf3-a577-4604-bb01-1067df8c1d30" />



5️⃣ Testing (Load Balancing Output)

📌 Access NLB DNS and verify traffic switching between EC2 instances.

<img width="1901" height="866" alt="Screenshot 2026-06-17 104457" src="https://github.com/user-attachments/assets/8fc68bd5-8307-487b-bfaf-74c8fdd7bb06" />

<img width="1901" height="807" alt="Screenshot 2026-06-17 110714" src="https://github.com/user-attachments/assets/d1198ba6-72f7-44e2-8301-3abccafa6b2c" />



6️⃣ CloudWatch Monitoring

📌 Monitor logs and health checks of instances.

<img width="1427" height="496" alt="NLB health (1)" src="https://github.com/user-attachments/assets/946cf1f6-a6a0-48fa-a0b8-cf7b0d884f0a" />


🎯 Final Output
Highly available architecture
Traffic distributed across EC2 instances
Fault tolerant multi-AZ system
Real-time monitoring enabled
⚡ Flow Summary

Internet → NLB → Target Group → EC2 Instances → CloudWatch
