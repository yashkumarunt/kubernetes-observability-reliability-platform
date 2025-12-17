# Kubernetes Observability & Reliability Platform

## Overview
This project demonstrates a containerized microservices platform deployed on Kubernetes with a focus on observability, auto-scaling, and reliability.

The platform uses Prometheus for metrics collection and Grafana for visualization to monitor application health, performance, and scaling behavior. It is designed to be fault-tolerant, self-healing, and scalable under load.

---

## Architecture
Components:
- API Service (Python)
- Frontend Service
- Redis
- Kubernetes
- Helm
- Prometheus
- Grafana
- Horizontal Pod Autoscaler (HPA)
- AWS (optional)

**Flow:**
User → Frontend → API → Redis
↓
Prometheus → Grafana


---

## Goals
- Containerize microservices using Docker
- Deploy workloads using Kubernetes
- Use Helm for repeatable deployments
- Implement health checks (liveness & readiness)
- Enable horizontal auto-scaling
- Monitor metrics using Prometheus
- Visualize metrics using Grafana
- Demonstrate self-healing behavior

---

## Tech Stack
- Docker
- Kubernetes
- Helm
- Prometheus
- Grafana
- Python
- AWS (EKS, ECR – optional)

---

## Repository Structure
kubernetes-observability-reliability-platform/
├── services/
│ ├── api/
│ └── frontend/
├── k8s/
├── charts/
├── dashboards/
├── scripts/
└── README.md


---

## Observability
- Prometheus scrapes metrics from the API
- Grafana dashboards display:
  - Request rate
  - CPU and memory usage
  - Pod count and restarts

---

## Reliability & Scaling
- Liveness probes restart unhealthy containers
- Readiness probes control traffic flow
- HPA scales API pods based on CPU usage
- Kubernetes automatically recreates failed pods

---

## Demo Scenarios
- Load testing triggers auto-scaling
- Pod failure demonstrates self-healing
- Metrics visible in Grafana dashboards

---

## Status
Work in progress. Built incrementally for learning and interview demonstration.

---

## License
MIT
