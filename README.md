# Simple FastAPI App

Simple FastAPI Application

## Features

- Domain layer with sample entities
- Application layer with abstractions for:
  - Example use cases
  - Cross-cutting concerns (logging, validation)
- Infrastructure layer with:
  - Authentication
  - SQLAlchemy, PostgreSQL (you can change to SQLite for development in database/core.py)
  - Rate limiting on registration
- Testing projects
  - Pytest unit tests
  - Pytest integration tests (e2e tests)

I'm open to hearing your feedback about the template and what you'd like to see in future iterations. DM me on LinkedIn or email me.

---

## Installation

Install all dependencies:

```bash
pip install -r requirements-dev.txt
```

## Running the Application

### Using Docker with PostgreSQL

1. Install Docker Desktop
2. Run `docker compose up --build`
3. Run `docker compose down` to stop all services

### Running Locally (without PostgreSQL or Docker)

1. In `database/core.py`, change the `DATABASE_URL` to SQLite
2. Run `uvicorn src.main:app --reload`

## Running Tests

Run all tests:

```bash
pytest
```
