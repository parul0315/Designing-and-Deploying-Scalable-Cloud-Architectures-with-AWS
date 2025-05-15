# Designing-and-Deploying-Scalable-Cloud-Architectures-with-AWS

This repository documents two complete AWS architectures developed to address real-world challenges in availability, scalability, and performance optimization. The project was executed as part of a postgraduate Cloud Computing course and simulates production-grade design using AWS best practices.

---

## Project Overview

The project is divided into two core systems:

### 1. **MyTravel – Scalable Travel Blogging Platform**
A cloud-native architecture built for a global blogging site. It emphasizes low-latency access, fault tolerance, data protection, and automated alerts for user engagement milestones.

### 2. **WordFreq – Auto-Scaling Word Frequency Application**
A distributed system designed for dynamic text processing. It uses message queues and compute autoscaling to handle varying workloads, with performance tuning across EC2 instance types.

---

## Architecture Summary

### MyTravel

- **Content Delivery:** Amazon Route 53 + CloudFront for global low-latency access
- **Static Assets:** Amazon S3 with versioning and AWS Backup
- **Notifications:** CloudWatch triggers Lambda + SNS for user milestone alerts
- **Security:** AWS WAF, IAM roles, and Trusted Advisor for monitoring and compliance
- **Disaster Recovery:** Backup, regional redundancy, and failover

### WordFreq

- **Workload Queueing:** Amazon SQS used as input trigger and scaling metric
- **Compute Layer:** EC2 Auto Scaling Group based on SQS queue depth
- **Storage:** Input via S3, output to DynamoDB
- **Performance Tuning:** Tested across `t2.micro`, `t2.medium`, and `t2.large` EC2 instances
- **Monitoring:** CloudWatch alarms and metrics used to optimize scaling and performance

---

## Technologies & Services Used

- **Compute:** Amazon EC2, Auto Scaling
- **Storage:** Amazon S3, Amazon DynamoDB
- **Networking & Delivery:** Route 53, AWS CloudFront
- **Messaging & Orchestration:** Amazon SQS, SNS, AWS Lambda
- **Monitoring & Management:** Amazon CloudWatch, Trusted Advisor
- **Security:** AWS IAM, AWS WAF
- **DevOps Tools:** AMI creation, launch templates, dynamic scaling policies

---

## Performance & Results

- **WordFreq** demonstrated robust horizontal scalability using dynamic EC2 scaling.
- Load testing validated optimal performance using `t2.medium` and `t2.large` instances under varying loads.
- **MyTravel** achieved highly available, secure content delivery with event-based alerting via serverless components.
- Disaster recovery and cost-efficiency principles were applied to both systems.

---


---

## Key Learnings

- Designed event-driven, scalable, and secure architectures on AWS
- Implemented auto-recovery and performance tuning mechanisms
- Evaluated infrastructure designs through simulated testing and benchmarking
- Practiced cloud cost optimization, security, and monitoring best practices

---

---

## Author

Developed as part of a postgraduate Cloud Computing coursework project simulating production-grade AWS architecture.

**Parul Nagar**  
Email: parulnagar1245@gmail.com  
LinkedIn: [www.linkedin.com/in/parul-nagar-244894202](https://www.linkedin.com/in/parul-nagar-244894202)

---

## Let's Connect

I'm always open to feedback, collaboration, or discussion on cloud architecture, scalable systems, or performance optimization.

Feel free to connect with me on LinkedIn or reach out via email. Feedback is welcome!




