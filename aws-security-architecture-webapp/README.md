# AWS Security Architecture for a Two-Tier Web Application

## Overview
This project demonstrates a security-focused AWS web application architecture using an Application Load Balancer, EC2, security groups, and AWS WAF.

## Goal
Build a secure web application entry layer with traffic inspection, IP-based blocking, and defense-in-depth controls.

## Current Scope
- VPC
- Public subnets
- Internet-facing Application Load Balancer
- Security groups
- EC2 web server
- AWS WAF IP set
- AWS WAF Web ACL
- Web ACL association with ALB

## Files
- `cloudformation/secure-webapp.yaml` – CloudFormation YAML template
- `docs/` – notes and later diagrams

## Services Covered
- Amazon VPC
- Amazon EC2
- Application Load Balancer
- AWS WAF
- Security Groups

## Planned Next Steps
- Add CloudFront in front of the ALB
- Document AWS Shield Standard in the architecture notes
- Add HTTPS listener and ACM certificate
- Add Lambda-based automation for log or response workflows
- Add Auto Scaling Group

## What I Learned
- How to define web security controls in CloudFormation YAML
- How to restrict web-tier access through security groups
- How to attach AWS WAF protection to an ALB
- How to present security architecture clearly on GitHub