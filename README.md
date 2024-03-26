# vpc-peering-aws
### Overview
This README provides information and guidelines for setting up and managing VPC peering connections within your AWS (Amazon Web Services) environment.

### Introduction
VPC peering allows you to connect two VPCs (Virtual Private Clouds) so that instances in one VPC can communicate with instances in the other VPC using private IP addresses.

### Prerequisites
AWS account with appropriate permissions to create and manage VPC peering connections.
Basic understanding of VPC concepts and networking in AWS.
VPCs with non-overlapping CIDR blocks.

### Setting Up VPC Peering
Navigate to the VPC Dashboard: Go to the AWS Management Console and open the VPC dashboard.
![AWS Logo](https://github.com/NimishRathi/vpc-peering-aws/blob/main/Screenshot%202024-03-26%20003026.png)
![AWS Logo](https://github.com/NimishRathi/vpc-peering-aws/blob/main/Screenshot%202024-03-26%20003012.png)


Create Peering Connection: Click on "Peering Connections" in the navigation pane and then click "Create Peering Connection".
![AWS Logo](https://github.com/NimishRathi/vpc-peering-aws/blob/main/Screenshot%202024-03-26%20002956.png)


Configure Peering Connection: Enter the necessary details such as the VPC you want to peer with, VPC peering connection name, and any optional settings.


Accept Peering Connection: Once the peering connection is created, navigate to the other VPC's peering connections and accept the pending request.
![AWS Logo](https://github.com/NimishRathi/vpc-peering-aws/blob/main/Screenshot%202024-03-26%20002841.png)


![AWS Logo](https://github.com/NimishRathi/vpc-peering-aws/blob/main/Screenshot%202024-03-26%20002819.png)



Update Route Tables: Update the route tables in each VPC to route traffic destined for the other VPC's CIDR block through the peering connection.
![AWS Logo](https://github.com/NimishRathi/Jump-Hosting-AWS/blob/main/Screenshot%202024-03-20%20154103.png)

now launch two ec2 in both the vpc and try to connect the intances  



