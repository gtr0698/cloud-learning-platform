# Bounded Contexts

| Property | Value                   |
|----------|-------------------------|
| Project | Cloud Learning Platform |
| Document | Bounded Contexts        |
| Version | 1.0                     |
| Status | Draft                   |
| Author | Guilherme Taborda       |
| Last Update | 2026-07-06              |

---

# Purpose

This document identifies the main Bounded Contexts of the platform.

---

# Context 1

## Identity & Access

### Purpose

Responsible for user identity, authentication, authorization and access management.

### Owns

- User
- Role
- Permission
- Invitation
- Authentication
- Password

### Collaborates With

- Organization
- Learning

---

# Context 2

## Organization Management

### Purpose

Responsible for managing customer organizations and their internal structure.

### Owns

- Organization
- Department
- Team

### Collaborates With

- Identity
- Learning

---

# Context 3

## Learning

### Purpose

Responsible for delivering educational experiences.

### Owns

- Course
- Module
- Lesson
- Learning Path
- Enrollment
- Progress

### Collaborates With

- Assessment
- Certification

---

# Context 4

## Assessment

### Purpose

Responsible for evaluating learner knowledge.

### Owns

- Assessment
- Question
- Question Bank
- Submission
- Grade

### Collaborates With

- Learning
- Certification

---

# Context 5

## Certification

### Purpose

Responsible for issuing certificates.

### Owns

- Certificate
- Certificate Template
- Certificate Policy

### Collaborates With

- Learning
- Assessment

---

# Context 6

## Communication

### Purpose

Responsible for all outbound communication.

### Owns

- Email
- Notification
- Template
- Delivery

### Collaborates With

- Everyone

---

# Context 7

## Analytics

### Purpose

Responsible for dashboards and business intelligence.

### Owns

- Reports
- Metrics
- Dashboards
- KPIs

### Collaborates With

- Almost every context.
