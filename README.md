# Acquisition Management API

A production-ready backend platform for managing business acquisitions, listings, and deal workflows. The project focuses on scalable API development, containerized deployments, CI/CD automation, and operational best practices commonly used in modern software systems.

## Overview

This project was developed to explore the complete software delivery lifecycle, from API development to deployment and operational readiness. It includes authentication, business listing management, deal processing, database migrations, testing, logging, monitoring endpoints, and containerized deployment workflows.

The primary objective was to gain hands-on experience with backend engineering, DevOps practices, CI/CD automation, and production-focused system design.

## Tech Stack

### Backend
- Node.js
- Express.js

### Database
- PostgreSQL
- Drizzle ORM

### DevOps & Infrastructure
- Docker
- GitHub Actions

### Security & Validation
- JWT Authentication
- Arcjet
- Zod

### Testing & Monitoring
- Jest
- SuperTest
- Winston Logging

---

## Key Features

### Authentication & Authorization
- JWT-based authentication and authorization
- Secure route protection
- Role-based access control

### Business Listing Management
- Create, update, delete, and retrieve acquisition listings
- Manage listing lifecycle and ownership

### Deal Processing
- Submit acquisition offers
- Accept or reject deals
- Track deal status and history

### Database Management
- PostgreSQL integration using Drizzle ORM
- Migration-based schema management

### Reliability & Operations
- Structured application logging
- Health monitoring endpoints
- Input validation and centralized error handling
- Containerized deployment using Docker

### CI/CD & Automation
- Automated build and testing workflows
- Deployment-ready project structure
- Environment-based configuration management

---

## System Architecture

The application follows a layered architecture:

```text
Client
   │
   ▼
API Layer (Routes)
   │
   ▼
Service Layer (Business Logic)
   │
   ▼
Database Layer (Drizzle ORM + PostgreSQL)
   │
   ▼
Storage
```

Supporting Components:

- JWT Authentication
- Validation Middleware
- Logging & Monitoring
- Error Handling
- CI/CD Pipelines

This architecture improves maintainability, scalability, and troubleshooting.

---

## Installation

### Clone Repository

```bash
git clone https://github.com/<your-username>/acquisitions.git
cd acquisitions
```

### Install Dependencies

```bash
npm install
```

---

## Environment Variables

Create a `.env` file in the project root:

```env
PORT=3000
NODE_ENV=development

DATABASE_URL=

JWT_SECRET=

ARCJET_KEY=
```

---

## Running Locally

```bash
npm run dev
```

The application will be available at:

```text
http://localhost:3000
```

---

## Running with Docker

Build and run the application:

```bash
docker-compose up --build
```

Stop containers:

```bash
docker-compose down
```

---

## Testing

Run unit and integration tests:

```bash
npm test
```

Generate coverage report:

```bash
npm run test:coverage
```

---

## API Health Check

Verify service availability:

```http
GET /health
```

Example Response:

```json
{
  "status": "UP",
  "timestamp": "2025-01-01T10:00:00Z"
}
```

---

## Project Structure

```text
src/
├── controllers/
├── routes/
├── services/
├── middleware/
├── validations/
├── db/
├── utils/
├── tests/
└── app.js
```

---

## CI/CD Workflow

The project includes automated workflows for:

- Dependency installation
- Build validation
- Automated testing
- Code quality checks
- Deployment readiness verification

---

## Learning Outcomes

Through this project, I gained practical experience with:

- REST API development
- PostgreSQL database design
- ORM-based data access patterns
- JWT authentication
- Docker containerization
- CI/CD workflow implementation
- Application logging and monitoring
- Production-ready deployment practices
- Troubleshooting and debugging backend systems

---

## Future Enhancements

- Kubernetes deployment support
- Prometheus and Grafana monitoring
- OpenTelemetry distributed tracing
- Infrastructure as Code using Terraform
- Performance and load testing automation

---

## License

This project is intended for educational and portfolio purposes.
