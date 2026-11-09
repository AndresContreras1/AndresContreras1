# Andrés Felipe Contreras Báez

**Systems Engineering student · backend and full-stack developer · Bogotá, Colombia**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-andres--contreras--baez-0A66C2)](https://linkedin.com/in/andres-contreras-baez)
[![Email](https://img.shields.io/badge/Email-andresfcontreras%40javeriana.edu.co-EA4335?logo=gmail&logoColor=white)](mailto:andresfcontreras@javeriana.edu.co)
![Javeriana](https://img.shields.io/badge/Pontificia%20Universidad%20Javeriana-6th%20semester%20%C2%B7%202028-2C5697)
![Spanish](https://img.shields.io/badge/Spanish-native-555555)
![English](https://img.shields.io/badge/English-C1-555555)
![French](https://img.shields.io/badge/French-B1-555555)

Systems Engineering student at Pontificia Universidad Javeriana, Bogotá, and freelance developer.
I build backends that hold up when they are put under pressure, and I write the tests that prove it.

These days I work on e-commerce automation for a Shopify store operator based in Paris: a Python
pipeline that turns one spreadsheet row into a published product — specs, French copy, variants,
images and SKUs — in about 25 seconds instead of half an hour of manual work.

## Tech stack

**Languages**

![Java](https://img.shields.io/badge/Java-007396?logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4169E1?logo=postgresql&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?logo=kotlin&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?logo=cplusplus&logoColor=white)

**Web and APIs**

![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring%20Security-JWT-6DB33F?logo=springsecurity&logoColor=white)
![OpenAPI](https://img.shields.io/badge/REST-OpenAPI-6BA539?logo=openapiinitiative&logoColor=white)
![Hibernate](https://img.shields.io/badge/JPA-Hibernate-59666C?logo=hibernate&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-19-DD0031?logo=angular&logoColor=white)
![RxJS](https://img.shields.io/badge/RxJS-B7178C?logo=reactivex&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?logo=express&logoColor=white)

**Mobile**

![Android](https://img.shields.io/badge/Android-34A853?logo=android&logoColor=white)
![Jetpack Compose](https://img.shields.io/badge/Jetpack%20Compose-4285F4?logo=jetpackcompose&logoColor=white)

**Databases**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=white)
![H2](https://img.shields.io/badge/H2-0000BB)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?logo=mongodb&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?logo=firebase&logoColor=black)
![Flyway](https://img.shields.io/badge/Flyway-CC0200?logo=flyway&logoColor=white)

**Testing and quality**

![JUnit 5](https://img.shields.io/badge/JUnit%205-25A162?logo=junit5&logoColor=white)
![Mockito](https://img.shields.io/badge/Mockito-78A641)
![Testcontainers](https://img.shields.io/badge/Testcontainers-291A3F)
![ArchUnit](https://img.shields.io/badge/ArchUnit-555555)
![Selenium](https://img.shields.io/badge/Selenium-43B02A?logo=selenium&logoColor=white)
![k6](https://img.shields.io/badge/k6-7D64FF?logo=k6&logoColor=white)
![SonarCloud](https://img.shields.io/badge/SonarCloud-F3702A?logo=sonarqubecloud&logoColor=white)

**DevOps**

![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?logo=githubactions&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white)
![Scrum](https://img.shields.io/badge/Scrum-Agile-009FDA?logo=scrumalliance&logoColor=white)

**AI and automation**

![Claude API](https://img.shields.io/badge/Claude%20API-D97757?logo=claude&logoColor=white)
![Python pipelines](https://img.shields.io/badge/Python-pipelines-3776AB?logo=python&logoColor=white)

**Foundations:** algorithms, design patterns, software architecture and distributed systems.

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

## Beyond code

- **Power BI research seedbed**, Pontificia Universidad Javeriana — data analyst. Dashboards that support the management of Joy, an ice cream shop.
- **Cybersecurity research seedbed**, Pontificia Universidad Javeriana — modern cybersecurity and how it changes with artificial intelligence.

## What is next

Taking BPMN Process Manager from portfolio to product: a deployed instance that can be opened and not
only cloned, passkeys, a diagram editor built on bpmn-js, and the app in Spanish, English and French.
