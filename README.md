# RETAIL ORDER MANAGEMENT API

## Overview
A scalable backend system built using FastAPI for managing users, products, inventory, and orders.The application supports JWT authentication, role-based access control, and follows clean architecture principles.
Designed to demonstrate production-ready backend engineering practices.

## Tech Stack
- Backend: Python, FastAPI
- Database: PostgreSQL
- ORM: SQLAlchemy
- Auth: JWT (OAuth2 Password Flow)
- Migrations: Alembic
- Cloud Ready: AWS / Docker (optional)
- Docs: Swagger (OpenAPI)

## Authentication & Authorization
- JWT-based authentication
- Role-based access:
    1. ADMIN – full access
    2. STAFF – operational access
    3. VIEWER – read-only

## Core Features
- User registration & login
- Secure role-based APIs
- Product & inventory management
- Order processing
- Clean error handling
- Database migrations

## Project Structure
<pre>
app/
 ├── api/
 ├── core/
 ├── database/
 ├── models/
 ├── schemas/
 ├── services/
 └── main.py
</pre>

## Setup Instructions
1. Clone the repository
    git clone <repo-url>
2. Create virtual environment
    python -m venv venv
    source venv/bin/activate
3. Install dependencies
    pip install -r requirements.txt
4. Configure environment
    cp .env.example .env
5. Run migrations
    alembic upgrade head
6. Start server
    uvicorn app.main:app --reload

## API Documentation
Swagger UI available at:
http://localhost:8000/docs

## Future Enhancements
- Dockerization
- CI/CD pipeline
- Monitoring (Prometheus)
- Cloud deployment


Author: **Vaishnavi**\
Backend Python Developer (FastAPI, Cloud, APIs)
