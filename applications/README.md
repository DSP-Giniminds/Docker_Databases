# Infrastructure & Platform Services

This repository serves as a centralized collection of deployment resources for the infrastructure services. It contains configurations and deployment assets for databases, messaging platforms, stream processing frameworks, monitoring tools, object storage, logging solutions, and integration platforms.

Each application is organized in its own folder, allowing it to be managed and deployed independently. The repository provides a consistent structure for maintaining infrastructure components and simplifies access to the deployment resources for each platform.

---

# Repository Structure

```text
Infrastructure-Services/
│
├── applications/
│   ├── clickhouse/
│   ├── confluentflink/
│   ├── elk/
│   ├── flink/
│   ├── ibmmq/
│   ├── kafka/
│   ├── minio/
│   ├── mssql/
│   ├── oracle/
│   ├── pg/
│   ├── postgres/
│   ├── vault/
│   └── webmethods/
│
└── README.md
```

---

# Available Applications

| Application       | Folder                        | Purpose                                                                                         |
| ----------------- | ----------------------------- | ----------------------------------------------------------------------------------------------- |
| ClickHouse        | `applications/clickhouse`     | Column-oriented analytical database for high-performance analytics workloads.                   |
| Confluent + Flink | `applications/confluentflink` | Apache Kafka (Confluent Platform) integrated with Apache Flink for real-time stream processing. |
| ELK Stack         | `applications/elk`            | Elasticsearch, Logstash, and Kibana for centralized logging and log visualization.              |
| Apache Flink      | `applications/flink`          | Distributed stream processing framework for real-time data processing.                          |
| IBM MQ            | `applications/ibmmq`          | Enterprise messaging platform for secure and reliable message delivery.                         |
| Kafka             | `applications/kafka`          | Apache Kafka platform for distributed event streaming and messaging.                            |
| MinIO             | `applications/minio`          | S3-compatible object storage service for storing unstructured data.                             |
| MSSQL             | `applications/mssql`          | Microsoft SQL Server 2022 relational database.                                                  |
| Oracle            | `applications/oracle`         | Oracle Database XE deployment.                                                                  |
| PostgreSQL        | `applications/postgres`       | Standalone PostgreSQL database deployment.                                                      |
| Vault             | `applications/vault`          | HashiCorp Vault for secure secrets and credential management.                                   |
| webMethods        | `applications/webmethods`     | Software AG webMethods Integration Server and API Gateway.                                      |

---

# Branch Structure

| Branch     | Platform             | Version |
| ---------- | -------------------- | ------- |
| `oracle`   | Oracle XE            | 21c     |
| `postgres` | PostgreSQL           | 18      |
| `mssql`    | Microsoft SQL Server | 2022    |
| `minio`    | MinIO                | Latest  |
| `ibmmq`    | IBM MQ               | Latest  |

---

# Service Access

| Platform                 | Access URL / Endpoint      |
| ------------------------ | -------------------------- |
| Oracle XE                | `localhost:1521/XEPDB1`    |
| PostgreSQL               | `http://10.10.20.32:8888`  |
| Microsoft SQL Server     | `localhost:1433`           |
| MinIO Console            | `http://10.10.20.32:9001`  |
| Kafka Broker             | `localhost:9092`           |
| Confluent Control Center | `http://10.10.20.32:9021`  |
| Apache Flink Dashboard   | `http://10.10.20.32:8081`  |
| ClickHouse               | `http://10.10.20.32:8123`  |
| Elasticsearch            | `http://10.10.20.32:9200`  |
| Kibana                   | `http://10.10.20.32:5601`  |
| Grafana                  | `http://10.10.20.32:3000`  |
| Prometheus               | `http://10.10.20.32:9090`  |
| IBM MQ Console           | `https://10.10.20.32:9443` |
| Vault                    | `http://10.10.20.32:8200`  |
| webMethods               | `http://10.10.20.32:5555`  |

