# Optimizing a cloud architecture

Imagine you own a bustling online florist business, with orders flowing in during peak times like Valentine’s Day or Mother’s Day. Behind the scenes, the cloud architecture needs to be just as resilient and efficient as the operations. Let’s use the Well-Architected Framework to optimize the system for reliability, performance, security, cost savings, and sustainability.


## Step 1: Starting architecture

<img width="4917" height="2877" alt="image" src="https://github.com/user-attachments/assets/54dc4826-3ac8-4782-9d04-9922ef856257" />

Let’s look at your current setup. You have a classic ecommerce architecture. It includes Amazon Elastic Compute Cloud (Amazon EC2) instances for the website and Amazon Relational Database Service (Amazon RDS) databases to handle orders and customer data. It also has an Amazon Simple Storage Service (Amazon S3) bucket full of product images. It’s functional, but let's evaluate how well it's scaling and handling traffic—especially during busy times.

----

## Step 2: Operational Excellence

<img width="4964" height="2668" alt="image" src="https://github.com/user-attachments/assets/ce8259d8-cc86-4754-b2dc-25cd6440fd79" />

Your business is running smoothly, but what happens if an EC2 instance crashes during a rush of orders? To be truly resilient, you can automate scaling with EC2 Auto Scaling. Additionally, to make day to day operations more reliable and efficient, you can use infrastructure as code and implement self healing mechanisms like auto-rollback. These practices help your system adapt during high-demand periods as well as operate efficiently over time.

**Enhancement:** EC2 Auto Scaling

----
## Step 3: Security

<img width="4964" height="2822" alt="image" src="https://github.com/user-attachments/assets/aca9a46f-5b6c-43d6-9d5d-21be563265b8" />

You’ve already got a secure foundation with an Amazon Virtual Private Cloud (Amazon VPC), but there’s more to do. Ask yourself: Are your EC2 instances regularly patched? Do your IAM policies follow the principle of least privilege? Protecting customer data—like names, addresses, and payment info—requires strong encryption for data at rest and in transit, along with fine-grained access controls. Strengthening these layers builds trust with your customers and safeguards sensitive information.

**Enhancement:** Strengthening encryption and IAM policies

----
## Step 4: Reliability

<img width="4964" height="2822" alt="image" src="https://github.com/user-attachments/assets/8d4e2e9d-43ee-4c03-a94d-044738b37c7e" />

During busy seasons, availability is everything. You’ve already taken a great step by deploying resources across multiple Availability Zones, but you can increase reliability even further. Use Amazon CloudWatch to monitor your system’s health and set up automated recovery actions.

**Enhancement:** Amazon CloudWatch

----
## Step 5: Performance Efficiency

<img width="4964" height="2822" alt="image" src="https://github.com/user-attachments/assets/a603cdce-38d7-4163-ad74-55ef0467117c" />

As your business scales, your system should scale with it. Are your EC2 instances and RDS instances rightsized for your workload? AWS Compute Optimizer can help make sure you’re not wasting resources or underprovisioning your infrastructure. You’re already using AWS Lambda for event-driven tasks like image processing, which is great for flexible scaling. Make sure those functions are rightsized, too. And with Amazon CloudFront, you can already deliver product images quickly to global customers for a smooth, fast shopping experience.

**Enhancement**: AWS Compute Optimizer

---
## Step 6: Cost Optimization

<img width="4964" height="2940" alt="image" src="https://github.com/user-attachments/assets/119858dd-e545-402a-bf13-ea05d10caedd" />

You're currently using On-Demand EC2 instances, which are great to start with, but switching to Spot Instances for variable traffic and Savings Plans for steady workloads can cut costs significantly. Track and manage your cloud spending in real time with AWS Budgets and AWS Cost Explorer. These tools help you make smart, cost-effective decisions while maintaining performance and reliability.

**Enhancement**: Savings Plans, AWS Budgets, AWS Cost Explorer

-----

# Step 7: Sustainability

<img width="4964" height="2958" alt="image" src="https://github.com/user-attachments/assets/74836e64-397f-4e80-b3c4-0b3c9f233d87" />

Your use of serverless and elastic resources already reduces your environmental footprint. To go further, continue optimizing workloads to minimize resource waste. Doing so benefits both the planet and your bottom line—proving that environmentally conscious decisions can also be business-smart.

**Enhancement**: AWS Cost & Usage Report

----
# Final cloud architecture

<img width="4862" height="2911" alt="image" src="https://github.com/user-attachments/assets/30e61c92-bf88-4391-9ad7-acb5c2e2eab1" />



















