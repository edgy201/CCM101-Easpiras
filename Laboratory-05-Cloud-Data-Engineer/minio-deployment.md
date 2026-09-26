\# MinIO S3-Compatible Object Storage Deployment



\## Overview

This document details the configuration and deployment of MinIO S3-compatible object storage on an Ubuntu Linux environment for handling client photos and object assets.



\## Deployment Details

\- \*\*Environment\*\*: Ubuntu Linux Playground (KillerCoda)

\- \*\*Deployment Method\*\*: Direct Binary Installation / Native Execution

\- \*\*Service Address\*\*: `0.0.0.0:9000` (API)

\- \*\*Console Address\*\*: `0.0.0.0:9001` (Web Management UI)

\- \*\*Data Directory\*\*: `/data`



\## Configuration Steps

1\. Configured administrator credentials using environment variables:

&#x20;  - `MINIO\_ROOT\_USER`: `cloudadmin`

&#x20;  - `MINIO\_ROOT\_PASSWORD`: `CloudNova2026!`

2\. Executed MinIO server process listening on all interfaces (`0.0.0.0`) to enable network forwarding.

3\. Accessed the MinIO Web Console on port `9001` using port forwarding.

4\. Created an S3-compatible object bucket named `client-photos` for storing photo files.



\## Screenshots

1\. \*\*MinIO Process Running\*\*: `screenshots/minio-deployed.png`

2\. \*\*`client-photos` Bucket Created\*\*: `screenshots/minio-bucket-created.png`

