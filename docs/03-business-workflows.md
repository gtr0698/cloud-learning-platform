# Business Workflows

| Property | Value                   |
|----------|-------------------------|
| Project | Cloud Learning Platform |
| Document | Business Workflows      |
| Version | 1.0                     |
| Status | Draft                   |
| Author | Guilherme Taborda       |
| Last Update | 2026-07-04              |

---

# Purpose

This document describes the main business workflows supported by the Cloud Learning Platform.

The objective is to document how business processes occur from the user's perspective, independently of technical implementation.

These workflows will serve as the foundation for use cases, APIs, domain events and software architecture.

---

# 1. Organization Onboarding

## Purpose

Allow a new organization to subscribe to the platform and perform its initial configuration.

## Primary Actors

- Platform Administrator
- Organization Administrator
- System

## Business Flow

1. Platform Administrator creates a new Organization.
2. The System creates the Organization workspace.
3. The System creates the initial Organization Administrator account.
4. The System sends an invitation email.
5. The Organization Administrator accepts the invitation.
6. The Organization Administrator activates the account.
7. The Organization Administrator configures the Organization.
8. The Organization becomes Active.

## Expected Outcome

The organization is ready to start using the platform.

---

# 2. Organization Member Invitation

## Purpose

Allow an organization to invite new members to access the platform.

## Primary Actors

- Organization Administrator
- Invited Member
- System

## Business Flow

1. The Organization Administrator registers a new member using basic information (e.g. full name and email address).
2. The Organization Administrator assigns one or more roles to the invited member.
3. The System validates the provided information.
4. The System generates an invitation.
5. The System sends an invitation email.
6. The invited member accepts the invitation.
7. The invited member completes the registration process and creates a password.
8. The account becomes Active.

## Expected Outcome

The invited member can access the platform with the assigned roles.

---

# 3. Course Creation

## Purpose

Allow instructors to create structured learning experiences.

## Primary Actors

- Instructor

## Business Flow

1. The Instructor creates a new Course.
2. The Instructor defines the course information.
3. The Instructor creates Modules.
4. The Instructor creates Lessons.
5. The Instructor uploads learning resources.
6. The Instructor creates Assessments.
7. The Instructor publishes the Course.

## Expected Outcome

The course becomes available for enrollment.

---

# 4. Learning Assignment

## Purpose

Assign mandatory or optional learning content to employees.

## Primary Actors

- Manager
- Employee

## Business Flow

1. The Manager selects a Learning Path.
2. The Manager selects one or more Employees.
3. The Learning Path is assigned.
4. Employees receive a notification.
5. Employees start the learning process.

## Expected Outcome

Employees have access to their assigned learning content.

---

# 5. Learning Completion

## Purpose

Track the employee's progress until course completion.

## Primary Actors

- Employee
- System

## Business Flow

1. Employee starts the Course.
2. Employee completes Lessons.
3. Employee completes Assessments.
4. The System calculates the final score.
5. The System validates completion requirements.

## Expected Outcome

The learning process is completed successfully.

---

# 6. Certificate Issuance

## Purpose

Issue a certificate after successful completion of a learning experience.

## Primary Actors

- Employee
- Manager
- System

## Business Flow

1. The System verifies completion requirements.
2. The System checks the organization's certificate policy.
3. If automatic issuance is enabled:
    - The System generates the Certificate.
4. Otherwise:
    - The Manager reviews the completion.
    - The Manager approves the issuance.
    - The System generates the Certificate.
5. The Employee receives the Certificate.

## Expected Outcome

A valid digital certificate is issued.
