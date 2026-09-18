# DevOps Intern Project – CI/CD Pipeline with Docker

A simple Node.js application demonstrating containerization and CI/CD automation.

## Tech Stack
- Node.js + Express
- Docker
- GitHub Actions (CI/CD)

## Features
- REST API with health check endpoint
- Dockerized application
- Automated CI/CD pipeline: install → test → build Docker image on every push

## How to Run

### Locally
\`\`\`bash
npm install
npm start
\`\`\`

### With Docker
\`\`\`bash
docker build -t devops-intern-app .
docker run -p 3000:3000 devops-intern-app
\`\`\`

## CI/CD Pipeline
On every push to `main`, GitHub Actions automatically:
1. Installs dependencies
2. Runs tests
3. Builds the Docker image

See `.github/workflows/ci-cd.yml`
