## AWS VPC Setup with Public and Private Subnets for Secure Application Deployment in Production

Objective: The primary objective of this project is to design and implement a secure and scalable Virtual Private Cloud (VPC) architecture in AWS for a production-grade environment. The setup includes public and private subnets to isolate services and provide enhanced security and efficient routing of traffic.

Scope:

	•	Virtual Private Cloud (VPC): Create a custom VPC to host cloud resources with a CIDR block suited for a production environment.
	•	Public and Private Subnets: Design two tiers of subnets (public and private) across multiple Availability Zones (AZs) to ensure high availability and fault tolerance.
	•	Internet Gateway: Attach an Internet Gateway (IGW) to the VPC to allow instances in the public subnet to communicate with the internet.
 	•	Auto Scaling Group (ASG): Implement an Auto Scaling Group to automatically scale the number of EC2 instances based on traffic and load metrics. 
	•	NAT Gateway: Deploy a Network Address Translation (NAT) Gateway in the public subnet to enable outbound internet connectivity for instances in the private subnet while keeping them protected from incoming traffic.
	•	Routing Tables: Configure separate routing tables for the public and private subnets to control traffic flow. Public subnet route tables will direct traffic to the IGW, while private subnet route tables will route traffic through the NAT Gateway.
	•	Security Groups and NACLs: Implement security groups and Network ACLs (Access Control Lists) to manage inbound and outbound traffic and to provide an additional layer of security.
	•	Bastion Host: Launch a Bastion Host in the public subnet for secure SSH access to instances running in the private subnet.
	•	EC2 Instances: Deploy EC2 instances across both the public and private subnets, with web servers in the public subnet and application servers in the private subnet.
	•	Application Load Balancer (ALB): Deploy an Application Load Balancer in the public subnet to distribute incoming traffic across multiple EC2 instances in the private subnet. 
 
Tools and Services:

	•	AWS VPC
	•	EC2
	•	Application Load Balancer (ALB)
	•	Auto Scaling Group (ASG)
	•	Internet Gateway (IGW)
	•	NAT Gateway
	•	VPC Flow Logs
	•	Security Groups & NACLs
	•	Bastion Host

Outcome: By the end of the project, the organization will have a production-ready, highly available, and secure AWS VPC environment capable of hosting applications with isolated networking layers, ensuring better security, and improved operational efficiency.

## AWS VPC Architecture

![vpc-example-private-subnets](https://github.com/user-attachments/assets/d9ec18b4-0856-4531-a3fd-7bd5361c6e70)

## sample screenshots

<img width="1440" alt="1" src="https://github.com/user-attachments/assets/305c925f-feb5-4258-b470-cf5121600072">
<img width="1440" alt="2" src="https://github.com/user-attachments/assets/6b5baa6c-50be-4699-a050-c652452b9908">
<img width="1440" alt="3" src="https://github.com/user-attachments/assets/e4659ee9-aec8-4471-8b00-c01ed7043bcb">
<img width="1440" alt="4" src="https://github.com/user-attachments/assets/80974256-8f4b-46aa-a429-f069df4a4246">
<img width="1440" alt="5" src="https://github.com/user-attachments/assets/047ecc1e-36be-4408-9f86-84a31da56dd9">
<img width="1440" alt="6" src="https://github.com/user-attachments/assets/535eb1f5-5195-4d88-a666-c24177bbdb26">
<img width="1440" alt="7" src="https://github.com/user-attachments/assets/66bf6564-a130-4e64-906c-436c1e5b59df">







