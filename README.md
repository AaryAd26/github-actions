🚀 Learning CI/CD with GitHub Actions

Recently, I started learning CI/CD pipelines using GitHub Actions as part of my DevOps journey.
The goal is to automate tasks like building, testing, and deploying applications directly from GitHub.

🔹 What I’m learning:
• Creating workflows using YAML
• Automating builds and tests
• Using runners in GitHub Actions
• Working with Docker in CI/CD pipelines
• Understanding jobs, steps, triggers, and actions
• Debugging workflow errors and fixing pipeline issues

One of the most interesting things is how every push to the repository can automatically trigger a workflow.

Example GitHub Actions Workflow:

```yaml
name: CI Pipeline

on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout Code
        uses: actions/checkout@v4

      - name: Show Current Directory
        run: pwd

      - name: List Files
        run: ls -la

      - name: Print Date
        run: date

      - name: Build Docker Image
        run: docker build -t my-app .
```

🔹 Some useful commands I practiced:

```bash
git add .
git commit -m "Added GitHub Actions workflow"
git push origin main
```

```bash
docker build -t my-app .
docker run -p 3000:3000 my-app
```

Through this learning process, I’m understanding how modern software teams automate development workflows and deployments efficiently.

Still learning and improving every day in DevOps 🚀

#DevOps #GitHubActions #CICD #Docker #Automation #Learning #OpenToWork #CloudComputing
