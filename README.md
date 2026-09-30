# Andrés Felipe Contreras Báez

Systems Engineering student at Pontificia Universidad Javeriana, Bogotá, and freelance developer.
I build backends that hold up when they are put under pressure, and I write the tests that prove it.

These days I work on e-commerce automation for a Shopify store operator based in Paris: a Python
pipeline that turns one spreadsheet row into a published product — specs, French copy, variants,
images and SKUs — in about 25 seconds instead of half an hour of manual work.

- **Studying** B.S. in Systems Engineering, 6th semester · expected 2028
- **Working with** Java · Spring Boot · Angular · Kotlin and Jetpack Compose · Python · PostgreSQL · Docker
- **Languages** Spanish (native) · English C1 · French B1
- **Reach me** [andresfcontreras@javeriana.edu.co](mailto:andresfcontreras@javeriana.edu.co) · [LinkedIn](https://linkedin.com/in/andres-contreras-baez)

## What I am building

| Project | What it is | Stack | Status |
|---|---|---|---|
| [**BPMN Process Manager**](https://github.com/AndresContreras1/bpmn-process-manager-api) | Multi-tenant platform where an online store models its order workflows as BPMN diagrams, publishes them as immutable versions and runs real orders on them | Spring Boot · Angular 19 · PostgreSQL · Docker | Active · 1,176 tests, 96% line coverage |
| [**Game Store**](https://github.com/AndresContreras1/shopscale-ai) | Online store that never oversells, scales horizontally and turns its own sales data into an executive report | Spring Boot · Angular · Redis · Nginx · Gemini API | In progress |
| [**Mixtapp**](https://github.com/AndresContreras1/Mixtapp) | Android app for rating and reviewing music albums, built with a team of three | Kotlin · Jetpack Compose · Firebase · Hilt | In progress |

## How I work

- **Everything enters through a pull request.** No direct pushes to the main branch, short branches, one branch per block of work.
- **Tests are part of "done",** not a later chore: unit tests, integration tests on real databases with Testcontainers, end-to-end tests with Selenium, and load thresholds with k6.
- **The pipeline is the referee.** GitHub Actions runs the build, the tests and SonarCloud on every pull request.
- **Architecture rules are enforced by code,** not by good intentions: 40 ArchUnit rules keep the layers where they belong.
- **A README is part of the product.** If someone cannot run the project and understand why it exists, the project is not finished.

## Beyond code

- **Power BI research seedbed**, Pontificia Universidad Javeriana — data analyst. Dashboards that support the management of Joy, an ice cream shop.
- **Cybersecurity research seedbed**, Pontificia Universidad Javeriana — modern cybersecurity and how it changes with artificial intelligence.

## What is next

Deploying the two web projects so they can be opened and not only cloned, and closing Game Store's
roadmap: connecting inventory to warehouses and marketplaces, and automating purchase orders.
