# Architecture

```mermaid
flowchart LR
  U[Internet Users] --> WAF[AWS WAFv2]
  WAF --> ALB[Application Load Balancer]
  ALB --> EC2[EC2 Web Server]
  ADMIN[Admin CIDR] --> EC2
