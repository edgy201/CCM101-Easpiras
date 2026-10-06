\# Infrastructure as Code: Docker Compose Deployment Guide



\## Purpose of `services:` Block

The `services:` block defines the distinct containers that make up the multi-tier application stack. In this deployment, it declares two separate services (`database` and `app`), specifying their Docker images, port bindings, environment variables, and network relations.



\## Container Service Discovery

The Nextcloud container locates the database container using the environment variable `MYSQL\_HOST=database`. Docker Compose creates a default internal bridge network where service names act as DNS hostnames, allowing the `app` container to resolve `database` directly to its internal IP address.



\## `docker run` vs. `docker-compose up -d`

\- `docker run`: Executes a single container manually with command-line flags. Managing complex multi-container apps requires long, repetitive CLI commands.

\- `docker-compose up -d`: Deploys and orchestrates multiple interconnected containers in detached mode using a single declarative YAML blueprint file (`docker-compose.yml`).

