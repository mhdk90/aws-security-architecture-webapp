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
- AWS WAFv2 Web ACL
- Optional IP blocking rules

## Repository Structure
- `cloudformation/` – CloudFormation YAML templates
- `docs/` – notes and architecture explanations

## Security Notes
- No secrets are stored in this repository
- Environment-specific values should be passed as parameters
- SSH access should be restricted to a narrow admin CIDR, not open to the world

## Planned Next Steps
- Add HTTPS listener and ACM certificate
- Add CloudFront in front of the ALB
- Add Auto Scaling Group
- Add architecture diagram
- Add logging and monitoring notes

## What I Learned
- How to define web security controls in CloudFormation YAML
- How to protect an ALB-backed application with AWS WAF
- How to use defense-in-depth in AWS architecture
- How to present security architecture clearly on GitHub
