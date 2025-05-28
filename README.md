# BobApp

### CI-CD
[![Frontend CI/CD](https://img.shields.io/github/actions/workflow/status/MickC0/FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD/ci-cd-frontend.yml?label=Frontend%20CI-CD&logo=Github)](https://github.com/MickC0/FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD/actions/workflows/ci-cd-frontend.yml)
[![Backend CI/CD](https://img.shields.io/github/actions/workflow/status/MickC0/FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD/ci-cd-backend.yml?label=Backend%20CI-CD&logo=Github)](https://github.com/MickC0/FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD/actions/workflows/ci-cd-backend.yml)

### Backend
[![Backend coverage](https://img.shields.io/codecov/c/github/MickC0/FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD?flag=backend&label=Backend%20coverage&logo=JUnit5)](https://mickc0.github.io/FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD/coverage-backend/index.html)
[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=MickC0_FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=MickC0_FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD)

[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=MickC0_FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD&metric=bugs)](https://sonarcloud.io/summary/new_code?id=MickC0_FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD)
[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=MickC0_FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD&metric=coverage)](https://sonarcloud.io/summary/new_code?id=MickC0_FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD)
[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=MickC0_FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=MickC0_FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD)

[Backend coverage report](https://mickc0.github.io/FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD/coverage-backend/index.html)

### Frontend
[![Frontend coverage](https://img.shields.io/codecov/c/github/wilzwert/BobApp?flag=frontend&label=Frontend%20coverage&logo=Jasmine)](https://wilzwert.github.io/BobApp/coverage-frontend/)
[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=MickC0_FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD_frontend&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=MickC0_FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD_frontend)

[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=MickC0_FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD_frontend&metric=bugs)](https://sonarcloud.io/summary/new_code?id=MickC0_FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD_frontend)
[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=MickC0_FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD_frontend&metric=coverage)](https://sonarcloud.io/summary/new_code?id=MickC0_FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD_frontend)
[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=MickC0_FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD_frontend&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=MickC0_FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD_frontend)


[Frontend coverage report](https://mickc0.github.io/FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD/coverage-frontend/)

## Table of contents

- [Clone project](#clone-project)
- [Frontend setup](#frontend-setup)
    - [Docker](#docker-for-frontend)
- [Backend setup](#backend-setup)
    - [Docker](#docker-for-backend)
- [Backend CI/CD](#backend-cicd-workflow)
- [Frontend CI/CD](#frontend-cicd-workflow)
- [KPIS](#kpis)
    - [Backend code coverage](#backend-code-coverage)
    - [Backend code quality analysis with SonarQube](#backend-code-quality-analysis-with-sonarqube)
    - [Frontend code coverage](#frontend-code-coverage)
    - [Frontend code quality analysis with SonarQube](#frontend-code-quality-analysis-with-sonarqube)
- [User reviews and issues](#user-reviews-and-issues)


## Clone project

> git clone https://github.com/MickC0/FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD.git


## Frontend setup

Go inside folder the front folder:

> cd front

Install dependencies:

> npm install

Launch Front-end:

> npm run start;

### Docker for frontend

Build the container:

> docker build -t bobapp-front .

Start the container:

> docker run -p 8080:8080 --name bobapp-front -d bobapp-front

## Backend setup

Go inside folder the back folder:

> cd back

Install dependencies:

> mvn clean install

Launch Back-end:

>  mvn spring-boot:run

Launch the tests:

> mvn clean install

### Docker for backend

Build the container:

> docker build -t bobapp-back .

Start the container:

> docker run -p 8080:8080 --name bobapp-back -d bobapp-back


## Backend CI/CD Workflow

A single pipeline handles both CI (tests, coverage, SonarCloud, Pages, Codecov) and CD (Docker build & push) for the Spring Boot backend

> .github/workflows/ci-cd-backend.yml

> [!NOTE]  
> These project use different triggers depending of the context :
> - `push` on `main`
> - `pull_request` targeting `main`
> - manual trigger (`workflow_dispatch`)

### Job `ci` (Tests, Coverage, SonarCloud, Pages, Codecov)

1. **Checkout code** (full history for Sonar blame)
2. **Setup JDK 17**
3. **Run Maven tests & generate Jacoco report** (continues on error)
4. **Verify coverage report exists**
5. **Upload coverage artifact**
6. **Publish coverage report** to GitHub Pages (`gh-pages`)
7. **Upload coverage** to Codecov
8. **Run SonarCloud scan** for `main`
9. **Check SonarCloud Quality Gate**
10. **Fail** if tests or quality gate fail

### Job `cd-docker` (Docker Build & Push)

This runs only if `ci` succeeds on a push to `main`:

1. **Checkout code**
2. **Setup JDK 17**
3. **Build with Maven** (skip tests)
4. **Login to Docker Hub**
5. **Extract Docker metadata** (tags from Git refs)
6. **Setup Docker Buildx**
7. **Build & push Docker image** to Docker Hub


## Frontend CI/CD workflow

A single pipeline handles both CI and CD for the Angular app

> .github/workflows/ci-cd-frontend.yml


> [!NOTE]  
> These project use different triggers depending of the context :
> - `push` on `main`
> - `pull_request` targeting `main`
> - manual trigger (`workflow_dispatch`)


### Job `ci` (Tests, Coverage, SonarCloud, Pages, Codecov)

1. **Checkout code (full history for Sonar blame)**
2. **Setup Node.js 22**
3. **Install Chrome for headless tests**
4. **Run Angular tests with coverage (continues on error)**
5. **Verify coverage report exists**
6. **Build _site/coverage-frontend and copy report**
7. **Publish coverage to GitHub Pages (gh-pages)**
8. **Upload coverage to Codecov**
9. **Run SonarCloud scan for main**
10. **Check SonarCloud Quality Gate**
11. **Fail if tests or quality gate fail**

### Job `cd-docker` (Docker Build & Push)

Runs only if ci succeeds on a push to main:

1. **Checkout code**
2. **Setup Node.js 22**
3. **Build Angular in production mode**
4. **Login to Docker Hub**
5. **Extract Docker metadata (tags from Git refs)**
6. **Setup Docker Buildx**
7. **Build & push Docker image to Docker Hub**


## KPIS

### Backend code coverage

Code coverage requirements for tests ar set up as follows in `./back/pom.xml`:

```xml 
  <limit>
      <counter>INSTRUCTION</counter>
      <value>COVEREDRATIO</value>
      <minimum>0.3</minimum>
  </limit>
 ```

> [!NOTE]
> As of now current requirements are very low but will allow code updates for the current application. As the overall code quality progresses, we should increase these values to 80%.

### Backend code quality analysis with SonarQube

Full report of the quality analysis for the main branch backend is available [here](https://sonarcloud.io/summary/overall?id=MickC0_FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD&branch=main).

A quality gate has been set up with requirements below.

For new code :

| Metric                     | Operator        | Value |
|----------------------------|-----------------|-------|
| Coverage                   | is less than    | 80.0% |
| Duplicated Lines (%)       | is greater than | 3.0%  |
| Maintainability Rating     | is worse than   | A     |
| Blocker Issues             | is greater than | 0     |
| Bugs                       | is greater than | 0     |
| Critical Issues            | is greater than | 1     |
| Reliability Rating         | is worse than   | A     |
| Security Hotspots Reviewed | is less than    | 100%  |
| Security Rating            | is worse than   | A     |

For overall code :
| Metric                     | Operator        | Value |
|----------------------------|-----------------|-------|
| Coverage                   | is less than    | 30.0% |



The quality gate passing status is reflected in the badge on top of this README.
Should the quality gate check fail on push, CI would fail too.

> [!NOTE]
> The expected code coverage ratio on overall code is very low and should be seen as an adjustable goal to increase overall code quality, as quickly as possible.


### Frontend code coverage

Code coverage requirements for tests are set up as follows in `./front/karma.conf.js`:
``` 
  statements: 75,
  branches: 75,
  functions: 50,
  lines: 75
 ```

> [!NOTE]
> As of now current values allow code updates for the current application, but as the overall code quality progresses, we should increase these values to 80%.

### Frontend code quality analysis with SonarQube

Full report of the quality analysis for the main branch frontend is available [here](https://sonarcloud.io/summary/overall?id=MickC0_FS-P10-Gerez-un-projet-collaboratif-en-int-grant-une-demarche-CI-CD_frontend&branch=main).

A quality gate has been set up with these requirements on new code :

| Metric                     | Operator | Value |
|----------------------------|----------|--------|
| Coverage                   | is less than | 80.0% |
| Duplicated Lines (%)       | is greater than | 3.0% |
| Maintainability Rating     |is worse than|A|
| Blocker Issues             | is greater than | 0     |
| Bugs                       |is greater than|0|
| Critical Issues            |is greater than|0|
| Reliability Rating         |is worse than|A|
| Security Hotspots Reviewed |is less than|100%|
| Security Rating            |is worse than|A|

The quality gate passing status is reflected in the badge on top of this README.
Should the quality gate check fail on push, CI would fail too.

> [!NOTE]
> These values are restrictive enough and allow quality development from now on, but should be fine-tuned as overall code quality increases.


## User reviews and issues

User reviews are very negative :

1. Je mets une une étoile car je ne peux pas en mettre zéro ! Impossible de poster une suggestion de blague, le bouton tourne  et fait planter mon navigateur ! - 1/5
2. #BobApp j'ai remonté un bug sur le post de vidéo il y a deux semaines et il est encore présent ! Les devs vous faites quoi ???? - 2/5
3. Ca fait une semaine que je ne reçois plus rien, j'ai envoyé un email il y a 5 jours mais toujours pas de nouvelles... - 1/5
4. J'ai supprimé ce site de mes favoris ce main, dommage, vraiment dommage.

Issues reported by the app's users should be converted into GitHub issues and addressed as quickly as possible. Users should also get quick feedback on the bugs statuses.

CI/CD pipelines will ensure bug fixes don't actually cause problems and regressions, thus ensuring that the overall user satisfaction increases.   
