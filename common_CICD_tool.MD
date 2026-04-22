# CI/CD Tools — Overview

Continuous Integration (CI) and Continuous Delivery/Deployment (CD) tools streamline development, testing, and deployment. Some tools focus on integration, while others focus on build/test automation and release management.

Jenkins is a widely used open-source CI/CD server that can orchestrate builds, tests, and deployments.

## Typical Jenkins CI/CD Workflow

1. **Developer Commit**: Code is pushed to a remote repository (GitHub, GitLab, Bitbucket).
2. **Trigger**: Jenkins detects the change (webhook or polling).
3. **Build**: Jenkins runs the build (Maven, Gradle, Docker, etc.).
4. **Test**: Automated tests execute to validate quality.
5. **Deploy**: Successful builds are deployed to staging or production.
6. **Feedback**: Notifications (email, Slack, etc.) inform developers of success or failure.

## Other CI/CD Tools

- **GitHub Actions**: Integrated CI/CD for GitHub repositories.
- **GitLab CI/CD**: Built-in CI/CD for GitLab projects.
- **CircleCI**: Cloud-based CI/CD with support for various languages and platforms.
- **Travis CI**: Cloud-based CI/CD, popular for open-source projects.
- **Bamboo**: Atlassian CI/CD server; integrates with Jira and Bitbucket.