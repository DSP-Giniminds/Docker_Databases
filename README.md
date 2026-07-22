# Docker_Databases

This repository contains Docker-based automated deployment scripts
for DSP Platform databases using Ansible and Jenkins.


## About This Repository

Each branch in this repository represents one database deployment.
The branch name indicates which database it contains along with
its complete Ansible scripts, configuration and Jenkinsfile.


## Branch Structure

| Branch   | Database      | Version | Port(s)    |
|----------|---------------|---------|------------|
| oracle   | Oracle XE     | 21c     | 1521, 5500 |
| postgres | PostgreSQL    | 18      | 5050, 8888 |
| mssql    | MS SQL Server | 2022    | 1433       |
| minio    | MinIO         | latest  | 9000, 9001 |
| ibmmq    | IBM MQ        | latest  | 1414, 9443 |


## Deployment

All databases are deployed on Docker 
and automated through Jenkins.


## Each Branch Contains

- inventory                  → Target server configuration
- ansible.cfg                → Ansible settings
- deploy_app.yml             → Main deployment playbook
- roles/app/tasks/main.yml   → All deployment steps
- roles/app/vars/main.yml    → Config values (image, ports, passwords)
- Jenkinsfile                → Jenkins pipeline for automated deployment
