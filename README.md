# Classwork Assignment 1

You are given a Python application and a client has requested your help to run it in a Docker container and automate the process of building the Docker image.

## Start up

Install necessary dependencies

```bash
pip3 install -r src/requirements.txt
```
Start the application

```bash
python3 src/app.py
```

## Tasks
- Create a new **public** repository and use this one as a template.
- Containerize the Python application in the `src/` directory. Create a Dockerfile and use ubuntu as a base image.
- Validate locally that the container is working.
- Create a GitHub Actions workflow that builds the Docker image and publishes it to your personal DockerHub account on every push to the main branch.

### Security
- Implement IDE-level code analysis with Snyk (install Snyk plugin for your IDE)
- Scan the application code with SonarCloud and Snyk as part of the existing workflow
- Scan the built Docker image with Trivy as part of the existing workflow
- Implement a new GitHub workflow with SonarCloud at Merge Request

### Bonus
- Optimize the size of the Docker image. Use a more minimal base image.