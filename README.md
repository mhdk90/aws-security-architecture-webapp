# AWS Security Architecture for a Two-Tier Web Application

## Overview
This project demonstrates a security-focused AWS web application architecture using an Application Load Balancer, EC2, security groups, and AWS WAFv2.

## Goal
Build a secure web application entry layer with traffic inspection, IP-based blocking, and defense-in-depth controls.

## Current Scope
- VPC
- Public subnets
- Internet-facing Application Load Balancer
- Security groups
- EC2 web server
- AWS WAFv2 Web ACL
- Optional IP-based blocking rules

## Repository Structure
- `cloudformation/` – CloudFormation templates
- `docs/` – architecture, threat model, and deployment notes

## Current Protections
- WAFv2 inspection at the entry layer
- ALB as the public entry point
- Backend restricted by security groups
- Parameterized admin access range

## Planned Hardening
- HTTPS listener with ACM certificate
- CloudFront in front of the ALB
- Auto Scaling Group
- Logging and monitoring enhancements

## Security Notes
- No secrets are stored in this repository
- Environment-specific values are parameterized
- SSH access must be restricted to a narrow CIDR

## Deployment
Add your deploy command here.

## Cleanup
Add your cleanup command here.
