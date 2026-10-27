# Kubernetes RoboShop

This repository contains Kubernetes manifests for deploying the RoboShop application in a cluster. It is organized by service and demonstrates how a multi-service application can be represented as Deployments, Services, and supporting K8s objects.

## Project Purpose

The goal of this repo is to show practical Kubernetes deployment patterns for a microservices-based application, including:

- workload deployment via Kubernetes resources
- service-to-service communication
- application configuration and environment variables
- modular service organization
- cluster-friendly deployment structure

## Application Components

The stack includes the following service folders:

- `cart`
- `catalogue`
- `frontend`
- `mongodb`
- `mysql`
- `payment`
- `rabbitmq`
- `redis`
- `shipping`
- `user`
- `debug`

## Typical Structure

```bash
.
├── README.md
├── cart/
├── catalogue/
├── frontend/
├── mongodb/
├── mysql/
├── payment/
├── rabbitmq/
├── redis/
├── shipping/
├── user/
├── debug/
```

## Why This Repo Matters

This is a strong example of Kubernetes application deployment work. It represents the next layer above containerization and infrastructure provisioning, showing how application services can be deployed, exposed, and managed in a cluster environment.

## Related Work

- [roboshop-docker](https://github.com/dasariravi145/roboshop-docker) — containerized local deployment using Docker Compose
- [roboshop-infra-eks](https://github.com/dasariravi145/roboshop-infra-eks) — AWS EKS infrastructure provisioning
- [roboshop-ansible](https://github.com/dasariravi145/roboshop-ansible) — infrastructure automation with Ansible
- [ansible-roboshop-roles](https://github.com/dasariravi145/ansible-roboshop-roles) — role-based application automation

## Suggested Next Steps

- add namespace definitions
- document service dependencies and traffic flow
- add ingress and external access configuration
- add health checks and readiness probes
- include deployment commands and validation steps

## Notes

This repo is a portfolio-quality Kubernetes workload example that complements the Docker, Terraform, and Ansible repos in the same RoboShop deployment series.
