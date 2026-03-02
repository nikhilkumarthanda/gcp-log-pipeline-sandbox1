# gcp-log-pipeline-sandbox1
End-to-end GCP data pipeline (Pub/Sub → Beam → BigQuery → Looker Studio Dashboard).

GCP Log Processing Pipeline

Overview

This project demonstrates the design and implementation of a scalable, cloud-native log processing pipeline using Google Cloud Platform (GCP).

The pipeline ingests structured log data, processes it automatically, and stores it for analytical querying using BigQuery.

The focus of this project is system design, scalability, automation, and cost-efficient architecture — not just data movement.

⸻

Architecture

Components Used
	•	Google Cloud Storage (GCS) – Raw log ingestion layer
	•	Cloud Functions – Event-driven processing
	•	Pub/Sub (Optional / if used) – Asynchronous message handling
	•	BigQuery – Scalable analytics and structured querying
	•	IAM & Monitoring – Security and observability

⸻

Pipeline Flow
	1.	Log files are uploaded to Cloud Storage.
	2.	A Cloud Function is triggered automatically.
	3.	Logs are validated and transformed.
	4.	Processed data is loaded into BigQuery.
	5.	Data becomes available for analytics and dashboarding.

⸻

Key Design Considerations
	•	Event-driven architecture
	•	Serverless compute to reduce infrastructure overhead
	•	Modular transformation logic
	•	Scalable storage & querying
	•	Cost-optimized resource usage

⸻

Scalability

The pipeline is designed to:
	•	Handle increasing log volumes
	•	Process files asynchronously
	•	Scale automatically with serverless architecture
	•	Support future integration with ML models or dashboards

⸻

Potential Extensions
	•	Real-time streaming with Dataflow
	•	Error-handling and dead-letter queues
	•	Integration with Looker Studio dashboards
	•	ML-based anomaly detection on logs
