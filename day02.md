# AWS Infrastructure Overview - Day 2

## Types of Compute

1. General Computing
   - Amazon EC2
2. GPU Compute
   - Amazon Inferentia
3. Quantum Computing
   - Amazon Braket via California Institute of Technology

## Benefits of Cloud

- Agility
- Pay as you go
- Economy of scale
- Global reach
- Security
- Reliability
- High Availability
- Scalability
- Elasticity
- Fault tolerance
- Disaster Recovery

## AWS Global Infrastructure

### Hierarchy

Regions → Availability Zones (AZs) → Data Centers

### Key Points

- General rule: 1 region has 3 AZs
- Most important region is us-east-1 (North Virginia)

### Region-Independent Services

- IAM - No concept of region
- S3 - A single region must be selected for launch of service
- CloudFront - A group of regions chosen

### Infrastructure Details

- Each data center is isolated and still gets <10ms latency
- High availability means deployment in at least 3 AZs
- Region naming example: us-east-1a
  - 'us-east-1' represents the region
  - 'a' represents the AZ

### PoP (Point of Presence)

- Operated by AWS and its partners
- Used in:
  - CloudFront
  - S3 Transfer Acceleration
