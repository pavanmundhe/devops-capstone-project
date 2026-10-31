# DevOps Capstone Project — Customer Accounts Microservice

[![CI](https://github.com/pavanmundhe/devops-capstone-project/actions/workflows/ci-build.yaml/badge.svg?branch=main)](https://github.com/pavanmundhe/devops-capstone-project/actions/workflows/ci-build.yaml)

## Project details

- **Course:** IBM DevOps Capstone Project (Coursera)
- **Objective:** Build and improve a RESTful Customer Accounts microservice using Agile planning, test-driven development, continuous integration, containers, and Kubernetes.
- **Service:** Flask API backed by PostgreSQL.
- **Repository:** https://github.com/pavanmundhe/devops-capstone-project

## Account API

The service supports creating, listing, reading, updating, and deleting accounts. Run the service tests with:

```bash
nosetests
```

The test configuration enables the coverage report. The service target is at least 95% coverage.

## Development

Install the dependencies with `make install`. Start PostgreSQL with `make db`, then run the service with `make run`. Run `make lint` to check code style.

The source code is in `service/`, automated tests are in `tests/`, and deployment resources are in `deploy/` and `tekton/`.

## User story template

The reusable story format is in [user-story.md](user-story.md).

## License

This project uses the Apache 2.0 license included with the starter template.
