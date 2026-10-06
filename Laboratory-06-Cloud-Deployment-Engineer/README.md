\# Laboratory Activity 6: The Cloud Deployment Engineer



\## Mission Overview

This laboratory activity focuses on transitioning from manual container deployment to Infrastructure as Code (IaC) using Docker Compose. A two-tier private cloud storage solution (Nextcloud and MariaDB) was defined and deployed automatically via a YAML configuration blueprint on Ubuntu Linux.



\## Objectives

\- Explain multi-tier application architecture principles.

\- Construct and configure a `docker-compose.yml` deployment file.

\- Deploy and manage multi-container application stacks using Docker Compose.

\- Expose and test private cloud web applications over specific web ports.

\- Document deployment procedures and IaC concepts using Markdown.



\## Commands Executed

```bash

mkdir nextcloud-deployment \&\& cd nextcloud-deployment

nano docker-compose.yml

docker-compose up -d

docker-compose ps

docker-compose down



