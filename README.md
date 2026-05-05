# AWS Serverless Data Architecture - Cost Reduction Implementation

![AWS](https://img.shields.io/badge/AWS-Serverless-orange?logo=amazon-aws)

## Company
Abstergo Industries (fictional project for DIO Bootcamp)

## Objective
Design a 100% serverless AWS architecture to reduce immediate infrastructure costs, moving away from a traditional server-based model.

## Architecture

| Layer | AWS Service | Purpose |
|-------|-------------|---------|
| **Storage** | Amazon S3 (Intelligent-Tiering) | Scalable, cost-effective data lake |
| **Catalog & ETL** | AWS Glue | Serverless data preparation and cataloging |
| **Analytics** | Amazon Athena | SQL-based business intelligence directly on S3 data |

## Key Outcomes
- **Zero Fixed Server Costs**: Computation is billed only per query or job execution.
- **Security**: AES-256 encryption at rest and IAM for granular access control.
- **Compliance**: Full alignment with LGPD (Brazilian General Data Protection Law) requirements.
