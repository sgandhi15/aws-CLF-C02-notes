# AWS Infrastructure and Services

## Network and Connectivity

- **AWS Direct Connect** - Dedicated service for high-speed and low-latency connections

- **AWS Local Zones** - Located in dense cities in data centers for ultra-low latency connection

  - Example: us-west-2-lax-1a
    - lax-1a is the local zone identifier

- **AWS Wavelength** - 5G edge computing service

- **AWS Outposts** - AWS managed service for on-premises

## Governance and Compliance

- **AWS Config** - Policy as code for AWS

- **AWS GovCloud** - Dedicated regions for US government

- **AWS China** - Separate and independent from global AWS

## Sustainability

Amazon plans to achieve Net-zero carbon emissions by 2040, including AWS, through:

- Renewable energy
- Cloud efficiency
- Water stewardship

## Specialized Services

- **AWS Ground Station** - For satellite data and communication

## Cloud Architecture Terminology

### Solution Architect / Cloud Architect

Key concepts to understand:

- **Availability**
  - Elastic Load Balancer
- **Scalability**
  1. Vertical Scaling - Adding more resources to existing server
  2. Horizontal Scaling - Adding more servers
- **Elasticity**
  - Works with horizontal scaling
  - Auto Scaling Groups
- **Fault Tolerance**
  - Having multiple copies
  - Multi-AZ RDS
- **High Availability**
- **Disaster Recovery**
  - High durability
  - AWS CloudEndure
- **Security**
- **Cost**

## AWS Interaction Methods

1. API
2. CLI
3. Management Console
4. SDK
5. CDK

## Account Management

### AWS Account ID

- Keep private
- Manages various AWS services
- Handles support
- Controls roles and policies

## Command Line Tools

- AWS CloudShell supports:
  - PowerShell
  - Bash
  - Zsh

## Resource Management

### ARNs (Amazon Resource Names)

- Used for:
  - APIs
  - Policies
  - IAM rules restrictions
  - Specific AWS resource identification

### AWS CLI

Supports multiple shells:

- PowerShell
- Bash
- Zsh
