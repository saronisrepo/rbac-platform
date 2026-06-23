# RBAC Platform

## Overview

A multi-tenant Role-Based Access Control (RBAC) platform designed to centralize authentication and authorization across multiple applications.

The platform provides:

- User Management
- Role Management
- Policy Management
- Permission Evaluation
- JWT Authentication
- Multi-Tenant Support
- Dynamic Configuration

## Architecture

```text
Frontend
    |
API Gateway
    |
RBAC Service
    |
Authorization Engine
    |
PostgreSQL
```

## Features

### Authentication
- JWT Access Tokens
- Refresh Tokens
- Login / Logout
- Token Validation

### Authorization
- Role Based Access Control (RBAC)
- Dynamic Policy Evaluation
- Permission Matrix
- Resource-level Access

### Multi-Tenant Support
- Organization Isolation
- Tenant-specific Policies
- Tenant-specific Roles

## Tech Stack

- Python
- FastAPI
- PostgreSQL
- SQLAlchemy
- Alembic
- Docker
- JWT

## API Examples

### Login

```http
POST /auth/login
```

### Evaluate Permission

```http
POST /evaluate
```

### Create Role

```http
POST /roles
```

## Architecture

![RBAC Architecture](architecture.png)

## System Design

The platform follows a centralized authorization model.

### Components

- Authentication Service
- Authorization Engine
- Role Management
- Policy Management
- Permission Evaluation
- Multi-Tenant Configuration

### Authorization Flow

User → JWT Validation → Role Lookup → Policy Evaluation → Access Decision

## Future Enhancements

- ABAC Support
- Keycloak Integration
- Amazon Cognito Integration
- Audit Logging
- Redis Permission Cache

## Author

Saroni
