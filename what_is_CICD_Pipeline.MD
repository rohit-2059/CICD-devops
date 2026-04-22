# What is a CI/CD Pipeline?

## CI/CD Meaning
- **CI/CD** stands for:
    - **Continuous Integration (CI)**
    - **Continuous Delivery/Deployment (CD)**
- It is a modern software practice where developers:
    - Make frequent code changes
    - Integrate changes quickly
    - Deliver updates safely and faster

## What is a CI/CD Pipeline?
A **CI/CD pipeline** is a **step-by-step automated workflow** that moves code from development to production.

> In simple words: it helps teams **build, test, and release software quickly and reliably**.

---

## Components of a CI/CD Pipeline

### 1) Commit Changes
- Developers write code and push commits to a version control system (e.g., **Git**).
- This starts the CI/CD process.
- Benefits:
    - Tracks all changes
    - Maintains version history
    - Enables team collaboration

### 2) Trigger Build
- The CI/CD tool detects the new commit automatically.
- It triggers the build process without manual action.
- Benefit:
    - Ensures every new change is validated immediately

### 3) Build
- Source code is compiled and packaged into a deployable artifact.
- Examples of artifacts:
    - Binary executable
    - Docker image
- Common tools:
    - **Maven**, **Gradle**, **Ant** (Java)
    - **Docker** (containerized apps)
- Benefit:
    - Confirms code compiles and dependencies are resolved

### 4) Notify Build Outcome
- Team gets notified whether build **passed** or **failed**.
- Notification channels:
    - Email
    - Slack / Microsoft Teams
    - CI dashboards (Jenkins, GitLab CI, etc.)
- Benefit:
    - Fast feedback helps fix issues early

### 5) Run Tests
- Automated tests run on the build artifact.
- Test types:
    - Unit tests
    - Integration tests
    - End-to-end tests
- Common testing tools:
    - **JUnit**, **TestNG**, **Selenium**, **pytest**
- Benefit:
    - Prevents bugs/regressions and checks quality

### 6) Notify Test Outcome
- Test results are shared with the team.
- Channels:
    - Email
    - Chat tools
    - Dashboards
- Benefit:
    - Developers can quickly address failed tests

### 7) Deliver to Staging
- If tests pass, artifact is deployed to a **staging** environment.
- Staging closely mirrors production for final checks.
- Common deployment tools:
    - **Ansible**, **Chef**, **Puppet**, **Kubernetes**
    - Cloud tools like **AWS CodeDeploy**
- Benefit:
    - Reduces risk before production release

### 8) Deploy to Production
- After validation, release is promoted to **production**.
- Deployment can be:
    - Automatic
    - Manual approval-based
- Common strategies:
    - Blue-Green deployment
    - Canary releases
    - Rolling updates
- Benefit:
    - Safer releases with minimal downtime

---

## Quick Summary
A CI/CD pipeline automates the full path from **code commit → build → test → staging → production**, giving faster delivery, better quality, and lower release risk.