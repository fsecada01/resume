# Francis Secada

New York, NY | linkedin.com/in/francissecada | github.com/fsecada01

## Professional Summary

Backend engineer with 10+ years in data and backend engineering, building APIs, microservices, and data pipelines across financial services, healthcare, cybersecurity, and media. Expert in Python (FastAPI, Django, Flask) and PostgreSQL, with production experience in event-driven systems on AWS, performance work on high-volume services, and LLM integrations. Most recently a technical lead at The Motley Fool (100+ merged PRs across 11 production repositories). Maintainer of two open-source Python libraries on PyPI. Principal of FJS Services Inc. since 2014, delivering full-stack systems for startups and small businesses.

## Technical Skills

- **Languages:** Python (expert, 7+ yrs), TypeScript/JavaScript, SQL (PostgreSQL), Rust (secondary)
- **Backend & APIs:** FastAPI, Django/Django Ninja/DRF, Flask, Litestar, SQLAlchemy/SQLModel, REST API design, microservices, service decomposition
- **Distributed Systems:** AWS EventBridge/SQS, Temporal (durable workflows), Celery/Taskiq, asyncio, event-driven pipelines
- **Data:** PostgreSQL (CTEs, window functions, `DISTINCT ON`, bulk upsert, indexing), Redis, MongoDB, Pandas, ETL pipelines
- **Cloud & DevOps:** AWS (ECS, Lambda, EventBridge, SQS, RDS, S3), Azure (Functions, API Management, DevOps), Docker, Kubernetes, Terraform, GitHub Actions, DataDog, Prometheus/Grafana
- **Frontend:** React, Vue.js, TypeScript, HTMX
- **AI/LLM:** OpenAI (GPT-4o), Pydantic AI, MCP server authorship, Claude Code
- **Domain:** HIPAA/HITECH, RBAC, audit logging, financial services and regulatory reporting

## Professional Experience

### The Motley Fool

**Python API and Microservices Development Lead (Contractor) | Oct 2025 - Jul 2026 | Remote**

Technical lead across production Django and FastAPI services for portfolio data, investing intelligence, and subscription lifecycle management. 100+ merged PRs across 11 production repositories.

- Redesigned a sequential market-data fetch into a concurrent fan-out with a larger HTTP connection pool, removing thread-pool exhaustion and request timeouts under load (benchmarked from about 1.2s to 300ms on large portfolios).
- Ran a five-phase caching rollout on a Django portfolio service; a reporting endpoint went from 55,412ms to 5ms on cache hits (1,377 queries down to 134 on a miss).
- Rewrote an N+1 ingestion path as a three-stage bulk pipeline with PostgreSQL upserts, a 99.9% query reduction, and built an async streaming generator for loads of 50K+ financial instruments.
- Split a data harvest into parallel fetches and short atomic bulk writes; a bulk options load fell from about 20 minutes to under 2 in production.
- Showed that a categorical field could not classify instruments (98.68% class overlap), then built a name-based heuristic validated against 3,399 confirmed records that corrected 992 misclassified production records.
- Built a subscription event pipeline on AWS EventBridge and SQS with pattern-matching dispatch and stateless handlers; Temporal ran the durable multi-step workflows downstream.
- Owned a cross-service capability migration from a legacy service to a newer one, with an idempotency layer that kept both consistent through a phased cutover.
- Enforced import-boundary contracts and structured DataDog telemetry on every PR, and wrote a CLI that migrates Python projects to uv.

### FJS Services Inc.

**Owner / Principal Consultant | Jan 2014 - Present | Brooklyn, NY**

Independent consultancy building software for startups, small businesses, and nonprofits in fintech, healthcare, and SaaS.

- Designed, built, and deployed 15+ full-stack web applications and API services, from MVP through production, in Python (FastAPI, Flask, Django) on AWS and GCP.
- Worked directly with founders and product owners on stack selection, architecture, and roadmap priorities for early-stage products.
- Built ETL pipelines, automation workflows, and AI features using OpenAI integrations, vector databases, and event-driven architectures.
- Set up containerized CI/CD on Docker, Kubernetes, GitHub Actions, and Azure DevOps.
- Built HIPAA-compliant healthcare data platforms and portfolio-tracking and compliance-monitoring tools for boutique investment firms.

### Cleveland Clinic

**Software Engineer (Contract) | May 2023 - Nov 2023 | Remote**

- Owned the migration of a monolithic Django application to modular microservices using FastAPI on Azure Functions behind API Management, improving scalability for high-volume healthcare data workflows.
- Engineered REST APIs for complex medical data queries using PostgreSQL indexing, window functions, and views; implemented Redis-based caching and asynchronous FastAPI endpoints.
- Tuned ETL and cohort-generation pipelines with Pandas and PostgreSQL query optimization.
- Partnered with clinical teams to meet HIPAA/HITECH requirements, implementing secure data-access patterns and audit logging for sensitive healthcare information.

### HSBC

**Software Engineer (Contract) | May 2020 - Nov 2022 | Jersey City, NJ & Remote**

- Led the re-architecture of a global cybersecurity control platform from a Django monolith into containerized microservices on AWS ECS, with event-driven Lambda functions for compliance monitoring.
- Built REST APIs with Flask and FastAPI for financial risk analysis, using PostgreSQL CTEs and window functions to serve real-time regulatory reporting dashboards.
- Built TypeScript React and Vue.js components that consume real-time market data and compliance APIs.
- Set up Prometheus and Grafana monitoring for API health, error rates, and latency.
- Mentored junior engineers on test-driven development, Git branching, and financial systems work, and contributed to hiring two of them.

## Selected Projects

**TextSpitter** ([PyPI](https://pypi.org/project/TextSpitter/), [GitHub](https://github.com/fsecada01/TextSpitter)) - Python library for text extraction from PDF, DOCX, CSV, and 50+ source-code formats. Version 2.0 added a Rust/PyO3 core with a pure-Python fallback. 70+ tests on a Python 3.12-3.14 CI matrix. Maintained since 2018. *(Python, Rust, PyMuPDF)*

**SQLModel CRUD Utilities** ([PyPI](https://pypi.org/project/sqlmodel-crud-utilities/), [GitHub](https://github.com/fsecada01/SQLModel-CRUD-Utilities)) - Sync and async CRUD layer over SQLModel and SQLAlchemy with transaction context managers, soft deletes, pagination, audit mixins, and a typed exception hierarchy. *(Python, SQLModel, PostgreSQL)*

**Ranked Jobs** ([rankedjobs.com](https://www.rankedjobs.com/)) - Job-search platform that matches and ranks postings with NLP. Its API microservice aggregates listings from 12 sources through a plugin system, with Taskiq workers and a Prometheus metrics endpoint. *(Python, FastAPI, Django, PostgreSQL, Redis)*

**AccountBridge** - Household budgeting app with a provider-agnostic OAuth account-linking core (Plaid and Teller) and a companion MCP server exposing 14 financial-data tools to Claude. *(Python, Litestar, MCP, OAuth)*

**Formana** - Django platform automating New York State's Medicaid waiver programs for traumatic brain injury and nursing-home transition, with HIPAA/HITECH controls and GPT-4o-generated clinical narratives. *(Python, Django Ninja, Celery, PostgreSQL)*

## Education

**Master of Public Administration (MPA)** - The Bernard M. Baruch College, City University of New York
Austin W. Marxe School of Public and International Affairs | Conferred September 2015
Primary research on cost savings and social determinants in Medicaid expansion across U.S. states.
