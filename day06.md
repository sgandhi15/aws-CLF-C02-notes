# Cost and Capacity Management Computing Services

## How We Save Money

1. Spot Instances & Reserved Instances
2. AWS Batch - Execute batch workloads across full range of AWS compute services. Can utilize spot instances
3. AWS Compute Optimizer - Use machine learning to optimize your workloads
4. EC2 Auto Scaling Groups - Automatically scale up or down based on workloads
5. Elastic Load Balancing - Load balancer for EC2 instances
6. Elastic Beanstalk - AWS managed service for running and scaling web applications

## Types of Storage Drive

1. EBS - Elastic Block Store - For VM storage
2. EFS - Elastic File System - For NFS file storage or sharing across multiple VMs
3. S3 - Simple Storage Service - For file storage and object storage

## S3

- Data stored as objects
- Provides unlimited scalability
- S3 buckets are global
  - Can be accessed from anywhere in the world
  - Holds S3 objects
- S3 objects contain:
  - Key
  - Value
  - Metadata
  - Version ID

### S3 Storage Classes (Higher to Lower Pricing)

1. Standard - Fast, 99.99% availability, 11 9's durability, replication across 3 AZs at least
2. Intelligent-Tiering - Uses ML to automatically move data between storage classes
3. Standard-IA - Fast but cheaper if file access is less than once per month
4. One Zone-IA - Fast but only exists in one AZ
5. Glacier - Long-term storage, retrieval can take longer than standard
6. Glacier Deep Archive - Long-term storage, retrieval can take 12 hours

### Snow Family - For Physically Moving Data to Cloud

- When moving data to cloud is slow, difficult, and costly
- Stores data later in S3

1. Snowcone - Two sizes: 8TB for HDD, 14TB for SSD
2. Snowball Edge - Two sizes: Storage optimized (80TB) and Compute optimized (39.5TB)
3. Snowmobile - Up to 100PB

### Storage Services

1. S3 - Simple Storage Service
2. S3 Glacier - Long-term storage
3. Elastic Block Store - For VM storage
4. Elastic File Storage - Cloud native NFS file system service
5. Storage Gateway - Hybrid cloud storage
   - Extends on-premise storage to cloud storage
   - File Gateway - Extend local storage to S3
   - Volume Gateway - Caches local drives to S3 for backup
   - Tape Gateway - Stores files on virtual tapes for backup for cost-effective long-term storage
6. Snow Family - Physical migration of data to cloud
7. AWS Backup - Fully managed backup service
8. CloudEndure Disaster Recovery - Fully managed disaster recovery service
   - Backup all machines to low-cost staging area and account
9. Amazon FSx - Feature-rich and highly performant file system
   - FSx for Windows File System - Uses SMB protocol
   - FSx for Lustre - Uses Lustre protocol for Linux file system

---

Important Notes:

- Can only have 100 buckets max
- EFS can connect to many machines via Network File System
- Snow Family only available in United States as service

---

## Database

### Types

- SQL and NoSQL
- Data Warehouse - Relational datastore for analytics
  - Generally performs aggregation
    - Aggregation is grouping data
    - Optimized around columns
  - Designed to be HOT - can return data really fast with vast amounts of data
  - Designed for infrequent access as reports are typically generated once a day

### NoSQL

- Simple and fast
- Key and value based
- Can have columns by using arrays and scales well beyond SQL
- Lacks indexes, aggregation, relationships

### Document Stores

- NoSQL but stores documents with keys like JSON and XML
- Subclass of key-value store
- Can have index and joins based on linking and embedding
- Can be similar to SQL in terms of offerings

### AWS Database Services

DynamoDB - Amazon's flagship NoSQL key-value pair document DB

- Fact: In 2019, Amazon Shopping shutdown their last Oracle database and migrated to DynamoDB. They had 7,500 Oracle DBs and 75 petabytes of data, reducing costs by 60% and latency by 40%

DocumentDB - MongoDB compatible NoSQL document DB
Amazon Keyspaces - Fully managed Apache Cassandra (open-source NoSQL key/value DB with additional functionality)

### Relational Database Service (RDS)

- Supports multiple SQL engines:
  - MySQL
  - MariaDB
  - PostgreSQL
  - Oracle SQL
  - Microsoft SQL Server

Aurora

- Fully managed DB supporting PostgreSQL or MySQL only
- Aurora Serverless available for low traffic scenarios (more cost-effective)

RDS on VMware - Allows deployment of RDS-supported engines on-premises (requires VMware for server virtualization)

### Other Database Services

1. Redshift - Petabyte-scale warehouse
2. ElastiCache - Managed Redis or Memcached
3. Neptune - Managed graph DB
4. Amazon Timestream - Fully managed time series DB for time-sensitive operations
5. Amazon Quantum Ledger Database - Fully managed ledger database providing transparent, immutable, and cryptographically verifiable transaction log (important for financial institutions)
6. Database Migration Service
