# DevOps Capstone Project — Customer Accounts Microservice

## Project details

- **Course:** IBM DevOps Capstone Project (Coursera)
- **Repository:** https://github.com/pavanmundhe/devops-capstone-project
- **Starter code:** IBM's [DevOps Capstone template](https://github.com/ibm-developer-skills-network/aolwx-devops-capstone-template), copied using GitHub's **Use this template** workflow.
- **Objective:** Plan and build a RESTful Customer Accounts microservice over Agile sprints using test-driven development, CI, containers, and Kubernetes.
- **Current scope:** Sprint 0 setup and Agile planning; implementation and later sprint work will be tracked in GitHub Issues and the project board.

## Development environment

The course labs use the IBM Developer Skills Network Cloud IDE with OpenShift. In that environment, initialize the project by sourcing the setup script:

```bash
source bin/setup.sh
```

This installs Python 3.9, creates and activates a virtual environment, and configures the lab environment. Do not run the setup script as a standalone program; source it as shown.

## Useful commands

Activate the virtual environment if needed:

```bash
source ~/venv/bin/activate
```

Install dependencies:

```bash
make install
```

Start the PostgreSQL container if it is unavailable:

```bash
make db
```

## Project layout

The Flask service is in `service/`; tests are in `tests/`. Business logic and persistence live in the model layer, while REST endpoints are defined in the routes layer.

## Account data model

| Field | Type | Optional |
|---|---|---|
| id | Integer | No |
| name | String(64) | No |
| email | String(64) | No |
| address | String(256) | No |
| phone_number | String(32) | Yes |
| date_joined | Date | No |

## Project objective

Complete the Customer Accounts service with REST APIs to read, update, delete, and list accounts while maintaining at least 95% code coverage. Follow test-driven development: write tests for the expected behavior, then implement the code that makes them pass.

## License

This project uses the Apache 2.0 license included with the starter template.
