# Hybrid Data Migration & Storage Integration on AWS

## Overview
This project demonstrates a hybrid data migration pattern from an on-premises NFS source to Amazon S3 using AWS DataSync.

## Goal
Show how large-scale hybrid data transfers can be structured with YAML-based Infrastructure as Code and documented migration patterns.

## Current Scope
- Amazon S3 destination bucket
- IAM role for DataSync access
- AWS DataSync NFS source location
- AWS DataSync S3 destination location
- AWS DataSync task

## Repository Structure
- `cloudformation/` – CloudFormation templates
- `docs/` – architecture and migration notes

## Hybrid Migration Context
This project is designed as part of a broader migration approach that can also include:
- AWS Direct Connect
- AWS Site-to-Site VPN
- AWS Snowball Edge
- AWS Storage Gateway

## Security Notes
- No secrets are stored in this repository
- Environment-specific values are parameterized
- Real enterprise network details are intentionally omitted

## Roadmap
- Add architecture diagram
- Add migration strategy notes
- Add CI workflow
- Add optional VPN foundation template
