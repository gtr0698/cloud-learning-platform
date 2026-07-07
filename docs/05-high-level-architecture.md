# High-Level Architecture

| Property | Value                   |
|----------|-------------------------|
| Project | Cloud Learning Platform |
| Document | High-Level Architecture |
| Version | 1.0                     |
| Status | Draft                   |
| Author | Guilherme Taborda       |
| Last Update | 2026-07-07              |

---

# Purpose

This document describes the high-level architecture of the Cloud Learning Platform.

It explains how the system is organized, the major architectural components, and the responsibilities of each layer, independently of implementation details.

---

# Architectural Style

The platform follows a **Modular Monolith** architecture.

Business capabilities are isolated into bounded contexts, allowing future extraction into independent microservices with minimal architectural impact.

---

# Architectural Principles

- Domain-Driven Design (DDD)
- Clean Architecture
- Hexagonal Architecture
- SOLID Principles
- Cloud-Native Design
- Event-Driven Communication (future)
- API First
- Observability by Default
- Security by Design

---

# System Overview

Cloud Learning Platform

├── Frontend (Angular)

│

├── Backend (Spring Boot)

│     ├── Identity

│     ├── Organization

│     ├── Learning

│     ├── Assessment

│     ├── Certification

│     ├── Communication

│     └── Analytics

│

├── PostgreSQL

├── Redis

├── Kafka

└── Object Storage (AWS S3)

---

# Technology Stack

## Frontend

- Angular

## Backend

- Java 21
- Spring Boot 3

## Database

- PostgreSQL

## Cache

- Redis

## Messaging

- Apache Kafka

## Infrastructure

- Docker
- Kubernetes
- Terraform

## Cloud

- AWS

## CI/CD

- GitHub Actions
- ArgoCD

## Observability

- OpenTelemetry
- Prometheus
- Grafana
- Loki
- Tempo

---

# Evolution Strategy

The application starts as a Modular Monolith.

As bounded contexts mature, individual modules may be extracted into independent microservices without significant business impact.

---

# References

- Product Vision
- Domain Model
- Business Workflows
- Bounded Contexts
