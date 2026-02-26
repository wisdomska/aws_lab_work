# Techora Solutions Company Portal Migration  
**Design and Evaluation Using AWS Well-Architected & Cloud Adoption Frameworks**

Author: **Wisdom Senya Kobla Agbetsiafa**  
Course / Lab: **Cloud Engineering 2**

---

## Overview

This project presents the architectural evaluation and cloud migration strategy for **Techora Solutions' Company Portal**, a two-tier web application transitioning from on-premises infrastructure to **Amazon Web Services (AWS)**.

The solution applies two core AWS frameworks:

- **AWS Well-Architected Framework (WAF)** – for workload quality and design optimization  
- **AWS Cloud Adoption Framework (CAF)** – for organizational readiness and transformation planning

The objective is to design a cloud architecture that is **secure, resilient, scalable, and cost-efficient from day one**.

---

## Existing Architecture Summary

The original system consists of a simple two-tier deployment:

### **Frontend Tier**
- Single web server
- Handles HTTP/HTTPS requests
- Runs on a single physical machine

### **Backend Tier**
- Relational database server
- Stores credentials and application data
- Directly connected to frontend

---

## Identified Risks & Weaknesses

The on-premises design introduces several limitations:

- Single points of failure (no redundancy)
- No automated backup or disaster recovery strategy
- No geographic distribution
- Fixed capacity / no elasticity
- Limited monitoring and visibility
- Inability to handle traffic spikes

---

## AWS Well-Architected Evaluation

The workload was assessed across the **five pillars** of the AWS Well-Architected Framework:

| Pillar | Key Focus |
|--------|-----------|
| **Operational Excellence** | Automation & Infrastructure-as-Code |
| **Security** | Least privilege, encryption, MFA |
| **Reliability** | Multi-AZ, failover, backups |
| **Performance Efficiency** | Right-sizing & caching |
| **Cost Optimization** | Cost visibility & governance |
| **Sustainability** | Energy Efficiency | 

The evaluation identified modernization opportunities using native AWS services such as:

- AWS CloudFormation  
- AWS IAM & AWS KMS  
- Amazon EC2 Auto Scaling  
- Amazon RDS (Multi-AZ)  
- Amazon ElastiCache  
- AWS Cost Explorer & Budgets

---

## Improved AWS Architecture

The redesigned cloud architecture resolves prior risks by introducing:

- High availability across multiple Availability Zones  
- Auto-scaling frontend infrastructure  
- Managed, fault-tolerant database layer  
- Encryption & identity-driven security controls  
- Caching for performance optimization  
- Monitoring & cost governance mechanisms  

Core design principles:

- Eliminate single points of failure  
- Prefer managed services over self-managed infrastructure  
- Automate provisioning and deployments  
- Embed security controls by default

---

## Cloud Adoption Framework (CAF) Insights

Successful migration requires organizational alignment beyond technology.

The CAF evaluation covers six perspectives:

1. **Business** – Value definition & success metrics  
2. **People** – Skills & role transformation  
3. **Governance** – Policies & cost control  
4. **Platform** – AWS-native architecture decisions  
5. **Security** – Identity, logging, protection layers  
6. **Operations** – Monitoring & automation

---

## Key Learning Outcomes

This lab demonstrates:

- How structured frameworks guide cloud design decisions  
- Why cloud migration is both technical and organizational  
- How AWS managed services improve multiple pillars simultaneously  
- The importance of automation, security, and cost visibility  

---

## Document Structure

The full report includes:

- Executive Summary  
- Review of Existing Architecture  
- Well-Architected Framework Evaluation  
- Cloud Adoption Framework Analysis  
- Improved Architecture Design  
- Reflection

---

## Purpose of This Repository

This repository serves as:

- Academic lab submission  
- Cloud architecture case study  
- Reference for AWS migration best practices  
- Demonstration of framework-driven design

---

## License / Usage

This material is provided for **educational and demonstration purposes**.

---

## Author

**Wisdom Senya Kobla Agbetsiafa**  
Cloud Engineering / AWS Architecture Studies
