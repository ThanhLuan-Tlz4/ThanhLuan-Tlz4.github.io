---

title: "Worklog Week 3"
date: 2024-01-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
----------------------

### Week 3 Objectives:

* Understand the fundamental concepts of computer networking and network architecture on AWS.
* Understand the Amazon Virtual Private Cloud (Amazon VPC) model and its main components.
* Understand how Public Subnet, Private Subnet, Route Table, Internet Gateway, NAT Gateway, and Elastic IP work.
* Distinguish between Security Group and Network ACL in controlling network traffic.
* Practice building a complete network infrastructure on AWS and testing connectivity between components.

### Tasks to be implemented this week:

| Day | Tasks                                                                                                                                                                                                                                                                                                                    | Start Date | Completion Date | Reference Materials                                                   |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | --------------------------------------------------------------------- |
| 2   | **Networking Fundamentals**<br>- Review basic networking knowledge: IP Address, CIDR, Subnet Mask.<br>- TCP/IP model, TCP and UDP protocols.<br>- DNS, HTTP/HTTPS, and the principles of data transmission over a network.<br>- Network architecture in a Cloud environment.                                             | 01/05/2026 | 01/05/2026      | https://000010.awsstudygroup.com/                                     |
| 3   | **Amazon VPC - Theory**<br>- Overview of Amazon VPC.<br>- Region, Availability Zone (AZ).<br>- CIDR Block, IPv4.<br>- Public Subnet and Private Subnet.<br>- Route Table and Internet Gateway (IGW).                                                                                                                     | 02/05/2026 | 02/05/2026      | https://00003.awsstudygroup.com/                                      |
| 4   | **Amazon VPC - Basic Practice**<br>- Create a VPC.<br>- Create a Public Subnet and Private Subnet.<br>- Create and configure a Route Table.<br>- Attach an Internet Gateway to the VPC.<br>- Test the Internet connection of the Public Subnet.                                                                          | 03/05/2026 | 03/05/2026      | https://00003.awsstudygroup.com/                                      |
| 5   | **Amazon VPC - Advanced Practice**<br>- Create an Elastic IP.<br>- Deploy a NAT Gateway.<br>- Configure a Route Table for the Private Subnet.<br>- Learn about Security Group and Network ACL.<br>- Compare Stateful and Stateless Firewalls.                                                                            | 04/05/2026 | 04/05/2026      | https://00003.awsstudygroup.com/                                      |
| 6   | **Comprehensive Practice**<br>- Complete the Amazon VPC network architecture.<br>- Deploy EC2 in the Public and Private Subnets.<br>- Test SSH, HTTP, and ICMP.<br>- Test Internet access from the Private Subnet through the NAT Gateway.<br>- Review and summarize all Networking Fundamentals and Amazon VPC content. | 05/05/2026 | 06/05/2026      | https://00003.awsstudygroup.com/<br>https://000010.awsstudygroup.com/ |

---

### Week 3 Achievements:

* Understood the fundamental concepts of computer networking, including IP addresses, CIDR, Subnet, TCP/IP, DNS, HTTP/HTTPS, and the principles of data transmission in a Cloud environment.

* Understood network architecture on AWS and the role of Amazon Virtual Private Cloud (Amazon VPC) in building secure network infrastructure.

* Understood and applied the key components of Amazon VPC, including:

  * Virtual Private Cloud (VPC)
  * CIDR Block
  * Public Subnet
  * Private Subnet
  * Route Table
  * Internet Gateway (IGW)
  * NAT Gateway
  * Elastic IP

* Understood the routing mechanism and Internet access flow of EC2 instances in Public Subnets and Private Subnets.

* Successfully deployed an Amazon VPC system with multiple Subnets and fully configured the Internet Gateway, Route Table, and NAT Gateway.

* Distinguished between Security Group and Network ACL and applied them to control network traffic at different security layers.

* Successfully tested and verified the following connections:

  * SSH.
  * HTTP.
  * ICMP (Ping).
  * Internet access from the Public Subnet.
  * Internet access from the Private Subnet through the NAT Gateway.

* Developed the ability to design and deploy AWS network infrastructure based on a Multi-tier Architecture, creating a foundation for advanced topics such as Elastic Load Balancing (ELB), Auto Scaling, Hybrid Networking, and Cloud architectures in the following weeks.
