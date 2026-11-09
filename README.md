# Andrés Felipe Contreras Báez

Systems Engineering student at Pontificia Universidad Javeriana, Bogotá, and freelance developer.
I build backends that hold up when they are put under pressure, and I write the tests that prove it.

These days I work on e-commerce automation for a Shopify store operator based in Paris: a Python
pipeline that turns one spreadsheet row into a published product — specs, French copy, variants,
images and SKUs — in about 25 seconds instead of half an hour of manual work.

- **Studying** B.S. in Systems Engineering, 6th semester · expected 2028
- **Working with** Java · Spring Boot · Angular · Kotlin and Jetpack Compose · Python · Node.js · PostgreSQL · Docker
- **Languages** Spanish (native) · English C1 · French B1
- **Reach me** [andresfcontreras@javeriana.edu.co](mailto:andresfcontreras@javeriana.edu.co) · [LinkedIn](https://linkedin.com/in/andres-contreras-baez)

## What I am building

| Project | What it is | Stack | Status |
|---|---|---|---|
| [**BPMN Process Manager**](https://github.com/AndresContreras1/bpmn-process-manager-api) | Multi-tenant platform where online stores model their order workflows as BPMN diagrams, publish them as immutable versions and run orders on them, against simulated partners and a clock of their own | Java 25 · Spring Boot 4 · Angular 19 · PostgreSQL · Docker | Active · 1,527 tests, 96% line coverage |
| [**Mixtapp**](https://github.com/AndresContreras1/Mixtapp) | Android app to rate, review and discover albums, songs and artists with the people you follow, with live notifications. Semester project for Mobile Computing, built as a team | Kotlin · Jetpack Compose · Hilt · Firebase · Retrofit | In progress |
| [**Mixtapp Backend**](https://github.com/AndresContreras1/mixtapp-backend) · [**Functions**](https://github.com/AndresContreras1/mixtapp-functions) | The REST API the app consumes for users, albums and reviews, and the Cloud Functions that keep the data consistent and send the notifications | Node.js · Express · Sequelize · PostgreSQL · Firebase | In progress |

### Inside BPMN Process Manager

- **Security of accounts:** session in `HttpOnly` cookies with CSRF, a second factor with an authenticator app
  and recovery codes, signing in with Google or Microsoft, and passwords as NIST SP 800-63B-4 asks.
- **Security of data:** every store isolated twice, by the build and by row-level security in PostgreSQL, rate
  limits shared by every instance, and an audit trail chained with SHA-256 that nobody can change.
- **Running processes:** cases that walk a published version, task trays per role, messages with simulated
  payments, carrier and customer, and a dashboard with cycle times.
- **Built to be operated:** Java 25 on virtual threads, an event outbox and a job queue in PostgreSQL,
  OpenTelemetry traces, Prometheus metrics and hardened Docker images.

## How I work

- **Everything enters through a pull request.** No direct pushes to the main branch, short branches, one branch per block of work.
- **Tests are part of "done",** not a later chore: unit tests, integration tests on real databases with Testcontainers, end-to-end tests with Selenium, load thresholds with k6 and nightly mutation testing.
- **The pipeline is the referee.** On every pull request GitHub Actions builds and tests on Linux and Windows, runs the end-to-end and load tests against the whole stack, and checks SonarCloud, CodeQL, Trivy and gitleaks.
- **Architecture rules are enforced by code,** not by good intentions: 41 ArchUnit rules and Spring Modulith keep the layers and the modules where they belong.
- **A README is part of the product.** If someone cannot run the project and understand why it exists, the project is not finished.

## Beyond code

- **Power BI research seedbed**, Pontificia Universidad Javeriana — data analyst. Dashboards that support the management of Joy, an ice cream shop.
- **Cybersecurity research seedbed**, Pontificia Universidad Javeriana — modern cybersecurity and how it changes with artificial intelligence.

## What is next

Taking BPMN Process Manager from portfolio to product: a deployed instance that can be opened and not
only cloned, passkeys, a diagram editor built on bpmn-js, and the app in Spanish, English and French.
