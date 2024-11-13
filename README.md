# Heart-Disease-Monitoring-and-Analysis---Real-Time-and-Batch-Data-Processing-in-AWS-Cloud

**Project Overview:** This project aims to build a comprehensive system for heart disease monitoring and analysis on the AWS Cloud, utilizing real-time and batch data processing. The solution helps healthcare providers manage patient data, gain insights, and receive timely alerts, ultimately improving patient care and proactive health management.

**Key Components:**

**Batch Data Processing:**

Patient data from PostgreSQL is ingested using AWS Lambda, stored in Amazon S3, and transformed using AWS Glue.
Data is organized in layers (Raw, Staging, Curated) and cataloged for easy access and querying via Amazon Athena.

**Real-Time Data Processing:**

Health data from wearables is ingested with AWS Kinesis and processed by AWS Lambda, storing results in DynamoDB for quick access.
Alerts are generated using Amazon SNS and CloudWatch for threshold-based health events.

**Data Warehousing with Amazon Redshift:**

Data is stored using a star schema, with fact tables for health metrics and dimension tables for demographics, health conditions, and lifestyle.
This design supports efficient querying and reporting for heart disease analysis.

**Technologies Used:**

**AWS Lambda:** Orchestrates both batch and real-time data ingestion.
**Amazon Kinesis:** Streams real-time data from wearable devices.
**AWS Glue:** ETL, data transformation, and cataloging for batch data.
**Amazon S3:** Stores raw, processed, and curated data layers.
**Amazon Redshift:** Data warehousing for efficient analytics and reporting.
**Amazon DynamoDB:** Stores real-time data with fast, scalable access.
**Amazon Athena:** Serverless SQL querying for data in S3.
**Amazon QuickSight:** Visualization tool for interactive dashboards and insights.
**Amazon SNS and CloudWatch:** Delivers real-time alerts and monitors system health.

**Project Objectives:**

Implement a cloud-based, dual-mode (real-time and batch) system for heart disease monitoring.

Provide analytical insights to help healthcare professionals take proactive action.

Generate real-time alerts for critical health events, improving patient care.
