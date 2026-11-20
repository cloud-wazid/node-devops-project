# Node DevOps Project

A Node.js application with a Dockerfile and Jenkinsfile for automated build and deployment.

## Tech Used
Node.js, Docker, Jenkins, Git/GitHub

## Project Structure
- `app.js` – Node.js application
- `package.json` – dependencies and scripts
- `Dockerfile` – container image definition
- `Jenkinsfile` – CI/CD pipeline definition

## Pipeline Flow
Git push → Jenkins pipeline → Docker image build → <run container / push image>

Pipeline stages: <Checkout, Build image, Deploy, ...>

## Run Locally
```bash
git clone https://github.com/cloud-wazid/node-devops-project.git
cd node-devops-project
npm install
node app.js
```

## Run with Docker
```bash
docker build -t node-devops-project .
docker run -d -p <PORT>:<PORT> node-devops-project
```

Then open `http://localhost:<PORT>`.

## What I Learned
- Writing a Dockerfile for a Node.js app
- Defining a Jenkins pipeline as code with a Jenkinsfile
